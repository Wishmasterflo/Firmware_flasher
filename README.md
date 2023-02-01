## Firmware Flasher script for Oneplus 8 series and Oneplus 9 series

# 01-Feb-2023 v1.2
 - Added prompt to continue or cancel the Firmware flashing
 - Removed RAM check for all other devices (exept OP8t and OP9r) 
 - Added RAM check for OP8t and 9r on OOS11 as well
 - Make flashing of Modem.img optional
 - Some small adjustments to the flashing script

# 25-Jan-2023 v1.1
 - Fixed typo in the flashing script
 - Cleaned up the flashing script

# 22-Jan-2023 v1.0
 - Initial Version of the updated flashable Firmware script for Oneplus 8 series and Oneplus 9 series
 - OOS13 Firmware files are using abl.img from OOS13 F10 to remove the yellow bootloader message
 - Flasher should support Firmware flashing from all OOS12 and OOS13 Versions (OOS11 is not supported now!)
 - added automatic DDR RAM type detection (for Oneplus 8t/9r)
 - Flasher will terminate if it can not detect the correct RAM type for some reason
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

Firmware download with updated Firmware flasher script: https://mega.nz/folder/W7JhwTAT#Yu6cxqvJcAC28cy0m_kkQA

The firmware can just be flashed from a custom recovery via adb sideload or flash directly from Storage on the Phone from custom recovery.

##### Credits
- Nixsuki for the initial Version of the Oneplus Flashable Firmwares
- OPTeam for the Repo of OxygenOS builds

