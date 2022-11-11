---
title: "Getting Started"
author: markSaava
draft: false
date: 2021-12-26
tags:
  - good first issue
categories:
  - First Issue
---

Download the latest stable release of the Flutter SDK
Extract the zip file and place the contained flutter in the desired installation location for the Flutter SDK (for example, C:\Users<your-user-name>\Documents).
Do not install Flutter in a directory like C:\Program Files\ that requires elevated privileges

Update your path
If you wish to run Flutter commands in the regular Windows console, take these steps to add Flutter to the PATH environment variable:

From the Start search bar, enter ‘env’ and select Edit environment variables for your account.
Under User variables check if there is an entry called Path:
If the entry exists, append the full path to flutter\bin using ; as a separator from existing values.
If the entry doesn’t exist, create a new user variable named Path with the full path to flutter\bin as its value.
You have to close and reopen any existing console windows for these changes to take effect.

where flutter dart
C:\path-to-flutter-sdk\bin\flutter
C:\path-to-flutter-sdk\bin\flutter.bat
C:\path-to-dart-sdk\bin\dart.exe :: this should go after C:\path-to-flutter-sdk\bin\ commands
C:\path-to-flutter-sdk\bin\dart
C:\path-to-flutter-sdk\bin\dart.bat
As shown above, the command dart from the Flutter SDK doesn’t come first. Update your path to use commands from C:\path-to-flutter-sdk\bin\ before commands from C:\path-to-dart-sdk\bin\ (in this case). After restarting your shell for the change to take effect, running the where command again should show that the flutter and dart commands from the same directory now come first.

where flutter dart
C:\dev\src\flutter\bin\flutter
C:\dev\src\flutter\bin\flutter.bat
C:\dev\src\flutter\bin\dart
C:\dev\src\flutter\bin\dart.bat
C:\dev\src\dart-sdk\bin\dart.exe
However, if you are using PowerShell, in it where is an alias of Where-Object command, so you need to use where.exe instead.
Run flutter doctor
From a console window that has the Flutter directory in the path, run the following command to see if there are any platform dependencies you need to complete the setup:
C:\src\flutter>flutter doctor
This command checks your environment and displays a report of the status of your Flutter installation. Check the output carefully for other software you might need to install or further tasks to perform

For example:
[-] Android toolchain - develop for Android devices
• Android SDK at D:\Android\sdk
✗ Android SDK is missing command line tools; download from https://goo.gl/XxQghQ
• Try re-installing or updating your Android SDK,
visit https://docs.flutter.dev/setup/#android-setup for detailed instructions.
The following sections describe how to perform these tasks and finish the setup process. Once you have installed any missing dependencies, you can run the flutter doctor command again to verify that you’ve set everything up correctly.

Note: If flutter doctor returns that either the Flutter plugin or Dart plugin of Android Studio are not installed, move on to Set up an editor to resolve this issue.

Android setup
Note: Flutter relies on a full installation of Android Studio to supply its Android platform dependencies.
Install Android Studio
Download and install Android Studio.
Start Android Studio, and go through the ‘Android Studio Setup Wizard’. This installs the latest Android SDK, Android SDK Command-line Tools, and Android SDK Build-Tools, which are required by Flutter when developing for Android.
Run flutter doctor to confirm that Flutter has located your installation of Android Studio. If Flutter cannot locate it, run flutter config --android-studio-dir to set the directory that Android Studio is installed to.
Set up your Android device
To prepare to run and test your Flutter app on an Android device, you need an Android device running Android 4.1 (API level 16) or higher.

![Sample](https://user-images.githubusercontent.com/96499644/147417931-ea0cb553-92bb-4aee-992c-8c966377f6ee.png)

- [EUNOMIA's official website](https://eunomia.social/)
- [EUNOMIA's blog](https://blog.eunomia.social/)
