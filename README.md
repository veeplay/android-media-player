android-media-player-standalone-library
=======================================

A container for the Android Veeso Libraries. 

Javadoc documentation is available here: [veeso.github.io/android-media-player-standalone-library/](veeso.github.io/android-media-player-standalone-library/)

A valid Veeso License is required for running the player. You can sign-up for a trial license here: [panel.veeso.co](https://panel.veeso.co)

The SDK is also available via Maven. Add the following lines to your build.gradle files:

    repositories {
      mavenCentral()
      maven {
        url "https://s3-eu-west-1.amazonaws.com/android.veeplay.com/releases"
      }
    }
    dependencies {
       compile 'com.veeplay:veeplay-player-android:2.0.26'
       compile 'com.veeplay:veeplay-cast-plugin:1.0.6' //optional
    }
