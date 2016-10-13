cmake_minimum_required (VERSION 2.8)
project (3.multiDirWithSours)
aux_source_directory(. DIR_SRCS)
add_executable(Demo ${DIR_SRCS})
add_subdirectory(utils)# 添加 utils 子目录
# 添加链接库
target_link_libraries(Demo hello)