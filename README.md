# hello-ns3

This is a sample project showing how to use a self-compiled version of ns3 together with CMake. Using CMake makes a lot of sense, because the most popular C++ code editors (i.e. CLion or VSCode) can easily configure themselves using a CMakeLists-file, which leads to a hassle-free configuration of auto completion/intellisense for your favourite editor :-)

# How to use

1. Make sure you have a recent version of CMake installed and successfully built ns3 ([Building ns-3](https://www.nsnam.org/docs/release/3.29/tutorial/html/getting-started.html#building-ns-3)).
2. Clone this repository
3. Change the NS3BUILDDIR variable at the beginning of the file `CMakeLists.txt` inside the project's root directory. Example:
```
set(NS3BUILDDIR /home/marco/build/ns3/ns-3.29/build)
```
4. In case you want to use VSCode, install the extension `CMake Tools`:
```
ext install vector-of-bool.cmake-tools
```
5. Restart VSCode and open the project directory. If asked whether you want to generate a `c_cpp_properties.json` file, choose Yes.

# License

The sample code in `hello-ns3.cc` was directly taken from the official ns3 sources and is thus GPLv2-licensed. Feel free to use the rest of this repository however you like ([CC0](http://creativecommons.org/publicdomain/zero/1.0/)).