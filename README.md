## Firmware Flasher for Oneplus 8t and 9r

# 22-Jan-2023 v1.0
 - Initial Version of the updated flashable Firmware script for Oneplus 8t and 9r
 - OOS13 Firmware files are using abl.img from OOS13 F10 to remove the yellow bootloader message
 - Flasher should support Firmware flashing from all OOS12 and OOS13 Versions (OOS11 is not supported now!)
 - added automatic DDR RAM type detection
 - Flasher will terminate if it can not detect the correct RAM type by some reason
 - added a check that the Firmware flasher is flashed from recovery only
 - added device check that the Frimware is flashed on a supported device
 - Updated info that the Firmware is getting flashed to both slots (A and B)


Since the Oneplus 8t and 9r can have different RAM types (DDR4 or DDR5) you always had to check your RAM
type before flashing a new Firmware using the Firmware flasher.
Flashing the wrong Firmware file with wrong DDR type could brick your phone and it can be a mess to get it working again if so.

Now I built an updated Version of the Firmware Flasher which will automatically detect the RAM type of your device and flash the correct
Firmware files, so no need anymore to check the DDR RAM type before, now you can just go ahead and flash the needed Firmware you want to flash.
The flasher will terminate if it can not detect the RAM type or the correct Device for the Firmware you want to flash so it is quite safe now to use it and should not cause
any more bricks due to wrongly flashed Firmware for DDR RAM type. 
Since the command I use for detecting the RAM type is only working from OOS12 and OOS13 base the flasher will not work when trying to flash a new Firmware from OOS11 base!


##### Credits
- Nixsuki for the initial Version of the Oneplus Flashable Firmwares
- OPTeam for the Repo of OxygenOS builds

