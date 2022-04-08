### Demo3 说明
在Demo3中power.h和power.cc被写在了math目录下。对于这种情况,需要分别在项目根目录 Demo3 和 math 目录里各编写一个 CMakeLists.txt 文件。为了方便，我们可以先将 math 目录里的文件编译成静态库再由 main 函数调用。
* 在子目录的CMakeLists.txt中使用命令 add_library 将目录下的源文件编译成静态链接库
* 在根目录的CMakeLists.txt中使用命令 add_subdirectory 指明本项目包含一个子目录 math;使用命令 target_link_libraries 指明可执行文件 main 需要连接一个名为 power 的链接库