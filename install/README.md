### Firmware Installation

If a previous version of the Flux Capacitor firmware is installed on your device, you can update easily using the pre-compiled binary. Enter the [Config Portal](#the-config-portal), click on "Update" and select the pre-compiled binary file provided in this repository ([install/fluxcapacitor-A10001986.ino.nodemcu-32s.bin](https://github.com/realA10001986/Flux-Capacitor/blob/main/install/fluxcapacitor-A10001986.ino.nodemcu-32s.bin)).

If you are using a fresh ESP32 board, please see [fluxcapacitor-A10001986.ino](https://github.com/realA10001986/Flux-Capacitor/blob/main/fluxcapacitor-A10001986/fluxcapacitor-A10001986.ino) for detailed build and upload information, or, if you don't want to deal with source code, compilers and all that nerd stuff, go [here](https://install.out-a-ti.me) and follow the instructions.

 *Important: After a firmware update, the inner and outer LEDs might blink alternately for short while after reboot. Do NOT unplug the device during this time.*

### Audio data installation

The firmware comes with audio data ("sound-pack") which needs to be installed separately. The audio data is not updated as often as the firmware itself. If you have previously installed the latest version of the sound-pack, you normally don't have to re-install the audio data when you update the firmware. Only if either a the FC puts up a respective [signal](#appendix-b-led-signals) at startup, or your device is quiet after a firmware update, a re-installation is needed.

The first step is to download "install/sound-pack-xxxxxxxx.zip" and extract it. It contains one file named "FCA.bin".

Then there are two alternative ways to proceed. Note that both methods *require an SD card*.

1) Through the [Config Portal](#the-config-portal). Click on *Update*, select this file in the bottom file selector and click on *Upload*. Note that an SD card must be in the FC's slot during this operation.

2) Via SD card:
- Copy "FCA.bin" to the root directory of of a FAT32 formatted SD card;
- power down the Flux Capacitor,
- insert this SD card into the slot and 
- power up the Flux Capacitor; the audio data will be installed automatically.
