# CMake-argp

[![](https://img.shields.io/github/issues-raw/alehaa/CMake-argp.svg?style=flat-square)](https://github.com/alehaa/CMake-argp/issues)
[![LGPL license](http://img.shields.io/badge/license-LGPL-blue.svg?style=flat-square)](http://www.gnu.org/licenses/)

CMake module to search for argp library.



## Include into your project

To use [Findargp.cmake](cmake/Findargp.cmake), simply add this repository as git submodule into your own repository
```Shell
mkdir externals
git submodule add git://github.com/alehaa/CMake-argp.git externals/CMake-argp
```
and adding ```externals/cmake-argp/cmake``` to your ```CMAKE_MODULE_PATH```
```CMake
set(CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/externals/cmake-argp/cmake" ${CMAKE_MODULE_PATH})
```

If you don't use git or dislike submodules you can copy the [Findargp.cmake](cmake/Findargp.cmake) file into your repository. *Be careful when there are version updates of this repository!*


## Usage

As for any other ```find_package```module, simply search for argp:
```CMake
find_packe(argp)
```

This module will set `ARGP_FOUND`, if argp was found. `ARGP_LIBRARIES` and `ARGP_INCLUDE_PATH` will include the necessary data to build and link your target for using argp.


## Contribute

Anyone is welcome to contribute. Simply fork this repository, make your changes **in an own branch** and create a pull-request for your change. Please do only one change per pull-request.

You found a bug? Please fill out an issue and include any data to reproduce the bug.

#### Contributors

[Alexander Haase](https://github.com/alehaa)


## License

CMake-argp is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,but **WITHOUT ANY WARRANTY**; without even the implied warranty of **MERCHANTABILITY** or **FITNESS FOR A PARTICULAR PURPOSE**. See the GNU General Public License for more details. A Copy of the GPL can be found in the [LICENSE](LICENSE) file.

Copyright (c) 2016 Alexander Haase
