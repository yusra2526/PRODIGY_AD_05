# QR Code Scanner App

This Android application scans QR codes and opens the URLs contained within the codes in a browser.

## Features

- Scans QR codes using the device's camera
- Automatically opens URLs contained in QR codes
- Simple and intuitive user interface

## Prerequisites

- Android Studio
- An Android device or emulator with a camera

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/yourusername/qrcode-scanner.git
cd qrcode-scanner
```

## Open the Project in Android Studio

1. Open Android Studio.
2. Select File > Open and navigate to the cloned repository.
3. Open the project.

## Add ZXing Dependencies

Ensure that the following dependencies are included in your build.gradle (Module: app) file:

```bash
dependencies {
    implementation 'com.journeyapps:zxing-android-embedded:4.3.0'
    implementation 'com.google.zxing:core:3.4.1'
    // other dependencies
}
```

## Sync Project with Gradle Files

After adding the dependencies, sync your project with Gradle files.

## Update Android Manifest

Add the necessary camera permissions in your AndroidManifest.xml:

```bash
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.INTERNET"/>

<application
    ...>
    ...
    <activity android:name=".MainActivity">
        <intent-filter>
            <action android:name="android.intent.action.MAIN" />
            <category android:name="android.intent.category.LAUNCHER" />
        </intent-filter>
    </activity>
</application>
```
