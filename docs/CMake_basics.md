# CMake Basics

The point of this assignment is to prove that you are able to piece all the missing pieces of information together to create a working barebones CMake project.

Therefore this file will mostly consist of useful notes and links to get you started on this assignment.

## Why CMake
- You want to avoid hard-coding paths
- You need to build a package on more than one computer
- You want to use CI (continuous integration)
- You need to support different OSs (maybe even just flavors of Unix)
- You want to support multiple compilers
- You want to use an IDE, but maybe not all of the time
- You want to describe how your program is structured logically, not flags and commands
- You want to use a library
- You want to use tools, like Clang-Tidy, to help you code
- You want to use a debugger

> See the [Modern-CMake wiki introduction page](https://cliutils.gitlab.io/modern-cmake/) for more reasons and history on CMake (and why there are so many different styles of CMake on the web)

## CMakeLists.txt
It is the script the CMake tool uses to configure your build environment. It automatically generates the required build files for your compiler and linker.

> See the [Modern-CMake Basics introduction](https://cliutils.gitlab.io/modern-cmake/chapters/basics.html) to see the general structure of a CMake project

### Variables and the Cache
> See the [Modern-CMake Variables and the Cache page](https://cliutils.gitlab.io/modern-cmake/chapters/basics/variables.html)

## Project structure
> It is recommended to use the structure as described by the [Modern-CMake structure](https://cliutils.gitlab.io/modern-cmake/chapters/basics/structure.html) page.

## Including other projects/libraries
There are three main ways to include other projects or libraries in to your CMake project:
- Using git submodule's
- Using CMake's DownloadProject module
- Using CMake's Fetch module

### Git Submodule's
> See [Modern-CMake Git submodule page](https://cliutils.gitlab.io/modern-cmake/chapters/projects/submodule.html)

### CMake's DownloadProject module
> See [Modern-CMake DownloadProject page](https://cliutils.gitlab.io/modern-cmake/chapters/projects/download.html)

### CMake's Fetch module
> See [Modern-CMake Fetch module](https://cliutils.gitlab.io/modern-cmake/chapters/projects/fetch.html)

> You can also take a look at the [CMake's original documentation](https://cmake.org/cmake/help/latest/module/FetchContent.html)