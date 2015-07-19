About
-----

This project is originally a Launcher3 project that was maintained separately in a separate folder.
With a new capability to set lockscreen wallpaper from CM, I extend this project so that it can be used to set wallpaper for lockscreen.


Requirement
-----------
You need this following patch to work with this project:
https://github.com/SlimSaber/frameworks_base/commit/eec3552a1af220fe5388b25cc91f6ba373f29b60


How to use it
-------------
There is an intent's extra "keyguardMode" to distinguish between lockscreen or home screen mode.
You can use it in a preference screen like this following example:
```
<intent
    android:targetPackage="com.slim.wallpaperpicker"
    android:targetClass="com.slim.wallpaperpicker.WallpaperPickerActivity">
	<extra android:name="keyguardMode" android:value="true" />
</intent>
```
