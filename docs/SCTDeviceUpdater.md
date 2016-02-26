#SCT Device Updater
The SCT Device Updater application is a buggy piece of software that handles updating firmware, tunes, strategies, and other functions of SCT devices.

##Initial Startup
The application calls out to this URL to determine if it needs to self update.
http://cdn.derivesystems.com/sctfiles/SoftwareUpdates/SCTDeviceUpdater/currentsctdeviceupdater.txt
Note: All calls to the CDN should use a cache break of some sort at the end of the URL such as "?this=that".

The response will be a pipe and comma delimited list of update data.  It contains the version numbers to their corresponding platform builds.
```
Executable32|2.9.16033.08|23797760,Executable64|2.9.16033.08|23797760
```
Where the sections can be expressed as this regular expression: `#Executable32\|([0-9\.]*?)\|([0-9]*?),Executable64\|([0-9\.]*?)\|([0-9]*?)#`

##Driver Update Check
The application will call out to one of these two URLs, depending on the platform, to determine if driver updates are needed.
http://cdn.derivesystems.com/sctfiles/SoftwareUpdates/DriverUpgrade/latestdriver_x64.txt
http://cdn.derivesystems.com/sctfiles/SoftwareUpdates/DriverUpgrade/latestdriver_x86.txt