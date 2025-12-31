# Library main CMakeLists, add here dependencies for compilation

add_library(module_name STATIC
    src/Drv_Template.c
)

target_include_directories(module_name
    PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}/include
)