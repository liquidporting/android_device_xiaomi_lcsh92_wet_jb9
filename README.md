## TWRP device tree for Xiaomi Redmi Note 3G (lcsh92_wet_jb9)

Add to `.repo/local_manifests/lcsh92_wet_jb9.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/xiaomi/lcsh92_wet_jb9" name="android_device_xiaomi_lcsh92_wet_jb9" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_lcsh92_wet_jb9-eng
make -j5 recoveryimage
```