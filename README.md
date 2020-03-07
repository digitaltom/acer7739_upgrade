# Upgrading an Acer Aspire 7739 to Windows 10

Upgrading an Acer 7739 notebook from Windows 7 to Windows 10 with the 
official [update script](https://www.chip.de/downloads/Windows-10-Update-Assistent_97600470.html) 
will fail because that notebook doesn't have the virtualization features (VT) enabled 
by default. 

Unfortunately the BIOS is locked by default into a 'simple' mode, which cannot change that 
setting. 

## Unlocking 'advanced' BIOS settings

To enable the 'advanced' BIOS settings, put the file [HMAX64.fd](HMAX64.fd) on
a Fat32 formatted USB stick and follow this procedure: 

* Put the USB Memory Stick in the USB port
* Hold "Fn" + "Esc" and power on the notebook
* Wait until the fan will run, then release "Fn" + "Esc" keys
* The fan will run for about 2-10 minutes and the USB drive activity LED will blink

After this is done, you will have all options available in the BIOS, 
and the Windows10 update will work. 

