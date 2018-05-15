# stm32h743
Peripheral access API for STM32H743ZI microcontroller (generated using svd2rust)

Documentation can be built with the following command if you git clone the repository:

    xargo/cargo doc --lib --target thumbv7em-none-eabihf

Please note that openocd's latest version does not contain a config (.cfg) script for the ST-Nucleo-144 for STM32H743. Here is a successful (so far!) script that you can use. Place the file called openocd.cfg in your project directory and the file called stm32h7x3.cfg into the "scripts/target/" folder found within openocd's source directory. For me, that folder was found in /usr/local/Cellar/open-ocd/0.10.0/share/openocd/ - but that is because I am using a mac, and I installed openocd using homebrew.  

Once you have installed those two scripts in the two appropriate places, call openocd from that directory, as follows:

    openocd

Or, if you are not in the project directory and want to call openocd, you can just type

    openocd -f [path to openocd.cfg]

There are other ways to do this and you can peruse the two scripts as you see fit. Good luck!


