>环境:ubuntu20.04 

>编译器：gcc (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0

提供一份goole的cityhash源代码和编译后的静态库和头文件
```.
├── cityhash-master // 源文件,github地址：https://github.com/google/cityhash
├── opensdk // 编译后的文件
└── README.md // 介绍
```
编译用的指令：
``` shell
$ ./configure --host=i686-w64-mingw32 --prefix=/usr/local/target/opensdk --enable-static --disable-shared --with-mp4v2=no --build=i686-pc-linux
$ make all check CXXFLAGS="-g -O3"
$ sudo make install
```
