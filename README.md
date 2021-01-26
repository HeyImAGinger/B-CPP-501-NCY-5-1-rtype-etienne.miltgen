# R-Type-Etienne-Miltgen
> Reproduction of the famous R-Type Game

This project is a Epitech 3rd year project about redevelopping the famous multiplayer R-Type game. This project is part of the advanced C++ module.

The graphic is made with SFML, the communication protocol between the client and the server is made with an RFC that you can find in the doc folder. The technologie used for communication is Boost Asio.
Some documentation can be found in the doc folder.


## Installation

OS X & Linux:

```sh
conan remote add conan-center https://api.bintray.com/conan/conan/conan-center
conan remote add epitech-center https://api.bintray.com/conan/epitech/public-conan
conan remote add bincrafters-center https://api.bintray.com/conan/bincrafters/public-conan

mkdir -p build && cd build && conan install ../conanfileLinux.txt --build=missing && cmake .. -G "Unix Makefiles" -DCMAKE_BUILD_TYPE=Release

cd build && cmake --build . --config Release

LAUNCH SERVER
./build/r-type_server

LAUNCH CLIENT
./build/r-type_client
```

Windows:

```sh
conan remote add bincrafters https://api.bintray.com/conan/bincrafters/public-conan
conan remote add epitech-center https://api.bintray.com/conan/epitech/public-conan
conan remote add conan-center https://api.bintray.com/conan/conan/conan-center

mkdir build
cd build && conan install --build=missing -s compiler="Visual Studio" -s compiler.version=16 -s "arch=x86_64" -s "arch_build=x86_64" .. && cmake .. -G "Visual Studio 16 2019" -DCMAKE_BUILD_TYPE=Release

cd build/
cmake --build . --config Release

LAUNCH SERVER
./build/r-type_server

LAUNCH CLIENT
./build/r-type_client
```

## Usage example

You can play the game solo or with friends.

## Meta

Etienne MILTGEN – [@EtienneMiltgen](https://twitter.com/EtienneMiltgen) – etienne.miltgen@outlook.com
