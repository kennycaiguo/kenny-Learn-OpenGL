#include <math.h>
#include <gl/glut.h>
#include <iostream>
using namespace std;

struct  Point2 {
	double x;
	double y;

	Point2(int px, int py) { x = px; y = py; }
};

Point2 P0(100, 200);
Point2 P1(350, 200);
Point2 derP0(200, 200);
Point2 derP1(200, 200);

bool mouseLeftDown = false;
bool mouseRightDown = false;

/* 计算Hermite曲线 */
void Hermit(int n) {
	float f1, f2, f3, f4;

	double deltaT = 1.0 / n;

	glBegin(GL_LINE_STRIP);
	for (int i = 0; i <= n; i++) {

		double T = i * deltaT;

		f1 = 2.0 * pow(T, 3) - 3.0 * pow(T, 2) + 1.0;
		f2 = -2.0 * pow(T, 3) + 3.0 * pow(T, 2);
		f3 = pow(T, 3) - 2.0 * pow(T, 2) + T;
		f4 = pow(T, 3) - pow(T, 2);

		glVertex2f(f1 * P0.x + f2 * P1.x + f3 * derP0.x + f4 * derP1.x,
			f1 * P0.y + f2 * P1.y + f3 * derP0.y + f4 * derP1.y);
	}
	glEnd();
}

/* 用鼠标进行绘制，完成后可改变控制点，拖动即可 */
void display() {
	glClear(GL_COLOR_BUFFER_BIT);

	glLineWidth(1.5);
	glColor3f(1.0, 0.0, 0.0);
	glBegin(GL_LINES);
	glVertex2f(P0.x, P0.y);
	glVertex2f(P0.x + derP0.x / 4, P0.y + derP0.y / 4);
	glVertex2f(P1.x, P1.y);
	glVertex2f(P1.x - derP1.x / 4, P1.y - derP1.y / 4);
	glEnd();

	glColor3f(0.0, 0.0, 1.0);
	glPointSize(10.0f);

	glBegin(GL_POINTS);
	glVertex2f(P0.x, P0.y);
	glVertex2f(P0.x + derP0.x / 4, P0.y + derP0.y / 4);
	glVertex2f(P1.x, P1.y);
	glVertex2f(P1.x - derP1.x / 4, P1.y - derP1.y / 4);
	glEnd();

	Hermit(20);

	glFlush();
	glutSwapBuffers();
}

void init() {
	glClearColor(0.0, 0.0, 0.0, 0.0);
	glShadeModel(GL_FLAT);
}

void myReshape(int w, int h) {
	glViewport(0, 0, (GLsizei)w, (GLsizei)h);
	glMatrixMode(GL_PROJECTION);
	glLoadIdentity();
	gluOrtho2D(0.0, (GLsizei)w, (GLsizei)h, 0.0);
	glMatrixMode(GL_MODELVIEW);
	glLoadIdentity();
}

void mouse(int button, int state, int x, int y) {
	if (button == GLUT_LEFT_BUTTON && state == GLUT_DOWN)
		mouseLeftDown = true;

	if (button == GLUT_LEFT_BUTTON && state == GLUT_UP)
		mouseLeftDown = false;

	if (button == GLUT_RIGHT_BUTTON && state == GLUT_DOWN)
		mouseRightDown = true;

	if (button == GLUT_RIGHT_BUTTON && state == GLUT_UP)
		mouseRightDown = false;
}

double distance(int x1, int y1, int x2, int y2) {
	return sqrt((x1 - x2) * (x1 - x2) + (y1 - y2) * (y1 - y2));
}

void motion(int x, int y) {
	if (mouseLeftDown) {
		if (distance(P0.x + derP0.x / 4, P0.y + derP0.y / 4, x, y) < 20) {
			derP0.x = (x - P0.x) * 4;
			derP0.y = (y - P0.y) * 4;
		}

		if (distance(P1.x - derP1.x / 4, P1.y - derP1.y / 4, x, y) < 20) {
			derP1.x = (P1.x - x) * 4;
			derP1.y = (P1.y - y) * 4;
		}
	}

	glutPostRedisplay();
}

int  main(int argc, char** argv) {
	glutInit(&argc, argv);
	glutInitDisplayMode(GLUT_DOUBLE | GLUT_RGB);
	glutInitWindowSize(450, 450);
	glutInitWindowPosition(200, 200);
	glutCreateWindow("Hermite");
	init();
	glutDisplayFunc(display);
	glutReshapeFunc(myReshape);
	glutMouseFunc(mouse);
	glutMotionFunc(motion);
	glutMainLoop();
	return 0;
}