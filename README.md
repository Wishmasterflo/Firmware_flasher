# Firmware Flasher for Oneplus devices

I built an updated Version of the Firmware Flasher which will automatically detect the RAM type of your device and flash the correct
Firmware files, so no need anymore to check the DDR RAM type before, now you can just go ahead and flash the needed Firmware you want to flash.
The flasher will terminate if it can not detect the RAM type or the correct Device for the Firmware you want to flash so it is quite safe now to use it and should not cause any more bricks due to wrongly flashed Firmware.

# Download
Firmware download with updated Firmware flasher: https://mega.nz/folder/W7JhwTAT#Yu6cxqvJcAC28cy0m_kkQA

Device type and region
- XXX0 = China
- XXX1 = India
- XXX3 = Europe
- XXX5 = Global/NA
- XXX7 = T-Mobile Version

# Flashing procedure
Download the firmware zip file for your Device and Region from the download link above.
The firmware zip file can be flashed from a custom recovery via adb sideload or it can be directly flashed from the Internal Storage on the Phone (using TWRP/Orangefox).
It gets flashed to both slots so no need to flash it twice!
Disable your Virusscanner on Windows before adb sideloading the file!

# Features
 - automatic detection of RAM type
 - automatic detection of device type
 - The Firmware gets flashed to both A/B slots
 - For T-Mobile devices on OOS13 it will enable the Dual SIM feature (Oneplus 8/9 series)
 - Choice to Update modem.img or not (in 90% of the cases you choose yes here to update Modem)
   Only in some cases where you want to cross flash a different region Firmware it could be needed
   not to Update the modem.img as otherwise you might not have all 5G bands available for that region.

# Supported Devices
 - Oneplus 6 (enchilada)
 - Oneplus 6t (fajita)
 - Oneplus 7 GM190X (guacamoleb)
 - Oneplus 7 Pro GM191X (guacamole)
 - Oneplus 7t HD190X (hotdogb)
 - Oneplus 7t Pro HD191X (hotdog)
 - Oneplus 8 IN201X (instantnoodle)
 - Oneplus 8t KB200X (kebab)
 - Oneplus 8 Pro IN202X (instantnoodlep)
 - Oneplus 9 LE211X (lemonade)
 - Oneplus 9r LE210X (lemonades)
 - Oneplus 9 Pro LE212X (lemonadep)
 - The T-Mobile devices are supported as well. For those you would flash the NA/Global Firmware
 
# Changelog
# 14-Mar-2023 v1.3
 - Changed device check method
 - Cleaned up some old Firmware files to free up space on Mega

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
 - added device check that the Firmware is flashed on a supported device
 - Updated info that the Firmware is getting flashed to both slots (A and B)


##### Credits
- Nixsuki for the initial Version of the Oneplus Flashable Firmwares
- OPTeam for the Repo of OxygenOS builds
