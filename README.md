### TBT8A10 Modded Recovery
This is the stock recovery, with some modifications made to it.

#### Modifications:
* The recovery menu is now immediately displayed, pressing volume and power buttons to access it is no longer needed
* Decreased security: Build variant set to userdebug, selinux to permissive, etc.
* Fixes to ADB: Now it's always available, and root access can be obtained with `adb root`
* Added "RECOVERY" label to the ENACOM logo. Note that this logo is almost never shown, only when rebooting to recovery through fastboot/ADB.
* pstore mounted at `/sys/fs/pstore`. Kernel panic logs are available there

If your `data` partition is not encrypted and you want to mount it, take a look to [this commit](https://github.com/TBT8A10/recovery/commit/4bd4af4f509666d721de886bfcf56aea30a6dee2)
