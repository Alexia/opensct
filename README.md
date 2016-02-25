#Open SCT Flash
Reverse engineering SCT Flash products mainly the X4.

**Done**
* [Pull file system off device.](sdcard/NO NAME)
* [Document important integrated circuits and JTAG connectors.](docs/Circuit Board.md)

**To Do / Goals**
* Figure out what the pin hole button does on the button.
 * This prevents the device from being able to communicate over USB.  Theorized to be a service mode for repair services at SCT.
* Fully reverse engineer update server API and document.
* Flash custom firmware to the X4 handheld.
 * SCT Updater software will flash anything it is given from a HTTP server it contacts assuming the response is correct.
* Removing all pairing restrictions.
 * Initial discovery shows this can be done with JTAG and some soldering.  However, the preferable way would be through a custom firmware update since there would be no evidence of tampering by way of a broken "WARRANTY VOID" sticker.
* Load unlimited custom tunes(strategies) onto the device.
 * This already seems possible software wise.  It just looks it is functionality limited possibly due to hardware limitations.