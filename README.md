android-media-player-standalone-library
=======================================

A container for the Android Veeso Libraries. 

Javadoc documentation is available here: [http://veeplay.github.io/android-media-player-standalone-library/](http://veeplay.github.io/android-media-player-standalone-library/)

A valid Veeso License is required for running the player. You can sign-up for a trial license here: [panel.veeso.co](https://panel.veeso.co)

Please note that the Eclipse project distribution is no longer supported. The most recent Veeplay SDK is available via Maven. Add the following lines to your build.gradle files:

    repositories {
      mavenCentral()
      maven {
        url "https://s3-eu-west-1.amazonaws.com/android.veeplay.com/releases"
      }
    }
    dependencies {
       compile 'com.veeplay:veeplay-player-android:2.1.0'
       compile 'com.veeplay:veeplay-cast-plugin:1.1.0' //optional
    }
