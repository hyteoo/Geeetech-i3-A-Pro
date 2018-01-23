# Geeetech i3 A Pro
## Config files for the Marlin 1.1.8 firmware

This repo contains the ported settings for the latest Marlin firmware.
Stock settings + minor tweaks.

I try to keep the config up to date, for earlier versions, check the revision history.

# Installation, flashing
* Get the latest version of Arduino (tested with 1.8.5 but latest one should work fine)
* Get the official Marlin release from here: https://github.com/MarlinFirmware/Marlin/releases
* Download config files from this repo and overwrite the ones in the Marlin firmware
* Get the U8glib library from here: https://github.com/olikraus/U8glib_Arduino/releases. Currently latest version 1.19.1 works fine

Compile, upload with Arduino IDE (selecting "*Arduino/Genuino Mega or Mega 2560*" as board) directly to the Geeetech GT2560 controller.

**Tip** It's highly recommended to clear the EEPROM values. This can be done **after** flashing the firmware in 2 ways:
* by sending GCode: `M502` `M500` (Restore default settings + save to EEPROM)
* by selecting from the printer LCD menu: Control -> Init EEPROM.
