cmake_minimum_required(VERSION 3.20)

# Uses stm32cub generated toolchain
set(CMAKE_TOOLCHAIN_FILE
    ${CMAKE_SOURCE_DIR}/test_prj/cmake/gcc-arm-none-eabi.cmake
    CACHE FILEPATH "ARM GCC toolchain"
)

# set(ENV{STM32_LINKER_SCRIPT} "${CMAKE_SOURCE_DIR}/test_prj/STM32L433XX_FLASH.ld")
set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -T ${CMAKE_SOURCE_DIR}/test_prj/STM32L433XX_FLASH.ld")


project("stm32_driver_template")

add_subdirectory(test_prj)
add_subdirectory(module_name)