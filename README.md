# Stm32_Driver_Template
My own personal stm32 based driver tamplate for development.

## Requirements
- GCC Compiler + arm-none-eabi packages (https://developer.arm.com/downloads/-/arm-gnu-toolchain-downloads)
- CMake
- STM32Cube
- West
- Python
- Extension: Cortex-Debug

## Usage
- Fork this repo and rename with "STM32_DRIVERNAME_DRV"
- Launch script/vscode action for project creation, based on device
- Modify .ioc with CubeMX editor as you wish
- Modify west.yml to use additional modules

## Notes
- Remember to check .gitignore to avoid unwanted code on main repos
- Remember to check launch.json for correct device target
- Rememeber to check your arm-none-eabi toolchain is set correctly

## TODOs
- move all of ths to containerized working space to set it up exactly as this

