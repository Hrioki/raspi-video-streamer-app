# raspi-video-streamer-app
Kotlin Android Application For Receiving a Live Stream from A RaspberryPi.

Server implementation is available at [robsmall/flask-raspi-video-streamer](https://github.com/robsmall/flask-raspi-video-streamer)

Resources For Learning:
-----------------------
- [Jake Wharton talk on use of Retrofit to help understand cool features.](http://jakewharton.com/making-retrofit-work-for-you-ohio/)
- [Jake Wharton talk on Retrofit and RxJava being used together](http://jakewharton.com/retrofit-and-rxjava/)
- [Kotlin & Retrofit article](https://android.jlelse.eu/keddit-part-6-api-retrofit-kotlin-d309074af0) -- See related github.
- [Kotlin & RxJava & RxAndroid article](https://android.jlelse.eu/keddit-part-5-kotlin-rxjava-rxandroid-105f95bfcd22) -- See related github.

Configuration
-------------
In the `build.gradle` file licated in `app`, you must create and set the path and properties for `secureProperties`.

For Example:

I have a file located at `/Users/robsmall/src/android/RaspiVideoStreamer/secure-gradle.properties` that contains:
```
BaseApiUrl=http://10.0.0.7:5000
BaseRawStreamUrl=http://10.0.0.7:8000
```

For more information on this gradle plugin, please [Check the Java Prop File documentation](https://plugins.gradle.org/plugin/com.admc.javaPropFile)

For the example server, check out [robsmall/flask-raspi-video-streamer](https://github.com/robsmall/flask-raspi-video-streamer)

Credits
-------
- [MJpeg Library](https://github.com/niqdev/ipcam-view)
- [RetroFit](http://square.github.io/retrofit/)
- [RxJava](https://github.com/ReactiveX/RxJava)
- [RxAndroid](https://github.com/ReactiveX/RxAndroid)
- [OkHTTP](http://square.github.io/okhttp/)
- [Timber](https://github.com/JakeWharton/timber)
- [RxJava2Adapter for Retrofit](https://github.com/square/retrofit/tree/master/retrofit-adapters/rxjava2)
- [Moshi Converter for Retrofit](https://github.com/square/retrofit/tree/master/retrofit-converters/moshi)
- [ButterKnife](http://jakewharton.github.io/butterknife/)
- [Java Prop File](https://plugins.gradle.org/plugin/com.admc.javaPropFile)