cmake_minimum_required(VERSION 3.0)
project(main)

# 配置编译选项
set(CMAKE_CXX_FLAGS ${CMAKE_CXX_FLAGS} -g)
# set(CMAKE_CXX_FLAGS ${CMAKE_CXX_FLAGS} -g -O2)

# 设置可执行文件最终存储的路径
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)

# 配置头文件搜索路径
include_directories({PROJECT_SOURCE_DIR}/code/include)
# include_directories({PROJECT_SOURCE_DIR}/code/include/xxx)
# include_directories({PROJECT_SOURCE_DIR}/code/include/xxx/xxxx)
include_directories({PROJECT_SOURCE_DIR}/thirdparty)

# 搜索子目录
add_subdirectory(code)