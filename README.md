# ffmpeg-kit-apk (mobile-ffmpeg)
The Android test apps for [mobile-ffmpeg](https://github.com/tanersener/mobile-ffmpeg) and [ffmpeg-kit](https://github.com/tanersener/ffmpeg-kit), compiled. The official repositories contain the source for these apps, but they don't come precompiled (only the .AAR package is provided).

I've been using these apps for a while, since they're not really 'test' apps but full-featured example apps that do everything I need. However, I recently lost the APK and had to re-compile it for my new phone. So I decided to archive my compiled APKs in this repo, given that compiling ffmpeg and the subpackages for the apps took a lot of time on regular hardware. I don't want to do that again anytime soon.

No changes to the source were made. The only change I made to the mobile-ffmpeg app was the gradle version in gradle-wrapper.properties, because 6.0.1 gave me errors but 6.7.1 did not.

Tested with a Samsung Galaxy S21 on Android 12. Only used the ARM64-packages but the other archs should work fine too.


Args used for building mobile-ffmpeg:
```
--enable-chromaprint --enable-fontconfig --enable-freetype --enable-gnutls --enable-lame --enable-twolame --enable-libaom --enable-libass --enable-libtheora --enable-libvorbis --enable-libvpx --enable-libwebp --enable-libxml2 --enable-opus --enable-rubberband --enable-snappy --enable-soxr --enable-speex --enable-tesseract --enable-x264 --enable-x265 --enable-shine --enable-libvidstab --enable-wavpack --enable-fribidi --enable-opencore-amr --enable-xvidcore --enable-gpl
```

Args used for building ffmpeg-kit-test:
```
--enable-chromaprint --enable-fontconfig --enable-freetype --enable-gnutls --enable-lame --enable-twolame --enable-libaom --enable-libass --enable-libtheora --enable-libvorbis --enable-libvpx --enable-libwebp --enable-libxml2 --enable-opus --enable-rubberband --enable-snappy --enable-soxr --enable-speex --enable-tesseract --enable-x264 --enable-x265 --enable-shine --enable-libvidstab --enable-dav1d --enable-fribidi --enable-opencore-amr --enable-xvidcore --enable-gpl
```

###mobile-ffmpeg:<br>
<img src="https://raw.githubusercontent.com/belieb/ffmpeg-kit-apk/main/mobile-ffmpeg.gif" width="295">

###ffmpeg-kit-test:<br>
<img src="https://raw.githubusercontent.com/belieb/ffmpeg-kit-apk/main/ffmpeg-kit.gif" width="295">
