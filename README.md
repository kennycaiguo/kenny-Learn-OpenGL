# Learn-OpenGL
learn OpenGL
# VS2022 编译 OpenGL编程指南第9版 (红宝书) 代码: https://blog.csdn.net/qq_25547755/article/details/134643272
# VS2022 编译 OpenGL超级宝典 第7版 (蓝宝书) 代码: https://blog.csdn.net/qq_25547755/article/details/134644642
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
<p align="left"><strong>SDL </strong></p> 
<p><span><span>在</span>3D<span>的世界里，</span>SDL<span>可真所胃是大名顶顶，正所谓</span>“<span>为人不知陈近南，自称英雄也枉然</span>”<span>，因此呢，如果你是做</span>OpenGL<span>开发的，一定要认识一下</span>SDL<span>。我们都知道，在</span>windows<span>系统中，有一个</span>DirectX<span>是游戏开发商的首选的开发包，其背后只支持的</span>Direct3D<span>作为三维图形接口。而</span>SDL<span>就被认为是非</span>window<span>系统中的</span>DirectX<span>，而且是开源的。</span>SDL<span>所使用的</span>3D<span>图形接口是</span>OpenGL<span>。但除了图形之外，它还支持对声音、键盘、鼠标、操纵杆、</span>2D<span>图像等等的底层处理。现在已有不少游戏使用这个开发包进行开发。</span></span></p> 
<p><span>SDL<span>是跨平台的，目前支持的系统有：</span>Linux, Windows, Windows CE, BeOS, MacOS, Mac OS X, FreeBSD, NetBSD, OpenBSD, BSD/OS, Solaris, IRIX, and QNX</span></p> 
<p><span>SDL <span>是用</span>C<span>语言写的，但是能很好地兼容</span>C++<span>语言。并且能被其它语言绑定使用，如：</span> Ada, C#, Eiffel, Erlang, Euphoria, Guile, Haskell, Java, Lisp, Lua, ML, Objective C, Pascal, Perl, PHP, Pike, Pliant, Python, Ruby, and Smalltalk. </span></p> 
<p><span>SDL<span>发布支持</span>GNU LGPL v2.0<span>许可协议。也就是说</span>SDL<span>可以免费用于商业应用。</span></span></p> 
<p><a rel="nofollow" href="http://www.libsdl.org/index.php"><span>http://www.libsdl.org/index.php</span></a></p> 
<p><strong><span> </span></strong></p> 
<p><strong><a><span>glew(OpenGL Extension Wrangler Library )</span></a></strong></p> 
<p><span>GLEW<span>是一个跨平台的</span>C++<span>扩展库，基于</span>OpenGL<span>图形接口。使用</span>OpenGL<span>的朋友都知道，</span>window<span>目前只支持</span>OpenGL1.1<span>的涵数，但</span>OpenGL<span>现在都发展到</span>2.0<span>以上了，要使用这些</span>OpenGL<span>的高级特性，就必须下载最新的扩展，另外，不同的显卡公司，也会发布一些只有自家显卡才支持的扩展函数，你要想用这数涵数，不得不去寻找最新的</span>glext.h,<span>有了</span>GLEW<span>扩展库，你就再也不用为找不到函数的接口而烦恼，因为</span>GLEW<span>能自动识别你的平台所支持的全部</span>OpenGL<span>高级扩展涵数。也就是说，只要包含一个</span>glew.h<span>头文件，你就能使用</span>gl,glu,glext,wgl,glx<span>的全部函数。</span>GLEW<span>支持目前流行的各种操作系统（</span>including Windows, Linux, Mac OS X, FreeBSD, Irix, and Solaris<span>）。</span></span></p> 
<p><span><span>下载：</span><a rel="nofollow" href="http://glew.sourceforge.net/"><span>http://glew.sourceforge.net/</span></a></span></p> 
<p><strong><a rel="nofollow" href="http://developer.3dlabs.com/downloads/shadergen/"><span>ShaderGen</span></a></strong><span><span> 提供简单的UI接口让你可以产生固定管线(Fixed Pipeline)的Shader.如果你对Shader不熟悉的话,这是一个不错的入门工具.详细网址如下</span></span><span>:<br /></span><a rel="nofollow" href="http://developer.3dlabs.com/downloads/shadergen/"><span>http://developer.3dlabs.com/downloads/shadergen/</span></a></p> 
<p><span> </span></p> 
<p align="left"><strong><a rel="nofollow" href="http://developer.nvidia.com/"><span>NVSG</span></a></strong></p> 
<p align="left"><span><span>The NVIDIA Scene Graph Software Development Kit (NVSGSDK) is an object-oriented programming library for creating scenegraph-based applications. The NVSGSDK provides a comprehensive set of classes that developers can easily combine and extend to create fast and reliable graphics applications.</span></span></p> 
<p align="left"> </p> 
<p align="left"><strong><a rel="nofollow" href="http://tweety3d.no-ip.org/">CG_GL</a></strong></p> 
<p align="left"><span>CG_GL is OpenGL API-based open source engine for creating 3D effects. The new release adds depth-of-field with lens blur, and motion blur using shaders. Older version of the engine work on GeForce4 and support full screen blur, transparent object distortion, and glow. Engine is available here: </span> <a rel="nofollow" href="http://tweety3d.no-ip.org/"><span>http://tweety3d.no-ip.org</span></a><span>. There are also other 3D related programs.</span></p> 
<p align="left"><strong><a rel="nofollow" href="http://opensteer.sourceforge.net/"><span>OpenSteer</span></a></strong><span> for AI. [MIT license]<br /><br /><strong><a rel="nofollow" href="http://www.fluidstudios.com/">Fluid Studios</a></strong> provides a memory manager, matrix class, font generator, radiosity processor, and various other things.<br /><br /><strong><a rel="nofollow" href="http://panda3d.etc.cmu.edu/">Panda3D</a></strong> (Game/graphics lib, released by Disney after being used for Toontown Online)<br /><br /></span><strong><a rel="nofollow" href="http://trenki.al.msshost.com/math3d/">math3d++</a></strong><span>provides the normal matrix, vector and quaternion classes, and their associated operations.<br /><br /></span><strong><a rel="nofollow" href="http://trenki.al.msshost.com/bmf/">BMF_Font</a></strong><span> bitmap font library (and font texture generator)<br /><br /><strong><a rel="nofollow" href="http://www.openscenegraph.org/">OpenSceneGraph</a></strong> - 3D engine.<br /><br /><strong><a rel="nofollow" href="http://www.terrainengine.com/">Demeter Terrain Engine</a></strong> [LGPL]</span></p> 
<p align="left"><strong><u><a rel="nofollow" href="http://oglwfw.sourceforge.net/"> OGLWFW</a> </u> </strong>（OpenGL Window Framework）  and basically does what it says on the tin, acts as a framework to create OpenGL windows.<a rel="nofollow" href="http://oglwfw.sourceforge.net/">here</a></p> 
<p align="left"> <strong><a rel="nofollow" href="http://artoolkit.sf.net/">ARToolKit</a></strong> An augmented reality toolkit, works really nice and very fun to play with. Documentation is still in the works though so you will have to do with the examples.<br /><br /><strong><a rel="nofollow" href="http://mxrtoolkit.sourceforge.net/">MXRToolKit</a></strong> I haven't used this one but it appears to offer about the same as ARToolKit except it comes with documentation.<br /><br /><strong><a rel="nofollow" href="http://sourceforge.net/projects/mathgl-pp/"><span>MathGL++</span></a></strong>  <span><span>MathGL++ is a class library for fast C++ maths for use in OpenGL C++ projects. Easy to use and similar to the OpenGL API. Matricies, Vectors, Quaternions, Linear polynomials with eigen systems are all going to be included.</span></span></p> 
<p align="left"><strong><a rel="nofollow" href="http://www.sf.net/projects/managedgl">ManagedGL</a></strong> - The cross-platform .NET game library. Development ManagedGL 1 is stalled in faviour of ManagedGL 2. Currently mostly 2D graphics.</p> 
<p align="left"><strong><a rel="nofollow" href="http://libufo.sourceforge.net/index.html">LibUFO</a></strong> GUI library (for OpenGL) [LGPL] 一个基于OpenGL的界面库<br /><br /><strong><a rel="nofollow" href="http://www.cegui.org.uk/modules/news/">Crazy Eddie's GUI</a></strong> (another GUI lib)另一个比较有名气的游戏界面库，被OGRE游戏引擎收录使用。</p> 
<p align="left"><a rel="nofollow" href="http://hge.relishgames.com/index.html"><strong>HGE</strong></a>is a greate library for creating hardware accelerated 2D games for windows that is free for freeware games.</p> 
<p align="left"><strong><a rel="nofollow" href="http://www.novodex.com/">Novodex</a></strong> under physics libraries, free for non-commercial use.一个物理引擎，现在被收购了，改名为：<strong><a rel="nofollow" href="http://www.physx.org/">PhysX</a></strong></p> 
<p align="left"><strong><a rel="nofollow" href="http://www.pixeltoaster.com/">Pixel Toaster</a></strong><br /><a rel="nofollow" href="http://www.pixeltoaster.com/">http://www.pixeltoaster.com/</a><br /> Open source c++ library for realtime software rendering.<br /> It gives you a truecolor or floating point framebuffer at your choice, then converts the pixels to the display on the fly. Keyboard and mouse input, and a high resolution timer are also provided.<br /> Currently supports only Windows (DirectX9), but ports to MacOS X and Unix (XWindows etc) are underway.</p> 
<p align="left"><strong><a rel="nofollow" href="http://ptk.phelios.com/">PTK</a></strong> . PTK is a great Mac/Windows 2d library running on top of OpenGL (so it's fast). It's free for freeware but it does have a PTK Watermark in the corner</p> 
<h2>
<u><a rel="nofollow" href="http://www.bellew.net/rand/MMXRand.html">MMXRand</a></u> Almost twice as fast as the original Wagner's C++ code using Pentium MMX instruction by Matthew Bellew:<br /><u><a rel="nofollow" href="http://www.taoframework.com/">Tao Framework</a></u> - .Net libraries for Cg, DevIL, FreeGLUT, ODE, OpenAL, OpenGL, and SDL.</h2> 
<h2>
<u><a rel="nofollow" href="http://opal.sourceforge.net/">OPAL</a></u> - Open Physics Abstraction Layer, currently wraps just ODE I think but could be adapted to use other libraries. Choice of BSD or LGPL license.</h2> 
<p align="left"><strong><u><a rel="nofollow" href="http://www.oonumerics.org/blitz/">Blitz++</a></u></strong> (math library for C++)</p> 
<p align="left"> </p> 
<p align="left"><strong><a rel="nofollow" href="http://www.portaudio.com/">PortAudio</a></strong> does cross-platform audio output and input using callbacks.</p> 
<p align="left"> </p> 
<p align="left"><strong><a rel="nofollow" href="http://www.cs.rit.edu/~jpt2433/glftfont">GLFTFont</a></strong> - zlib license<br /> Not exactly a library, but a simple class that bridges <a rel="nofollow" href="http://freetype.org/"> freetype</a> and OpenGL allowing drawing of truetype fonts in OpenGL. It's functionality is requested often enough I figured I'd release it</p> 
<p align="left"> </p> 
<p align="left"><strong><a rel="nofollow" href="http://www.wreckedgames.com/wiki/index.php/WreckedLibs:OIS">Object-Oriented Input System</a> (OIS)</strong><br /> OIS is a library for cross-platform input management. It is under the zlib/libpng license. The library supports keyboard, mouse, and joystick/gamepad input. Action mapping is included in one of the demos, and force feedback is planned for the 0.4.0 release (currently in development).</p> 
<p align="left"><strong> </strong></p> 
<p align="left"><strong><a rel="nofollow" href="http://mikmod.raphnet.net/">libMikMod</a></strong> is a audio module player and library supporting many formats, including<em>mod, s3m, it,</em> and <em>xm</em>. Originally a player for MS-DOS, MikMod has been ported to other platforms, such as Unix, Macintosh, BeOS, and Java. libMikMod falls under the<a rel="nofollow" href="http://www.gnu.org/copyleft/lesser.html">LGPL</a> agreement.</p> 
<p align="left"> </p> 
<p align="left"><strong><a rel="nofollow" href="http://members.tripod.com/markus_ilmola">GLM</a></strong> - a Math Library for OpenGL</p> 
<p align="left"> </p> 
<p align="left">http://members.tripod.com/markus_ilmola</p> 
<p align="left">This library contains useful math functions that are needed when </p> 
<p align="left">programming with OpenGL. Mostly vector and matrix math.</p> 
<p align="left"><strong> </strong></p> 
<p align="left"><strong><a rel="nofollow" href="http://gimpact.sourceforge.net/">GIMPACT</a></strong> : Collision detection library.<br /> http://gimpact.sourceforge.net/</p> 
<p align="left"><strong> </strong></p> 
<h2 id="h1"><a><span>General purpose libraries</span></a></h2> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://agate.sourceforge.net/wiki/index.php/Main_Page">AgateLib (.NET library)</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://www.opensource.org/licenses/mozilla1.1.php">MPL</a>)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.gamedev2d.com/">Alchemist's Game Library (2D game engine)</a></p> </td>
<td> <p>(Free for non-commercial use) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.talula.demon.co.uk/allegro/">Allegro</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://www.talula.demon.co.uk/allegro/license.html">giftware</a>)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://home.gna.org/amaltheia/">Amaltheia (game programming API)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://perso.wanadoo.es/sesses/bgl/index_en.htm">Basic Game Library</a> (Docs in Spanish?)</p> </td>
<td> <p><a rel="nofollow" href="http://creativecommons.org/licenses/by-nc-sa/2.1/es/">Creative Commons</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://dxgame.com/">DXGame (Visual Basic 6, 2D game engine/toolkit)</a></p> </td>
<td> <p>("100% free to use"), but check for details </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://ika.sourceforge.net/">IKA (generic gaming engine)</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://ika.sourceforge.net/articles.php?view=1#07">'free'</a>) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.clanlib.org/">ClanLib</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.megastormsystems.com/sdk/crm32pro_en.htm">CRM32Pro multimedia SDK</a></p> </td>
<td> <p>(free, with sub-libraries under <a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php"> LGPL</a> etc) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.devlib-central.org/">Devlib</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://gi.kamron.net/">Game Incubator</a></p> </td>
<td> <p><a rel="nofollow" href="http://gi.kamron.net/english/License.php">free</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://glfw.sourceforge.net/">GLFW</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://hoek.inkblue.net/goblin/goblin.html">Goblin 2D+ Engine</a></p> </td>
<td> <p>(free for noncommercial, commercial licenses available for purchase) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://goldenstudios.or.id/products/GTGE/">Golden T Game Engine (Java)</a></p> </td>
<td> <p>(free to use, but requires credit) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.kjapi.com/">KJAPI</a></p> </td>
<td> <p>(free for non commercial projects) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://acheron-design.net/dev/MCXSE/">MASI-CiX 2D sprite-based game platform</a></p> </td>
<td> <p>(free for noncommercial, <a rel="nofollow" href="http://acheron-design.net/dev/MCXSE/licensing.htm"> negotiate for commercial</a>) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://plib.sourceforge.net/">PLIB</a> General purpose library.</p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://developer.popcap.com/">Popcap</a> 2D library with extras.</p> </td>
<td> <p>(<a rel="nofollow" href="http://developer.popcap.com/license.php">Popcap license</a>) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://dxlib32.se32.com/">Proyecto dx_lib32</a> Spanish language. VB6.</p> </td>
<td> <p>Free</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.phelios.com/ptk/">PTK</a></p> </td>
<td> <p>(free for freeware, commercial license otherwise) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://sourceforge.net/projects/realmforge">Realmforge (in C#)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.libsdl.org/index.php"><span>SDL</span></a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://cs-sdl.sourceforge.net/index.php/Main_Page">SDL.NET</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://sxdl.sourceforge.net/">SxDL</a> 2D and 3D.</p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.mono-project.com/Tao">The Tao Framework (various libs ported to .Net)</a></p> </td>
<td> <p>(various/<a rel="nofollow" href="http://www.opensource.org/licenses/mit-license.html">MIT</a>)</p> </td>
</tr></tbody></table><h2 id="h2"><a><span>3D Graphics</span></a></h2> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://www.amanith.org/">Amanith (vector graphics)</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://www.amanith.org/include/qpl.php">QPL</a>)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.arkham-development.com/">Antiryad GX</a></p> </td>
<td> <p>(various licenses depending on chosen usage, but free for freeware) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://apocalyx.sourceforge.net/">Apocalyx</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://artoolkit.sourceforge.net/">ARToolkit</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> (or commercial)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.axiom3d.org/">Axiom (OGRE in C#)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://developer.nvidia.com/object/cg_toolkit_1_1.html">CG</a></p> </td>
<td> <p>(free) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://crystal.sourceforge.net/">Crystal Space</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.cubeengine.com/">Cube</a></p> </td>
<td> <p>(slightly modified zlib)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://delta3d.org/">Delta3D</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.terrainengine.com/">Demeter terrain engine</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.ploksoftware.org/">ExNihilo</a></p> </td>
<td> <p>(unknown) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.fly3d.com.br/">Fly3D</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://homepages.paradise.net.nz/henryj/code/index.html#FTGL">FTGL (fonts in OpenGL)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://g3d-cpp.sourceforge.net/">G3D</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.opensource.org/licenses/bsd-license.php">BSD</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.genesis3d.com/">Genesis3D</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://www.genesis3d.com/g3dlicense.txt">similar to GPL</a>) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://projects.blender.org/projects/ghost/">Ghost (glut-like)</a></p> </td>
<td> <p>(Dual license - BL and <a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php"> GPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://elf-stone.com/glee.php"><span>GLee</span></a></p> </td>
<td> <p><a rel="nofollow" href="http://elf-stone.com/downloads/GLee/readme.txt">BSD-like</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.geocities.com/vmelkon/glhlibrary.html">Graphics Library Helper (like GLU)</a></p> </td>
<td> <p>(freeware) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www2.ravensoft.com/source/">Heretic/Hexen</a></p> </td>
<td> <p>(free for non-profit use)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://gorkon.byggmek.lth.se/ivfweb/">Interactive Visualisation Framework</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://irrlicht.sourceforge.net/">Irrlicht</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://lf.mmdevel.de/news.php">LightFeather</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://mxrtoolkit.sourceforge.net/">MXR Toolkit</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.radonlabs.de/nebula.html">The Nebula Device</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://www.radonlabs.de/license.html">free license</a>)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.neoengine.org/">NeoEngine</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://www.opensource.org/licenses/mozilla1.1.php">MPL</a>)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://home.gna.org/ngl/about.html">NGL (glut-like framework)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://developer.nvidia.com/object/nvsg_home.html">NVIDIA Scene Graph SDK</a></p> </td>
<td> <p>(free to use) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.ogre3d.org/">OGRE 3D</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://openglean.sourceforge.net/">OpenGlean</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.opensource.org/licenses/mit-license.html">MIT</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://openglut.sourceforge.net/">OpenGlut</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.opensource.org/licenses/mit-license.html">MIT</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://freeglut.sourceforge.net/">FreeGlut</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.opensource.org/licenses/mit-license.html">MIT</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://oglwfw.sourceforge.net/">OpenGL Window Framework</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.openscenegraph.org/">OpenSceneGraph</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://www.openscenegraph.org/osgwiki/uploads/Legal/LICENSE.txt">OpenSceneGraph licence, like LGPL</a>)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.opensg.org/">OpenSG</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://panda3d.etc.cmu.edu/">Panda 3D</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://panda3d.etc.cmu.edu/docs/license/">free</a>) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.qhull.org/">Qhull</a></p> </td>
<td> <p>(free?) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.quakeforge.net/">QuakeForge</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://xengine.sourceforge.net/">XEngine</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.yake.org/">Yake</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.html">LGPL</a>, custom licenses)</p> </td>
</tr></tbody></table><h2 id="h3"><a><span>2D Graphics</span></a></h2> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://www.antisphere.com/Wiki/doku.php?id=tools:anttweakbar">AntTweakBar (GUI for DX/OGL)</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.cegui.org.uk/modules/news/">Crazy Eddie's GUI System</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://eclipseeng.sourceforge.net/">Eclipse</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://codeproject.com/csharp/Endogine.asp">Endogine sprite engine (C#)</a></p> </td>
<td> <p>("no restrictions on the use") </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.bigdaddygames.com/index.php?option=com_docman&amp;task=doc_details&amp;gid=2&amp;Itemid=41">GameVision SDK</a></p> </td>
<td> <p>(unknown license) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://hge.relishgames.com/index.html">HGE</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://hge.relishgames.com/license.html">free</a> for non-commercial, otherwise<a rel="nofollow" href="http://hge.relishgames.com/purchase.html">pay</a>) </p> </td>
</tr><tr><td> <p>hxrender -docs here</p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.grinninglizard.com/kyra/">Kyra</a> <a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php"> LGPL</a> </p> </td>
<td> <p><span> </span></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://sourceforge.net/projects/managedgl">ManagedGL (C#/.NET/SDL)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.paragui.org/">ParaGUI (for SDL)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://saqscrap.com/saq2d.aspx">Saq2D</a> (C#) </p> </td>
<td> <p>"free to use for personal/commercial use"</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.gaffer.org/tinyptc/">TinyPTC</a> (open source) </p> </td>
<td> <p><span> </span></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://libufo.sourceforge.net/index.html">LibUFO (gui, for OpenGL etc)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://zengine.sourceforge.net/index.php">zEngine</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.opensource.org/licenses/bsd-license.php">BSD</a> </p> </td>
</tr></tbody></table><h2 id="h4"><a><span>Video</span></a></h2> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://sourceforge.net/projects/dirac">Dirac</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://www.opensource.org/licenses/mozilla1.1.php">MPL</a>) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://ffmpeg.sourceforge.net/">FFmpeg</a></p> </td>
<td> <p>(open source) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.theora.org/">Theora</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://www.opensource.org/licenses/bsd-license.php">'BSD-like'</a>) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.xvid.org/">XviD</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> </p> </td>
</tr></tbody></table><h2 id="h5"><a><span>Image and Font Handling</span></a></h2> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://www.cs.unibo.it/~dbilli/bfont/bfont.html">BFont</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://trenki.gippsbiz.com/bmf/">BMF_font (bitmap fonts in OpenGL)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://cimg.sourceforge.net/">CImg</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://www.cecill.info/licences/Licence_CeCILL_V1.1-US.html">CeCill</a> license)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://corona.sourceforge.net/">Corona</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.xdp.it/cximage.htm">CxImage</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://openil.sourceforge.net/">DevIL</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://freeimage.sourceforge.net/">FreeImage</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a>, <a rel="nofollow" href="http://freeimage.sourceforge.net/freeimage-license.txt"> FIPL</a>) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://perso.wanadoo.fr/pierre.g/xnview/engfl.html">GFL SDK</a></p> </td>
<td> <p>(free for non-commercial use) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.cs.rit.edu/~jpt2433/glftfont/">GLFT_Font</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://tgtl.sourceforge.net/">GTL (Game Texture Loader)</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.ijg.org/">IJG (jpeg library)</a></p> </td>
<td> <p>(free?) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.imagemagick.org/">ImageMagick</a></p> </td>
<td> <p>(apache-style license) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.libpng.org/pub/png/libpng.html">libPNG</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://www.libpng.org/pub/png/src/libpng-LICENSE.txt">libPNG</a> license)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.remotesensing.org/libtiff/">libTiff</a></p> </td>
<td> <p>(free?) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.paintlib.de/paintlib/">Paintlib</a></p> </td>
<td> <p>(free, must give credit) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.libsdl.org/projects/SDL_image/">SDL_image</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.linux-games.com/sfont/">SFont</a></p> </td>
<td> <p>(choose <a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.html">LGPL</a> or<a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a>) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://titan.sourceforge.net/">Titan</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a> </p> </td>
</tr></tbody></table><h2 id="h6"><a><span>Sound +</span> Music</a></h2> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://audiere.sourceforge.net/">Audiere</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.un4seen.com/">BASS</a></p> </td>
<td> <p>(Free for freeware projects, otherwise commercial)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.fmod.org/">FMOD</a></p> </td>
<td> <p>(Free for freeware projects, otherwise commercial)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.shlzero.com/">Hekkus Sound System</a></p> </td>
<td> <p>(For WinCE/Win32/Symbian and .NET.) (Free use, but credit or donation required.)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://mikmod.raphnet.net/">libMikMod</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.mega-nerd.com/libsndfile/">libsndfile</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.vorbis.com/">Ogg Vorbis</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.xiph.org/licenses/bsd/">BSD-like</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.openal.org/">OpenAL</a></p> </td>
<td> <p>(?) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.portaudio.com/">PortAudio</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.portaudio.com/license.html">essentially free</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://jcatki.no-ip.org/SDL_mixer/">SDL_mixer (requires SDL)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://icculus.org/SDL_sound/">SDL_sound (requires SDL)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr></tbody></table><h2 id="h7"><a><span>Networking</span></a></h2> 
<h3 id="h8"><span>Low level</span></h3> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://www.junction.bafsoft.com/#dyconnect">Dyconnect</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://enet.bespin.org/">Enet</a></p> </td>
<td> <p><a rel="nofollow" href="http://enet.bespin.org/License.html#License">free use</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.hawksoft.com/hawknl/">HawkNL</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://curl.haxx.se/libcurl/">libCURL</a> (URL transfer)</p> </td>
<td> <p><a rel="nofollow" href="http://curl.haxx.se/docs/copyright.html">Curl license</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.libsdl.org/projects/SDL_net/">SDL_net</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.lidgren.net/wiki/doku.php?id=lidgren.library.network">Lidgren.Library.Network</a> (.NET/C#)</p> </td>
<td> <p>Unspecified license - contact author</p> </td>
</tr></tbody></table><h3 id="h9"><span>High-level</span></h3> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://www.nevrax.org/">Nevrax/NEL</a></p> </td>
<td> <p>(GPL?)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.gameprogrammer.com/net2/net2-1.html">Net2</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://developer.apple.com/darwin/projects/openplay/">OpenPlay</a></p> </td>
<td> <p>(<a rel="nofollow" href="http://www.opensource.apple.com/apsl/">Apple Public Source License</a>)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.opentnl.org/">OpenTNL</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> , or commercial</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.rakkarsoft.com/">RakNet</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> , or free by application</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.replicanet.com/">ReplicaNet</a></p> </td>
<td> <p>Free for freeware, otherwise commercial</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.zoidcom.com/">Zoidcom</a></p> </td>
<td> <p>Free for noncommercial, otherwise contact author</p> </td>
</tr></tbody></table><h3 id="h10"><span>Unknown</span></h3> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://www.rit.edu/~jpw9607/gne/">Game Network Engine</a> </p> </td></tr><tr><td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td></tr></tbody></table><h2 id="h11"><a><span>Model Handling</span> and Character Animation (3D)</a></h2> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://animadead.sourceforge.net/">Animadead</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://cal3d.sourceforge.net/">Cal3D</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://w3imagis.imag.fr/Membres/Sylvain.Lefebvre/GPUmesh/">GPUMesh</a></p> </td>
<td> <p>(free) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://gts.sourceforge.net/">GNU Triangulated Surface Library</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://interreality.org/wwwvos/projects/libase">LibASE</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://lib3ds.sourceforge.net/">lib3DS</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr></tbody></table><h2 id="h12"><a><span>Filesystems, persistence</span>, and format parsing</a></h2> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://sources.redhat.com/bzip2/">bzip2</a></p> </td>
<td> <p>(free) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.eskimo.com/~weidai/cryptlib.html">Crypto++</a></p> </td>
<td> <p>free, but note possible crypto. legal issues</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://ezxml.sourceforge.net/">ezXML</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.opensource.org/licenses/mit-license.html">MIT</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.xmlsoft.org/">libXML</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.opensource.org/licenses/mit-license.html">MIT</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.7-zip.org/sdk.html">LZMA (7-Zip compression)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> or <a rel="nofollow" href="http://www.eclipse.org/legal/cpl-v10.html"> CPL</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.oberhumer.com/opensource/lzo/">LZO</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://icculus.org/physfs/">PhysFS</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.angelcode.com/angelscript/license.asp">zlib</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://student.agh.edu.pl/~koshmaar/SDL_Config/news.php">SDL_Config</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.sqlite.org/">SQLite</a></p> </td>
<td> <p>(public domain)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://sourceforge.net/projects/tinyxml">TinyXML</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.angelcode.com/angelscript/license.asp">zlib</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.unrarlib.org/">Unrarlib</a></p> </td>
<td> <p>free for non-commercial, otherwise <a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php"> GPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.artpol-software.com/index_zip.html">ZipArchive</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> , or pay for commercial license</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.codeproject.com/vcpp/stl/zipstream.asp">zipstream, bzip2stream</a> (iostream wrappers for the zlib and bzip2 libraries)</p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/">zlib</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/">zziplib</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> /<a rel="nofollow" href="http://www.opensource.org/licenses/mozilla1.1.php">MPL</a></p> </td>
</tr></tbody></table><h2 id="h13"><a><span>Scripting Languages</span></a></h2> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://www.angelcode.com/angelscript/">AngelScript</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://boo.codehaus.org/">BOO</a> (Reqs .NET/CLI)</p> </td>
<td> <p>MIT/BSD style</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://root.cern.ch/root/Cint.html">CInt (C interpreter)</a></p> </td>
<td> <p><a rel="nofollow" href="http://root.cern.ch/root/Cint.phtml?readme">free, reg. required for commercial use</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://eosscript.sourceforge.net/">EosScript</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.somedude.net/gamemonkey/">GameMonkey</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.opensource.org/licenses/mit-license.html">MIT</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.simion.co.uk/gs9/">GS9</a></p> </td>
<td> <p>'free' for any use</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.gnu.org/software/guile/guile.html">Guile</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gnu.org/software/guile/docs/guile-ref/Guile-License.html#Guile%20License">Modified GPL - almost LGPL</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.iolanguage.com/">IO</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.opensource.org/licenses/bsd-license.php">BSD</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.mozilla.org/js/">Javascript</a></p> </td>
<td> <p>(presumably <a rel="nofollow" href="http://www.opensource.org/licenses/mozilla1.0.php">Mozilla license</a>)</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.lua.org/">Lua</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.lua.org/license.html#5">MIT</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.perl.com/">Perl</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.perl.com/language/misc/Artistic.html">Artistic</a> license</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://tcl.sourceforge.net/">Tcl</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.tcl.tk/software/tcltk/license_terms.html">free</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.python.org/">Python</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.python.org/psf/license.html">free</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.ruby-lang.org/en/">Ruby</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.ruby-lang.org/en/LICENSE.txt">Ruby license</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.compuphase.com/small.htm">Small</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://squirrel.sourceforge.net/">Squirrel</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://msdn.microsoft.com/scripting/">VBScript</a></p> </td>
<td> <p><a rel="nofollow" href="http://msdn.microsoft.com/library/default.asp?url=/library/en-us/script56/html/vbswhat.asp">'license at no charge'</a></p> </td>
</tr></tbody></table><h2 id="h14"><a><span>Artificial Intelligence</span></a></h2> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://fear.sourceforge.net/">FEAR</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> , other</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://opensteer.sourceforge.net/">OpenSteer</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.opensource.org/licenses/mit-license.html">MIT</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://pathlib.hildebrand.cz/pathlib.html">PathLib</a></p> </td>
<td> <p>(old, mainly Czech) </p> </td>
</tr></tbody></table><h2 id="h15"><a><span>Mathematics, Physics and Collision</span> Detection</a></h2> 
<h3 id="h16"><span>Mathematics</span></h3> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://www.oonumerics.org/blitz/">Blitz++</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> or <a rel="nofollow" href="http://www.oonumerics.org/blitz/legal/"> Blitz Artistic License</a>) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://members.tripod.com/markus_ilmola">GLM (OpenGL helpers)</a></p> </td>
<td> <p>free?</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://trenki.gippsbiz.com/math3d/">Math3D++ (vectors, quaternions)</a></p> </td>
<td> <p>free?</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://sourceforge.net/projects/mathgl-pp/"><span>MathGL++ (Matrices, Vectors, Quaternions, Linear polynomials with eigen systems)</span></a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www-personal.engin.umich.edu/~wagnerr/MersenneTwister.html">Mersenne Twister random number generator</a></p> </td>
<td> <p>free</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.fluidstudios.com/">VMath (NxM matrix template class)</a></p> </td>
<td> <p>free </p> </td>
</tr></tbody></table><h3 id="h17"><span>Physics</span></h3> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://flatland.sourceforge.net/">Flatland (2D physics)</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.opensource.org/licenses/bsd-license.php">BSD</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.newtondynamics.com/">Newton Game Dynamics</a></p> </td>
<td> <p>Free, but must notify creators </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.novodex.com/">Novodex</a></p> </td>
<td> <p>free for noncommercial, contact for commercial</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://ode.org/">Open Dynamics Engine (ODE)</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.opensource.org/licenses/bsd-license.php">BSD</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.physicstools.org/">Open Dynamics Framework</a></p> </td>
<td> <p>free for both commercial and non-commercial use</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://ox.slug.louisville.edu/~o0lozi01/opal_wiki/index.php/Main_Page">OPAL</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.opensource.org/licenses/bsd-license.php">BSD</a> or <a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php"> LGPL</a> - please check </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://physical.alecrivers.com/">Physical</a></p> </td>
<td> <p>(free) </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.mathematik.uni-bielefeld.de/~pserocka/ODE-Plane2D/">Plane2D (for ODE)</a></p> </td>
<td> <p>presumably <a rel="nofollow" href="http://www.opensource.org/licenses/bsd-license.php">BSD</a> also</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.tokamakphysics.com/">Tokamak</a></p> </td>
<td> <p>free</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.trueaxis.com/">True Axis</a></p> </td>
<td> <p>free for non-commercial use</p> </td>
</tr></tbody></table><h3 id="h18"><span>Collision detection:</span></h3> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://photoneffect.com/coldet/">ColDet</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://gimpact.sourceforge.net/">GImpact</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> /<a rel="nofollow" href="http://gimpact.sourceforge.net/GIMPACT-LICENSE-BSD.TXT">BSD-like</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.codercorner.com/Opcode.htm">Opcode</a></p> </td>
<td> <p>free usage</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.cs.unc.edu/~geom/OBB/OBBT.html">Rapid</a></p> </td>
<td> <p>free for non-commercial use</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.win.tue.nl/~gino/solid/index.html">Solid</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/lgpl-license.php">LGPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.cs.unc.edu/~geom/V_COLLIDE/">V-Collide</a></p> </td>
<td> <p>free for non-commercial use</p> </td>
</tr></tbody></table><h2 id="h19"><a><span>Debugging, memory checks, general</span> purpose, etc</a></h2> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://www.boost.org/"><span>Boost (C++ smart pointers, parsers, random numbers, quaternions, and more)</span></a></p> </td>
<td> <p><a rel="nofollow" href="http://www.boost.org/LICENSE_1_0.txt">Boost license</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.chatteringpixels.com/products.php">Chattering Pixels libraries (memory, I/O, sorting, timers)</a></p> </td>
<td> <p>Free for noncommercial use, <a rel="nofollow" href="http://www.chatteringpixels.com/terms-8-share.php"> shareware</a> and <a rel="nofollow" href="http://www.chatteringpixels.com/terms-8-comm.php">commercial</a> licenses also available</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.perens.com/FreeSoftware/">ElectricFence</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.fluidstudios.com/">Fluid Studios Logger</a></p> </td>
<td> <p>free </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.hpl.hp.com/personal/Hans_Boehm/gc/">Hans Boehm garbage collector for C++</a></p> </td>
<td> <p>free use, no warranty</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.cs.unc.edu/~baxter/projects/imdebug/">The Image Debugger (Win32 image output)</a></p> </td>
<td> <p>free</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://silverspaceship.com/src/iprof/">IProf('A portable industrial-strength interactive profiler for C++ and C.')</a></p> </td>
<td> <p>public domain</p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.andreasen.org/LeakTracer/">LeakTracer</a></p> </td>
<td> <p>Public domain </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.fluidstudios.com/">MMGR (memory manager/checker)</a></p> </td>
<td> <p>free </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.wreckedgames.com/wiki/index.php/WreckedLibs:OIS">OIS (Object-oriented Input System)</a></p> </td>
<td> <p><a rel="nofollow" href="http://www.gzip.org/zlib/zlib_license.html">ZLIB</a></p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://valgrind.kde.org/">Valgrind (Linux debugging and profiling tool)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> </p> </td>
</tr></tbody></table><h2 id="h20"><a><span>Other Tools</span></a></h2> 
<table border="0" cellpadding="0"><tbody><tr><td> <p><a rel="nofollow" href="http://www.stack.nl/~dimitri/doxygen/">Doxygen (documentation generator)</a></p> </td>
<td> <p><a rel="nofollow" href="http://opensource.org/licenses/gpl-license.php">GPL</a> </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.jrsoftware.org/isinfo.php">InnoSetup (installer)</a></p> </td>
<td> <p>free </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://www.naturaldocs.org/">NaturalDocs (documentation generator)</a> (Requires Perl 5.05.)</p> </td>
<td> <p>Free </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://nsis.sourceforge.net/">NSIS (installer)</a></p> </td>
<td> <p>free </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://synopsis.fresco.org/">Synopsis (documentation generator)</a></p> </td>
<td> <p>free </p> </td>
</tr><tr><td> <p><a rel="nofollow" href="http://upx.sourceforge.net/">UPX (executable packer) </a></p> </td>
<td> <p>free </p> </td>
</tr></tbody></table><p align="left"><a rel="nofollow" href="http://www.boost.org/">boost</a><br /><a rel="nofollow" href="http://sourceforge.net/projects/loki-lib/">loki</a><br /><a rel="nofollow" href="http://oglwfw.sourceforge.net/">open gl win frame</a><br /><a rel="nofollow" href="http://www.cdxlib.com/index.phptarget=">gen library</a><br /><a rel="nofollow" href="http://opensteer.sourceforge.net/">AI lib</a><br /><a rel="nofollow" href="http://panda3d.etc.cmu.edu/">game graphics lib</a><br /><a rel="nofollow" href="http://trenki.50free.org/math3d/">same as previous</a><br /><a rel="nofollow" href="http://trenki.50free.org/bmf/">math 3D lib</a><br /><a rel="nofollow" href="http://www.openscenegraph.org/">3D engine</a><br /><a rel="nofollow" href="http://www.terrainengine.com/">terain engine</a><br /><a rel="nofollow" href="http://artoolkit.sf.net/">reality toolkit</a><br /><a rel="nofollow" href="http://mxrtoolkit.sourceforge.net/">another as previous</a><br /><a rel="nofollow" href="http://sourceforge.net/projects/mathgl-pp/">math gl</a><br /><a rel="nofollow" href="http://crayzedsgui.sourceforge.net/">gui lib</a><br /><a rel="nofollow" href="http://www.sf.net/projects/managedgltarget=">croll platform 2D text</a><br /><a rel="nofollow" href="http://hge.relishgames.com/index.htmltarget=">harware acc</a><br /><a rel="nofollow" href="http://www.novodex.com/">phisics</a><br /><a rel="nofollow" href="http://www.physicstools.org/">phisics again</a><br /><a rel="nofollow" href="http://www.pixeltoaster.com/">realtime rendering</a><br /><a rel="nofollow" href="http://sourceforge.net/projects/cppunit/">unti testing</a><br /><a rel="nofollow" href="http://www.dingogames.com/">2d lib</a><br /><a rel="nofollow" href="http://trenki.al.msshost.com/">3d font lib</a><br /><a rel="nofollow" href="http://trenki.al.msshost.com/math3d/">math lib</a><br /><a rel="nofollow" href="http://trenki.al.msshost.com/bmf/">font lib</a><br /><a rel="nofollow" href="http://www.oberhumer.com/opensource/lzo/">compresion lib</a><br /><a rel="nofollow" href="http://www.ijg.org/files/">image loading </a><br /><a rel="nofollow" href="http://www.remotesensing.org/libtiff/">tif image loading</a><br /><a rel="nofollow" href="http://www.yake.org/">VR</a><br /><a rel="nofollow" href="http://gts.sourceforge.net/">triagulae surface lib</a><br /><a rel="nofollow" href="http://www.tokamakphysics.com/">tokamak phisics</a><br /><a rel="nofollow" href="http://www-personal.engin.umich.edu/~wagnerr/MersenneTwister.htmltarget=">random numbers</a><br /><a rel="nofollow" href="http://www.geocities.com/vmelkon/glhlibrary.htmltarget=">glh lib</a><br /><a rel="nofollow" href="http://www.taoframework.com/">Cg </a><br /><a rel="nofollow" href="http://www.axiom3d.org/">ogre .net</a><br /><a>hex render</a><br /><a rel="nofollow" href="http://www.libsdl.org/libraries.php?match_id=1373target=">SDL collide</a><br /><a rel="nofollow" href="http://www.7-zip.org/sdk.htmltarget=">compresion lib</a><br /><a rel="nofollow" href="http://goldenstudios.or.id/products/GTGE/">java game engine</a><br /><a rel="nofollow" href="http://www.alias.com/eng/products-services/fbx/index.shtmltarget=">FBX SDK</a><br /><a rel="nofollow" href="http://www.artpol-software.com/index_zip.htmltarget=">zip handler</a><br /><a rel="nofollow" href="http://www.zalsoft.com/">3D Editor anfd BSP Compiler</a></p>  
<br /></div></div>


 


