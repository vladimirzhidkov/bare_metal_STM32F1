# Bare metal C programming for STM32F1x

Install ARM GNU Toolchain from https://developer.arm.com/downloads/-/arm-gnu-toolchain-downloads

Install gdb server: brew install stlink

Pull and build libopencm3: git submodule update --init && make -C libopencm3

Install Cortex-Debug extension for vscode