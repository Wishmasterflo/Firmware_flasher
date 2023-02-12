## Firmware Flasher script for Oneplus 8 series and Oneplus 9 series

Since the Oneplus 8t and 9r can have different RAM types (DDR4 or DDR5) you always had to check your RAM
type before flashing a new Firmware.
Flashing the wrong Firmware file with wrong DDR type could brick your phone and it can be a mess to get it working again.

Now I built an updated Version of the Firmware Flasher which will automatically detect the RAM type of your device and flash the correct
Firmware files, so no need anymore to check the DDR RAM type before, now you can just go ahead and flash the needed Firmware you want to flash.
The flasher will terminate if it can not detect the RAM type or the correct Device for the Firmware you want to flash so it is quite safe now to use it and should not cause any more bricks due to wrongly flashed Firmware.

# Download
Firmware download with updated Firmware flasher script: https://mega.nz/folder/W7JhwTAT#Yu6cxqvJcAC28cy0m_kkQA

Device type and region
XXX0 = China
XXX1 = India
XXX3 = Europe
XXX5 = Global/NA

# Flashing procedure
The firmware zip file can be flashed from a custom recovery via adb sideload or flash directly from Storage on the Phone from a custom recovery.
It gets flashed to both slots so no need to flash it twice!

# Features
 - automatic detection of RAM type
 - automatic detection of device type
 - The Firmware gets flashed to both A/B slots
 - For T-Mobile devices on OOS12/13 it will enable the Dual SIM feature
 - Choice to Update modem.img or not

# Supported Devices
 - Oneplus 8 IN201X (instantnoodle)
 - Oneplus 8t KB200X (kebab)
 - Oneplus 8 Pro IN202X (instantnoodlep)
 - Oneplus 9 LE211X (lemonade)
 - Oneplus 9r LE210X (lemonades)
 - Oneplus 9 Pro LE212X (lemonadep)

# Changelog
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


##### Credits
- Nixsuki for the initial Version of the Oneplus Flashable Firmwares
- OPTeam for the Repo of OxygenOS builds
