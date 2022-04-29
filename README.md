# Learn-OpenGL
learn OpenGL
# <a href="https://blog.csdn.net/MR1269427885/article/details/53283257">windows 64位 VS2015-2019 “模块计算机类型“x64”与目标计算机类型“X86”冲突解决方案</a>
# <a href="https://blog.csdn.net/m0_37876745/article/details/78174057">ERROR LNK2019：无法解析的外部的符号 _sscanf或者_vsprintf</a>
# <a href="https://www.cnblogs.com/kuliuheng/p/3397796.html">Visual Studio error C2001:常量中有换行符（解决办法）</a>
# <a href="https://blog.csdn.net/MASILEJFOAISEGJIAE/article/details/105712761">错误解决：error C2447: “{”: 缺少函数标题(是否是老式的形式表?)</a>
# <a href="https://blog.csdn.net/LYJ_viviani/article/details/51487877">解决“错误 D8016 “/ZI”和“/Gy-”命令行选项不兼容 ”问题</a>
# <a href="http://www.suchone.com/post/51.html">C++ std::cout在cmd输出中文乱码的解决方案</a>
# <a href="https://www.cxyzjd.com/article/weixin_33750452/86197676">VS2010中使用QtOpenGL出现 unresolved external symbol __imp__glClear@4 referenced in function之类的错误.</>
# <a href="https://blog.csdn.net/Septembre_/article/details/111320427">Visual Studio 2019 安装 Windows SDK 8.1</a>
# <a href="http://www.devacg.com/?post=1019">编译GLTools源码</a>
# <a href="https://www.jianshu.com/p/991d64d0205a">Visual Studio中使用NuGet设置OpenGL（nupengl有网络情况下）</a>
# <a href="https://blog.csdn.net/qq_41498261/article/details/109331819">VS2019+OpenGL配置</a>
# 注意以上教程中并没有glut64.dll 和glut64.lib的下载方法，需要从下面地址中下载，改名后将glut64.dll复制到systemwow64 和system32目录下面，将glut64.lib复杂到自己创建的libs目录下面
# <a href="https://blog.csdn.net/rhneqq/article/details/80935148">OpenGL配置glut64位和glut32位</a>
# <a href="https://www.cnblogs.com/liangliangh/p/3765221.html">OpenGL的学习资源</a>

OpenGL实用开源代码列表 转载
wx61139437dd0172021-08-14 10:57:07博主文章分类：视频综合
文章标签librarydocumentationgeneratorfilesystemsinstaller文章分类Java编程语言阅读数100

有了网络的最大好处就是可以资源共享。网络是最大的知识库，也是最好的老师，正所谓“没有你想不到的，只有你找不到的”。以下是我收集的以游戏编程，OpenGL 3D编程相关的免费扩展库资料。不断更新中，如果你有好的建义，也请把函数库名及大概功能写上，本人负责收集整理。免费共享

SDL

在3D的世界里，SDL可真所胃是大名顶顶，正所谓“为人不知陈近南，自称英雄也枉然”，因此呢，如果你是做OpenGL开发的，一定要认识一下SDL。我们都知道，在windows系统中，有一个DirectX是游戏开发商的首选的开发包，其背后只支持的Direct3D作为三维图形接口。而SDL就被认为是非window系统中的DirectX，而且是开源的。SDL所使用的3D图形接口是OpenGL。但除了图形之外，它还支持对声音、键盘、鼠标、操纵杆、2D图像等等的底层处理。现在已有不少游戏使用这个开发包进行开发。

SDL是跨平台的，目前支持的系统有：Linux, Windows, Windows CE, BeOS, MacOS, Mac OS X, FreeBSD, NetBSD, OpenBSD, BSD/OS, Solaris, IRIX, and QNX

SDL 是用C语言写的，但是能很好地兼容C++语言。并且能被其它语言绑定使用，如： Ada, C#, Eiffel, Erlang, Euphoria, Guile, Haskell, Java, Lisp, Lua, ML, Objective C, Pascal, Perl, PHP, Pike, Pliant, Python, Ruby, and Smalltalk.

SDL发布支持GNU LGPL v2.0许可协议。也就是说SDL可以免费用于商业应用。

 http://www.libsdl.org/index.php

 

glew(OpenGL Extension Wrangler Library )

GLEW是一个跨平台的C++扩展库，基于OpenGL图形接口。使用OpenGL的朋友都知道，window目前只支持OpenGL1.1的涵数，但OpenGL现在都发展到2.0以上了，要使用这些OpenGL的高级特性，就必须下载最新的扩展，另外，不同的显卡公司，也会发布一些只有自家显卡才支持的扩展函数，你要想用这数涵数，不得不去寻找最新的glext.h,有了GLEW扩展库，你就再也不用为找不到函数的接口而烦恼，因为GLEW能自动识别你的平台所支持的全部OpenGL高级扩展涵数。也就是说，只要包含一个glew.h头文件，你就能使用gl,glu,glext,wgl,glx的全部函数。GLEW支持目前流行的各种操作系统（including Windows, Linux, Mac OS X, FreeBSD, Irix, and Solaris）。

下载： http://glew.sourceforge.net/

 ShaderGen 提供简单的UI接口让你可以产生固定管线(Fixed Pipeline)的Shader.如果你对Shader不熟悉的话,这是一个不错的入门工具.详细网址如下:
 http://developer.3dlabs.com/downloads/shadergen/

 

 NVSG

The NVIDIA Scene Graph Software Development Kit (NVSGSDK) is an object-oriented programming library for creating scenegraph-based applications. The NVSGSDK provides a comprehensive set of classes that developers can easily combine and extend to create fast and reliable graphics applications.

 

 CG_GL

CG_GL is OpenGL API-based open source engine for creating 3D effects. The new release adds depth-of-field with lens blur, and motion blur using shaders. Older version of the engine work on GeForce4 and support full screen blur, transparent object distortion, and glow. Engine is available here:  http://tweety3d.no-ip.org. There are also other 3D related programs.

 OpenSteer for AI. [MIT license]

 Fluid Studios provides a memory manager, matrix class, font generator, radiosity processor, and various other things.

 Panda3D (Game/graphics lib, released by Disney after being used for Toontown Online)

 math3d++provides the normal matrix, vector and quaternion classes, and their associated operations.

 BMF_Font bitmap font library (and font texture generator)

 OpenSceneGraph - 3D engine.

 Demeter Terrain Engine [LGPL]

  OGLWFW （OpenGL Window Framework）  and basically does what it says on the tin, acts as a framework to create OpenGL windows. here

  ARToolKit An augmented reality toolkit, works really nice and very fun to play with. Documentation is still in the works though so you will have to do with the examples.

 MXRToolKit I haven't used this one but it appears to offer about the same as ARToolKit except it comes with documentation.

 MathGL++  MathGL++ is a class library for fast C++ maths for use in OpenGL C++ projects. Easy to use and similar to the OpenGL API. Matricies, Vectors, Quaternions, Linear polynomials with eigen systems are all going to be included.

 ManagedGL - The cross-platform .NET game library. Development ManagedGL 1 is stalled in faviour of ManagedGL 2. Currently mostly 2D graphics.

 LibUFO GUI library (for OpenGL) [LGPL] 一个基于OpenGL的界面库

 Crazy Eddie's GUI (another GUI lib)另一个比较有名气的游戏界面库，被OGRE游戏引擎收录使用。

 HGEis a greate library for creating hardware accelerated 2D games for windows that is free for freeware games.

 Novodex under physics libraries, free for non-commercial use.一个物理引擎，现在被收购了，改名为： PhysX

 Pixel Toaster
 http://www.pixeltoaster.com/
Open source c++ library for realtime software rendering.
It gives you a truecolor or floating point framebuffer at your choice, then converts the pixels to the display on the fly. Keyboard and mouse input, and a high resolution timer are also provided.
Currently supports only Windows (DirectX9), but ports to MacOS X and Unix (XWindows etc) are underway.

 PTK . PTK is a great Mac/Windows 2d library running on top of OpenGL (so it's fast). It's free for freeware but it does have a PTK Watermark in the corner

 MMXRand Almost twice as fast as the original Wagner's C++ code using Pentium MMX instruction by Matthew Bellew:
 Tao Framework - .Net libraries for Cg, DevIL, FreeGLUT, ODE, OpenAL, OpenGL, and SDL.
 OPAL - Open Physics Abstraction Layer, currently wraps just ODE I think but could be adapted to use other libraries. Choice of BSD or LGPL license.
 Blitz++ (math library for C++)

 

 PortAudio does cross-platform audio output and input using callbacks.

 

 GLFTFont - zlib license
Not exactly a library, but a simple class that bridges   freetype and OpenGL allowing drawing of truetype fonts in OpenGL. It's functionality is requested often enough I figured I'd release it

 

 Object-Oriented Input System (OIS)
OIS is a library for cross-platform input management. It is under the zlib/libpng license. The library supports keyboard, mouse, and joystick/gamepad input. Action mapping is included in one of the demos, and force feedback is planned for the 0.4.0 release (currently in development).

 

 libMikMod is a audio module player and library supporting many formats, includingmod, s3m, it, and xm. Originally a player for MS-DOS, MikMod has been ported to other platforms, such as Unix, Macintosh, BeOS, and Java. libMikMod falls under the LGPL agreement.

 

 GLM - a Math Library for OpenGL

 

http://members.tripod.com/markus_ilmola

This library contains useful math functions that are needed when

programming with OpenGL. Mostly vector and matrix math.

 

 GIMPACT : Collision detection library.
http://gimpact.sourceforge.net/

 


============================================
目录
General purpose libraries
3D Graphics
2D Graphics
Video
Image and Font Handling
Sound + Music
Networking
Model Handling and Character Animation (3D)
Filesystems, persistence, and format parsing
Scripting Languages
Artificial Intelligence
Mathematics, Physics and Collision Detection
Debugging, memory checks, general purpose, etc
Other Tools
 

General purpose libraries
 AgateLib (.NET library)

( MPL)

 Alchemist's Game Library (2D game engine)

(Free for non-commercial use)

 Allegro

( giftware)

 Amaltheia (game programming API)

 LGPL

 Basic Game Library (Docs in Spanish?)

 Creative Commons

 DXGame (Visual Basic 6, 2D game engine/toolkit)

("100% free to use"), but check for details

 IKA (generic gaming engine)

( 'free')

 ClanLib

 LGPL

 CRM32Pro multimedia SDK

(free, with sub-libraries under   LGPL etc)

 Devlib

 LGPL

 Game Incubator

 free

 GLFW

 ZLIB

 Goblin 2D+ Engine

(free for noncommercial, commercial licenses available for purchase)

 Golden T Game Engine (Java)

(free to use, but requires credit)

 KJAPI

(free for non commercial projects)

 MASI-CiX 2D sprite-based game platform

(free for noncommercial,   negotiate for commercial)

 PLIB General purpose library.

 LGPL

 Popcap 2D library with extras.

( Popcap license)

 Proyecto dx_lib32 Spanish language. VB6.

Free

 PTK

(free for freeware, commercial license otherwise)

 Realmforge (in C#)

 LGPL

 SDL

 LGPL

 SDL.NET

 LGPL

 SxDL 2D and 3D.

 GPL

 The Tao Framework (various libs ported to .Net)

(various/ MIT)

3D Graphics
 Amanith (vector graphics)

( QPL)

 Antiryad GX

(various licenses depending on chosen usage, but free for freeware)

 Apocalyx

 GPL

 ARToolkit

 GPL (or commercial)

 Axiom (OGRE in C#)

 LGPL

 CG

(free)

 Crystal Space

 LGPL

 Cube

(slightly modified zlib)

 Delta3D

 LGPL

 Demeter terrain engine

 LGPL

 ExNihilo

(unknown)

 Fly3D

 GPL

 FTGL (fonts in OpenGL)

 LGPL

 G3D

 BSD

 Genesis3D

( similar to GPL)

 Ghost (glut-like)

(Dual license - BL and   GPL

 GLee

 BSD-like

 Graphics Library Helper (like GLU)

(freeware)

 Heretic/Hexen

(free for non-profit use)

 Interactive Visualisation Framework

 LGPL

 Irrlicht

 ZLIB

 LightFeather

 ZLIB

 MXR Toolkit

 GPL

 The Nebula Device

( free license)

 NeoEngine

( MPL)

 NGL (glut-like framework)

 LGPL

 NVIDIA Scene Graph SDK

(free to use)

 OGRE 3D

 LGPL

 OpenGlean

 MIT

 OpenGlut

 MIT

 FreeGlut

 MIT

 OpenGL Window Framework

 ZLIB

 OpenSceneGraph

( OpenSceneGraph licence, like LGPL)

 OpenSG

 LGPL

 Panda 3D

( free)

 Qhull

(free?)

 QuakeForge

 GPL

 XEngine

 ZLIB

 Yake

( LGPL, custom licenses)

2D Graphics
 AntTweakBar (GUI for DX/OGL)

 ZLIB

 Crazy Eddie's GUI System

 LGPL

 Eclipse

 LGPL

 Endogine sprite engine (C#)

("no restrictions on the use")

 GameVision SDK

(unknown license)

 HGE

( free for non-commercial, otherwise pay)

hxrender -docs here

 ZLIB

 Kyra   LGPL

 

 ManagedGL (C#/.NET/SDL)

 LGPL

 ParaGUI (for SDL)

 LGPL

 Saq2D (C#)

"free to use for personal/commercial use"

 TinyPTC (open source)

 

 LibUFO (gui, for OpenGL etc)

 LGPL

 zEngine

 BSD

Video
 Dirac

( MPL)

 FFmpeg

(open source)

 Theora

( 'BSD-like')

 XviD

 GPL

Image and Font Handling
 BFont

 LGPL

 BMF_font (bitmap fonts in OpenGL)

 LGPL

 CImg

( CeCill license)

 Corona

 ZLIB

 CxImage

 ZLIB

 DevIL

 LGPL

 FreeImage

( GPL,   FIPL)

 GFL SDK

(free for non-commercial use)

 GLFT_Font

 ZLIB

 GTL (Game Texture Loader)

 ZLIB

 IJG (jpeg library)

(free?)

 ImageMagick

(apache-style license)

 libPNG

( libPNG license)

 libTiff

(free?)

 Paintlib

(free, must give credit)

 SDL_image

 LGPL

 SFont

(choose  LGPL or GPL)

 Titan

 ZLIB

Sound + Music
 Audiere

 LGPL

 BASS

(Free for freeware projects, otherwise commercial)

 FMOD

(Free for freeware projects, otherwise commercial)

 Hekkus Sound System

(For WinCE/Win32/Symbian and .NET.) (Free use, but credit or donation required.)

 libMikMod

 LGPL

 libsndfile

 LGPL

 Ogg Vorbis

 BSD-like

 OpenAL

(?)

 PortAudio

 essentially free

 SDL_mixer (requires SDL)

 LGPL

 SDL_sound (requires SDL)

 LGPL

Networking
Low level
 Dyconnect

 ZLIB

 Enet

 free use

 HawkNL

 LGPL

 libCURL (URL transfer)

 Curl license

 SDL_net

 LGPL

 Lidgren.Library.Network (.NET/C#)

Unspecified license - contact author

High-level
 Nevrax/NEL

(GPL?)

 Net2

 LGPL

 OpenPlay

( Apple Public Source License)

 OpenTNL

 GPL , or commercial

 RakNet

 GPL , or free by application

 ReplicaNet

Free for freeware, otherwise commercial

 Zoidcom

Free for noncommercial, otherwise contact author

Unknown
 Game Network Engine

 LGPL

Model Handling and Character Animation (3D)
 Animadead

 LGPL

 Cal3D

 LGPL

 GPUMesh

(free)

 GNU Triangulated Surface Library

 LGPL

 LibASE

 LGPL

 lib3DS

 LGPL

Filesystems, persistence, and format parsing
 bzip2

(free)

 Crypto++

free, but note possible crypto. legal issues

 ezXML

 MIT

 libXML

 MIT

 LZMA (7-Zip compression)

 LGPL or   CPL

 LZO

 GPL

 PhysFS

 zlib

 SDL_Config

 LGPL

 SQLite

(public domain)

 TinyXML

 zlib

 Unrarlib

free for non-commercial, otherwise   GPL

 ZipArchive

 GPL , or pay for commercial license

 zipstream, bzip2stream (iostream wrappers for the zlib and bzip2 libraries)

 ZLIB

 zlib

 ZLIB

 zziplib

 LGPL / MPL

Scripting Languages
 AngelScript

 ZLIB

 BOO (Reqs .NET/CLI)

MIT/BSD style

 CInt (C interpreter)

 free, reg. required for commercial use

 EosScript

 LGPL

 GameMonkey

 MIT

 GS9

'free' for any use

 Guile

 Modified GPL - almost LGPL

 IO

 BSD

 Javascript

(presumably  Mozilla license)

 Lua

 MIT

 Perl

 Artistic license

 Tcl

 free

 Python

 free

 Ruby

 Ruby license

 Small

 ZLIB

 Squirrel

 ZLIB

 VBScript

 'license at no charge'

Artificial Intelligence
 FEAR

 GPL , other

 OpenSteer

 MIT

 PathLib

(old, mainly Czech)

Mathematics, Physics and Collision Detection
Mathematics
 Blitz++

 GPL or   Blitz Artistic License)

 GLM (OpenGL helpers)

free?

 Math3D++ (vectors, quaternions)

free?

 MathGL++ (Matrices, Vectors, Quaternions, Linear polynomials with eigen systems)

 LGPL

 Mersenne Twister random number generator

free

 VMath (NxM matrix template class)

free

Physics
 Flatland (2D physics)

 BSD

 Newton Game Dynamics

Free, but must notify creators

 Novodex

free for noncommercial, contact for commercial

 Open Dynamics Engine (ODE)

 BSD

 Open Dynamics Framework

free for both commercial and non-commercial use

 OPAL

 BSD or   LGPL - please check

 Physical

(free)

 Plane2D (for ODE)

presumably  BSD also

 Tokamak

free

 True Axis

free for non-commercial use

Collision detection:
 ColDet

 LGPL

 GImpact

 LGPL / BSD-like

 Opcode

free usage

 Rapid

free for non-commercial use

 Solid

 LGPL

 V-Collide

free for non-commercial use

Debugging, memory checks, general purpose, etc
 Boost (C++ smart pointers, parsers, random numbers, quaternions, and more)

 Boost license

 Chattering Pixels libraries (memory, I/O, sorting, timers)

Free for noncommercial use,   shareware and  commercial licenses also available

 ElectricFence

 GPL

 Fluid Studios Logger

free

 Hans Boehm garbage collector for C++

free use, no warranty

 The Image Debugger (Win32 image output)

free

 IProf('A portable industrial-strength interactive profiler for C++ and C.')

public domain

 LeakTracer

Public domain

 MMGR (memory manager/checker)

free

 OIS (Object-oriented Input System)

 ZLIB

 Valgrind (Linux debugging and profiling tool)

 GPL

Other Tools
 Doxygen (documentation generator)

 GPL

 InnoSetup (installer)

free

 NaturalDocs (documentation generator) (Requires Perl 5.05.)

Free

 NSIS (installer)

free

 Synopsis (documentation generator)

free

 UPX (executable packer)

free

 boost
 loki
 open gl win frame
 gen library
 AI lib
 game graphics lib
 same as previous
 math 3D lib
 3D engine
 terain engine
 reality toolkit
 another as previous
 math gl
 gui lib
 croll platform 2D text
 harware acc
 phisics
 phisics again
 realtime rendering
 unti testing
 2d lib
 3d font lib
 math lib
 font lib
 compresion lib
 image loading
 tif image loading
 VR
 triagulae surface lib
 tokamak phisics
 random numbers
 glh lib
 Cg
 ogre .net
hex render
 SDL collide
 compresion lib
 java game engine
 FBX SDK
 zip handler
 3D Editor anfd BSP Compiler

 
