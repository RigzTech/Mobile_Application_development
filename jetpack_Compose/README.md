Set up your Android project 

bookmark_border
Note: Instructions on this page are written for Android Studio Flamingo and may vary for later Android Studio versions.
Create a new Compose project
Android Studio projects need configuration to work with Relay. To start, create a project that supports Jetpack Compose version 1.2 or newer.

In Android Studio, create a new project (File > New > New Project…).
Select Empty Compose Activity and click Next.

Create new Compose project in Android Studio
Give your project a name. Accept all other defaults, including the language as Kotlin and the minimum SDK as API 21: Android 5.0 (Lollipop) and click Finish.

Android Studio project configuration
Edit module-level Gradle build file
Set up the module-level Gradle build file to use the Relay Gradle plugin.

Open build.gradle (Module: Hello_Figma.app — This can vary based on the name you entered above). This is the module-level Gradle build file.

Module-level Gradle file in the Android Studio
Add the Relay plugin in the module's Gradle file as shown below, changing the version number as appropriate. Save the file.

Groovy
Kotlin

plugins {
  id 'com.android.application'
  id 'kotlin-android'
  id 'com.google.relay' version '0.3.12'
}
Click Sync Now.

Gradle Sync message in the Android Studio
