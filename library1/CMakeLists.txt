
add_library(library1_api INTERFACE
        )
target_include_directories(library1_api
        INTERFACE
        inc/
        )

add_library(library1
        src/class_a.cpp
        )
target_link_libraries(library1
        library1_api
        )
