1.8.6
=====
- Minor bugfixes for DRM managers
1.8.5
=====
- APSMediaEvents definitions are now an Enum instead of String constants
- Player events are no longer local broadcasts but implement a Listener model. Please implement the new APSMediaPlayerTrackingEventListener interface and review the APSMediaEvents documentation if upgrading from older versions
- Fixed a bug where events were not emitted if no tracking urls were defined
- Fixed a bug where controls were not shown when building an APSMediaUnit instance and not setting an autohide duration
1.8.4
=====
- Fixed a bug preventing events to be dispatched
- Replaced JS YouTube API with the Android YouTubeAPI (if upgrading from 1.8.3 or older, please add your YouTube API key when initialising the player)
1.8.3
=====
- Added support for the Marlin DRM Plugin
1.8.2
=====
- Improved support for playing HLS / M3U8 streams
- Configurable livestream indicator in controls overlay
- Support for midrolls and overlays
- Support for youtu.be URLs in the Youtube Overlay Controller
- Added a configurable flag for disabling the player on rooted phones
- Added methods for explicitly entering or exiting full-screen mode
- Support for configuring actions when dismissing clicked overlays / linears
- Metadata support for units and overlays
- Corrected the aspect ratio of Webview buttons
- Configurable preferred video mime types
- Improved support for tracking royalties