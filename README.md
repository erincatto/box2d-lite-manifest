# Box2D-Lite
Box2D-Lite is a small 2D physics engine. It was developed for the [2006 GDC Physics Tutorial](docs/GDC2006_Catto_Erin_PhysicsTutorial.pdf). This is the original version of the larger [Box2D](https://box2d.org) library. The Lite version is more suitable for learning about game physics.

# Building
- Install [CMake](https://cmake.org/)
- Ensure CMake is in the user `PATH`
- Visual Studio 2017: run `build.bat`
- Otherwise: run `build.sh` from a bash shell
- Results are in the build sub-folder

# Building in VS2022 with vcpkg
- install vcpkg: https://github.com/microsoft/vcpkg
- define environment variable: `VCPKG_ROOT` as your local *vcpkg-dir*
- define environment variable: `VCPKG_DEFAULT_TRIPLET` as `x64-windows`
- close all instances of VS 2022
- open this folder with VS 2022 (wait for CMake to finish)
- in the toolbar set the startup item to `samples.exe`
- you can now press F5 to run and debug

# Build Status
[![Build Status](https://travis-ci.org/erincatto/box2d-lite.svg?branch=master)](https://travis-ci.org/erincatto/box2d-lite)
