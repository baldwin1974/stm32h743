# stm32h743
Peripheral access API for STM32H743ZI microcontroller (generated using svd2rust 0.13.1)

Documentation can be built with the following command if you git clone the repository:

    xargo/cargo doc --lib --target thumbv7em-none-eabihf

The latest version of openocd includes .cfg files for both the NUCLEO-144 board and for the STM32H7x chips. On macosx, homebrew will not install the latest version of openocd unless you direct homebrew to do so this way:

    brew install --HEAD openocd

Otherwise, using openocd 0.10.0+dev-00410 will allow you to successfully connect to the 'H743.

Please note: this file contains some "derivedFrom" errors, particularly w/r/t timers and some GPIO.
