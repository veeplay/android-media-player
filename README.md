Veeplay for Android SDK
=======================================

**Javadoc documentation:** [http://veeplay.github.io/android-media-player-standalone-library/](http://veeplay.github.io/android-media-player-standalone-library/)

**Current changelog:** https://github.com/veeplay/android-media-player/wiki/Changelog

**SSAI player documentation:** https://github.com/veeplay/android-media-player/wiki/SSAI-Documentation

**Google Cast documentation:** https://github.com/veeplay/android-media-player/wiki/Google-Cast-Documentation

A valid Veeplay License is required for running the player. You can sign-up for a trial license here: [panel.veeso.co](https://panel.veeso.co)

This repository contains a stand-alone container for the Android Veeplay Libraries, usable with old ANT-based Android projects. Please note that this Eclipse project distribution is no longer supported. The most recent Veeplay SDK is available via Maven. 

Add the following lines to your build.gradle files:

    repositories {
      mavenCentral()
      maven {
        url "https://s3-eu-west-1.amazonaws.com/android.veeplay.com/releases"
      }
    }
    dependencies {
       compile 'com.veeplay:veeplay-player-android:3.1.2'
    }
