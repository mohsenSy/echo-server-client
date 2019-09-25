Echo Server and client
======================

This repository holds a basic echo server and client suing sockets in c, it is used
for demonstration purposes only, to build the code follow these steps:

* Install conan from [here](https://conan.io)
* Install cmake from [here](https://cmake.org)
* `mkdir build && cd build`
* `conan install ..`
* `cmake ..`
* `make`
* `bin/server`
* On a second terminal execute `bin/client`

The source code for server is found in `src/server.c` and for the client in `src/client.c`
