# Library main CMakeLists, add here dependencies for compilation

add_library(module_name STATIC
    src/Drv_Template.c
)

target_link_libraries(module_name
    PUBLIC
        include
)