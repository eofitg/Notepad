Mac Terminal 编译运行 C/C++ 程序

```
/Applications/CLion.app/Contents/bin/cmake/mac/bin/cmake --build /Users/erou/CLionProjects/Algorithm/cmake-build-debug --target Algorithm -j 10
[1/2] Building CXX object CMakeFiles/Algorithm.dir/main.cpp.o
FAILED: CMakeFiles/Algorithm.dir/main.cpp.o 
/Library/Developer/CommandLineTools/usr/bin/c++   -g -std=gnu++20 -arch arm64 -isysroot /Library/Developer/CommandLineTools/SDKs/MacOSX13.3.sdk -fcolor-diagnostics -MD -MT CMakeFiles/Algorithm.dir/main.cpp.o -MF CMakeFiles/Algorithm.dir/main.cpp.o.d -o CMakeFiles/Algorithm.dir/main.cpp.o -c /Users/erou/CLionProjects/Algorithm/main.cpp
```