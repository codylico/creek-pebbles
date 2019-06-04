# Creek Pebbles: parts of a physics engine implementation

The Creek Pebbles repository aims to provide a working implementation of
a physics engine. The parts of the implementation, to be provided in both
C and C++, should be more or less usable independently of each other.

## Goals

This repository is currently empty. Goals for this repository include

* collision filters

* Verlet integration and/or implicit Euler integration

* dynamic addition and removal of items from the structure (whichever
  structure that is)

* proper and efficient support of physical stacking of items

* fluid simulation (likely by Smooth Particle Hydrodynamics techniques)

* allowing constrained objects to awake and sleep as needed

* simple and straightforward interface and implementation

* static culling

* allow objects to switch from static to dynamic (and between awake and asleep)

* construction of optimized static object storage and simpler dynamic
  object storage

* per-object continuous collision detection flag

* serialization of objects

* easy tie-in with entity component systems

## Build and Installation

This project will use the CMake build system, for easier cross-platform
development. CMake can be found at the following URL:

[https://cmake.org/download/](https://cmake.org/download/)

To use CMake with this project, a user would
first make a diretory to hold the build results.
Then, the user would run CMake in the directory with a path to the source code.
On UNIX, the commands would look like the following:
```
mkdir build
cd build
cmake ../creek-pebbles/src
```

Running CMake should then create a build project, which could then
be processed using other
tools. Usually, the tool would be Makefile or a IDE project.
For Makefiles, the following command would build the project:
```
make
```
For IDE projects, the IDE would have to be installed and ready to use.
The user woudl open the project within the IDE instead of working with the
project from the command line.

## License

The source code within this project will be provided under the MIT license.
