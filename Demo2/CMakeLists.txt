#CMake 最低版本号要求
cmake_minimum_required(VERSION 2.8)

#项目信息,项目名称
project(Demo2)

#指定生成目标
#add_executable(Demo main.cc MathFunctions.cc)

#查找当前目录下的所有源文件
#并将名称保存到DIR_SRCS变量
aux_source_directory(. DIR_SRCS)

#指定生成目标
add_executable(Demo ${DIR_SRCS})
