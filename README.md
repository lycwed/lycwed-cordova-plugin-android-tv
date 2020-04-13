# lycwed-cordova-plugin-android-tv

Cordova plugin to manage app for Android TV.

## Install

`cordova plugin add lycwed-cordova-plugin-android-tv`

## Requirements

Create a banner.png of your app (1280x720).
In the folder `resources/android` create a folder `drawable` and put it in.

Then add in your config.xml in platform android :

```xml
        <edit-config file="app/src/main/AndroidManifest.xml" mode="merge" target="/manifest/application" xmlns:android="http://schemas.android.com/apk/res/android">
            <application android:banner="@drawable/banner" />
            <application android:isGame="true" />
        </edit-config>
        <resource-file src="resources/android/drawable/banner.png" target="app/src/main/res/drawable/banner.png" />
```
