Nuparu
======

v0.1.17.32a

Third Party dependencies and foundation libraries for Karl's graphics projects

Nuparu currently consists of:

* [jsoncpp](http://sourceforge.net/projects/jsoncpp/) 0.10.5 (OSX/Win)
* [stb_image](https://code.google.com/p/stblib/) 1.33 (OSX/Linux/Win)
* [Eigen](eigen.tuxfamily.org/) 3.2.8 (OSX/Linux/Win)
* [OpenVDB](http://www.openvdb.org/) 2.3.0 (OSX/Win)
* [TBB](https://www.threadingbuildingblocks.org/) 4.4 (OSX/Win)
* [Boost](www.boost.org) 1.55.0 (OSX/Linux/Win)
* [Embree](https://embree.github.io) 2.17.0 (OSX)
* [tinyformat](https://github.com/c42f/tinyformat) 2.0.1 (OSX/Linux/Win)
* [NanoGUI](https://github.com/wjakob/nanogui) (OSX)
* [Ptex](http://ptex.us) 2.1.28 (OSX)
* [OpenSubdiv](http://graphics.pixar.com/opensubdiv/docs/intro.html)  3.2.0 (OSX)
* [Libdill](http://libdill.org) 1.6 (OSX)

Updated:

* [GLM](http://glm.g-truc.net) 0.9.8.5 (Src)
* [GLFW](http://www.glfw.org) 3.2.1 (Mac)
* [GLEW](http://github.com/nigels-com/glew) 2.1.0 (Mac)
* [OpenEXR](http://www.openexr.com) 2.2.1 (Mac)
* [Partio](http://www.disneyanimation.com/technology/partio.html) 1.1.0 (8b6ea0d) (Mac)
* [RMSD](http://boscoh.com/code/) (Src)
* [glslUtility](https://github.com/CIS565-Fall-2012/Project0-Cuda-Checker/blob/master/HW0_MAC/src/glslUtility.cpp) 1.2 (Src)
* [Leonhard Gruenschloss's Sobol Generator](http://gruenschloss.org) (Src)

Notes:

* On OSX, all binary libraries except for TBB are statically linked
* On Windows, all binary libraries except for TBB are statically linked
* Since OSX ships with Zlib by default, Nuparu does not include Zlib for OSX
* Nuparu does not contain the entirety of Boost; instead, only a subset of Boost required for OpenVDB is included. The components of Boost included are header-only.
* OpenVDB has a slight modification in Coord.h for Windows support
* RMSD has minor modifications for C++ support
* OpenSubdiv is built with Ptex and TBB support only. Other backends, such as OpenCL, are not included.
* All binary OSX libraries are built with OSX's Clang variant (Apple LLVM 5.1 or greater) using libc++.
* All binary Windows libraries are built using /MT with Visual Studio 2013, except for OpenVDB, which is build using /MT with Visual Studio 2012. OpenVDB will be updated soon.
* All binary libraries on all platforms are built for x86-64
* Licenses for each library are included in each library's include/ directory
