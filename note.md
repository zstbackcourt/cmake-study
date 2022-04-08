# Cmake学习笔记
## Linux下Cmake一般流程
* 编写 CMake 配置文件 CMakeLists.txt;
* 执行命令 cmake PATH 或者 ccmake PATH 生成 Makefile（ccmake 和 cmake 的区别在于前者提供了一个交互式的界面）。其中， PATH 是 CMakeLists.txt 所在的目录。
* 使用 make 命令进行编译。

## 编写CMakeLists.txt
CMakeLists.txt 的语法比较简单，由命令、注释和空格组成，其中命令是不区分大小写的。符号 # 后面的内容被认为是注释。命令由命令名称、小括号和参数组成，参数之间使用空格进行间隔。
