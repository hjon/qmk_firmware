# kyra

![kyra](imgur.com image replace me!)

*A short description of the keyboard/project*

* Keyboard Maintainer: [Jon Hjelle](https://github.com/hjon)
* Hardware Supported: *The PCBs, controllers supported*
* Hardware Availability: *Links to where you can find this hardware*

Make example for this keyboard (after setting up your build environment):

    make kyra:default

Flashing example for this keyboard:

    make kyra:default:flash

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Bootloader

Enter the bootloader in 3 ways:

* **Bootmagic reset**: Hold down the key at (0,0) in the matrix (usually the top left key or Escape) and plug in the keyboard
* **Physical reset button**: Briefly press the button on the back of the PCB - some may have pads you must short instead
* **Keycode in layout**: Press the key mapped to `QK_BOOT` if it is available

## My Notes
- Base Layout: numpad_4x4, but I think I'll adjust to a full 4x4, not a numpad
- Dev Board: elite_c

## Notes from QMK Toolbox for ABall
* QMK Toolbox 0.3.3 (https://qmk.fm/toolbox)
* Supported bootloaders:
*  - ARM DFU (APM32, Kiibohd, STM32, STM32duino) and RISC-V DFU (GD32V) via dfu-util (http://dfu-util.sourceforge.net/)
*  - Atmel/LUFA/QMK DFU via dfu-programmer (http://dfu-programmer.github.io/)
*  - Atmel SAM-BA (Massdrop) via Massdrop Loader (https://github.com/massdrop/mdloader)
*  - BootloadHID (Atmel, PS2AVRGB) via bootloadHID (https://www.obdev.at/products/vusb/bootloadhid.html)
*  - Caterina (Arduino, Pro Micro) via avrdude (http://nongnu.org/avrdude/)
*  - HalfKay (Teensy, Ergodox EZ) via Teensy Loader (https://pjrc.com/teensy/loader_cli.html)
*  - LUFA/QMK HID via hid_bootloader_cli (https://github.com/abcminiuser/lufa)
*  - WB32 DFU via wb32-dfu-updater_cli (https://github.com/WestberryTech/wb32-dfu-updater)
*  - LUFA Mass Storage
* Supported ISP flashers:
*  - AVRISP (Arduino ISP)
*  - USBasp (AVR ISP)
*  - USBTiny (AVR Pocket)
