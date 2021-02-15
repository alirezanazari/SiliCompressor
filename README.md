# SiliCompressor
A powerful, flexible and easy to use Video and Image compression library for Android.


Description
--------
#### Video
Due to the high resolution of our Smartphone cameras and cameras from other devices, Video files have become large in size and thus difficult for it to be shared with others on social apps, social media and even when we need to upload it on our server. With SiliCompressor you can now compress you video file while maintaining it quality.

Credit
--------
The image compressor part of this project is inspired from [Void Canvas] blog from which the core part of the compressor was done.
For the Video Compression part of this project, credit goes to [Jorge E. Hernandez (@lalongooo)] whose codes was used for the core part of the video compressor module.

Usage
--------
```
implementation "com.github.alirezanazari:silicompressor:3.0.0"
```

```
VideoCompressor.getInstance(context).run {
    convertVideo(videoPath, File(destinationDirectory), width, height, bitrate)
    val compressedPath = VideoCompressor.cachedFile.path.also {
       release()
    }
}
```

License
--------
Copyright 2016 [Teyou Toure Nathan][toure]

Licensed under the Apache License, Version 2.0 (the "License") and GNU General Public License v2.0;

you may not use this file except in compliance with the Licenses.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0 and https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.


[snap]:  https://oss.sonatype.org/content/repositories/snapshots
[toure]:  https://www.linkedin.com/in/toure-nathan/
[Void Canvas]: http://voidcanvas.com/whatsapp-like-image-compression-in-android/
[Jorge E. Hernandez (@lalongooo)]: https://github.com/lalongooo
