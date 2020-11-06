cmake_minimum_required(VERSION 3.17)
project(clion)

set(CMAKE_CXX_STANDARD 14)


add_subdirectory(library1)


add_executable(clion
        main.cpp
        )
target_link_libraries(clion
        library1
        library1_api
        )

