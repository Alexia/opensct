#Open SCT Flash
Reverse engineering SCT Flash products mainly the X4.

**Goals**
* Fully reverse engineer update server API and document.
* Flash custom firmware to the X4 handheld.
 * SCT Updater software will flash anything it is given from a HTTP server it contacts assuming the response is correct.
* Removing all pairing restrictions.
 * This can be done with JTAG and some soldering, but the preferable way would be through a custom firmware update.  That way there is no evidence of tampering by way of a broken "WARRANTY VOID" sticker.
* Load unlimited custom tunes(strategies) onto the device.
 * This already seems possible software wise.  It just looks it is functionality limited possibly due to hardware limitations.