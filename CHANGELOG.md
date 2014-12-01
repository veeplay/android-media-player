1.9.6
=====
- Added a bugfix for a crash during player finish
- Added seek handling support: by default, the player will only play the last scheduled adbreak, when seeking. This can be configured via the APSMediaUnit#seekHandling field, or using the JSON configuration, on the content unit: "seekAdHandling": "last" (/first/all)
- Added automatic ad breaks positioning: a minimum initial offset, minimum final offset and minimum interval between ad-breaks can be set (all default to 300 seconds). Ad breaks that are not configured with an offset will be automatically scheduled based on these three parameters.
- Added the FORWARD event, for detecting forward seeks
- The SurfaceView is now secure, by default, on devices with API level > 17. This behaviour can be changed by calling APSMediaPlayer#setSecureSurfaceView(false) before initializing the player.

1.9.5
=====
- Added unit and overlay metadata keys for current adbreak offset
- Unit metadata is now copied for unit clones

1.9.4
=====
- Added a bugfix preventing seeking past the end of a video unit
- Added the PLAYLIST_FINISHED trackable event for detecting the end of the playback of the last unit in the playlist

1.9.3
=====
- Re-implemented full-screen mode toggling
- Bug fixes for text and skip overlays
- Bugfixes affecting multiple ads in an adbreak

1.9.2
=====
- Addressed a bug causing a crash when toggling full-screen mode.

1.9.1
=====
- Added a more detailed error message for invalid licenses

1.9.0
=====
- Units, Overlays and AdBreaks are now APSMediaEvent instances. This allows just-in-time VAST/VMAP feed retrieval, as well as banner preloading on Image overlays
- APSMediaBuilder#mediaUnits and APSMediaPlayer#playMediaUnits now accept ArrayList<APSMediaEvent>
- APSMediaUnit, APSMediaOverlay and APSVastAdBreak are now members of the com.appscend.media.events package
- APSMediaEvents has ben renamed to APSMediaTrackingEvents

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
