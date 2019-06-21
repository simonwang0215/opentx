## OpenTX 2.2.3.1

Fork of released OpenTX 2.2.3

Fixed bugs:

- SBEC sensor [#6457](https://github.com/opentx/opentx/issues/6457)
- FrSky telemetry crc escape sequence [#6486](https://github.com/opentx/opentx/issues/6486)

### Build instructions

1.Download gcc-arm-none-eabi-4_7 and export gcc path:

*export=<PATH_TO_GCC_FOLDER>/bin:$PATH*

3.*cd build-taranis*

4.*cmake -DPCB=X7 -DGVARS=YES -DLUA=YES -DHELI=OFF -DDEBUG=OFF -DCMAKE_BUILD_TYPE=Release ../*

This builds firmwafre for X7 radio with lua and noheli options

5.*make firmware*

6.*make flash* (this flashes also the bootloader. To flash the firmware only, copy to sdcard folder and update from bootloader in the radio)

For detailed instructions [OpenTX build instructions](https://github.com/opentx/opentx/wiki/OpenTX-2.2-Linux-Build-Instructions)
