# Geeetech i3 A Pro
## Config files for the Marlin 1.1.5 firmware

This repo contains the ported settings for the latest Marlin firmware
Stock settings + minor tweaks
I try to keep the config up to date, for earlier versions, check the revision history.

# Installation, flashing
* Get latest version of Arduino (tested with 1.8.3 but latest one should work fine)
* First get the official Marlin release from here: https://github.com/MarlinFirmware/Marlin/releases
* Download config files from this repo and overwrite the ones in the Marlin firmware
* Get the U8glib library from here: https://github.com/olikraus/U8glib_Arduino/releases. Currently latest version 1.19.1 works fine

Compile, upload with Arduino IDE directly to the Geeetech GT2560 controller.

**Tip** It's highly recommended to clear the EEPROM values. This can be done **after** flashing the firmware, by sending GCode M502 (Revert to the default "factory settings").
