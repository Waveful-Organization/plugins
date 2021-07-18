# Video Player plugin for Flutter (+ caching support)

A modified version of Video Player plugin that has been forked from the official [video_player](https://pub.dev/packages/video_player) package except that it supports caching in Android and iOS.
Web plugin will work like official [video_player](https://pub.dev/packages/video_player) i.e. without caching support.


### Managing new updates of video_player
To add cache support to a new version of [video_player](https://pub.dev/packages/video_player) simply copy and paste these 5 files:
* `/android/src/main/java/io/flutter/plugins/videoplayer/CacheDataSourceFactory.java`
* `/android/src/main/java/io/flutter/plugins/videoplayer/SimpleCacheSingleton.java`
* `/android/src/main/java/io/flutter/plugins/videoplayer/VideoPlayer.java`
* `/ios/Classes/FLTVideoPlayerPlugin.m`
* `/ios/video_player.podspec`

Of course some changes may be needed if those files have been modified in an update of [video_player](https://pub.dev/packages/video_player).

### Issues
* `maxFileSize` and `maxCacheSize` are hardcoded at 100MiB and 1GiB respectively in Android.


### Contributors

* [Vikram Pratap Singh](https://github.com/vikram25897)
* [EnderTan](https://github.com/EnderTan)
* [Desno365](https://github.com/Desno365)
