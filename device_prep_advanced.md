# Co:Vid Device Prepping Volunteer Guide: Advanced

## **⚠🛑 Do not share outside of the Co:Vid development team. The content is under review and does not represent official positions of any entity or organization. This site will be updated as the project develops. **

## Overview

This series of steps assumes something went wrong with the steps above. It will use a command line tool on a desktop/laptop computer and a usb connection to the device to manually update the phone to work with Signal. This section will be added to as problems / solutions arise.

## Procedure

### Step 1 - Set up Computer
* You’ll need:
    * USB Driver from: [https://developer.android.com/studio/run/win-usb](https://developer.android.com/studio/run/win-usb) (Only required for Windows- install this)

    * ADB command line tool package from: [https://developer.android.com/studio/releases/platform-tools](https://developer.android.com/studio/releases/platform-tools)

    * Signal APK file from: [https://signal.org/android/apk/](https://signal.org/android/apk/)

### Step 2 - Setup Phone
* Step 1 - Put the phone in developer mode.
    * From the Settings -> About Phone, find the ‘Build Number’
    * Tap this multiple times until you are a developer
* Step 2 - Turn on Settings for development
    * Under the Settings Menu, find the ‘Developer Options’
    * Enable the option marked ‘USB Debugging’
    * Optionally enable ‘Stay Awake’
* Step 3 - Plug Phone into Computer USB

### Step 3 - Install Signal Via ADB
*(If the apk installed correctly using the manual method in non-advanced setup steps, you can skip this step)*
* In the PowerShell Window, and using the tab key for auto-completion, type:
```
    adb{tab} install sig{tab}
```
* This should autocomplete to something like:
```
    .\adb.exe install .\Signal-website-universal-release-4.57.2.apk
```
* Press {enter}
    * The application will be installed.

