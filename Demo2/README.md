### Demo2 说明
在Demo2中 power 函数被声明在头文件中,定义在.cc 文件中,并在 main.cc 中被调用。也就是同一个目录下有多个源文件。

可以简单的在 CMakeLists.txt 中改动 add_executable, 将所有的源文件写入。但是如果源文件很多,把所有源文件的名字都加进去很繁琐。更省事的方法是使用 aux_source_directory 命令,该命令会查找指定目录下的所有源文件，然后将结果存进指定变量名。

语法:aux_source_directory$(<dir> <variable>)$
