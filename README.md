## Extend version of react-native-youtube 

I just add the portrait mode mentioned [this article](https://medium.com/@mridx/youtubestandaloneandroid-play-youtube-videos-in-portrait-mode-in-android-react-native-hack-edd0fdce6088)

All Readme can be found [here](https://github.com/davidohayon669/react-native-youtube)

## Install

` yarn add react-native-youtube-portrait-mode-enabled ` 

If you already the react-native-youtube package installed.

just remove the old one with 

` yarn remove react-native-youtube ` then rebuild your project

change your import names as new package

## Extra install requirement

Expand ‘app > manifests’ , there might be two files with same name as ‘AndroidManifest.xml’ one for debug. Open the other one add these lines 

```
<activity android:name="com.inprogress.reactnativeyoutube.YTPlayer"
    android:configChanges="orientation|screenSize|layoutDirection"
    android:turnScreenOn="true"
    tools:targetApi="o_mr1"
    android:resizeableActivity="true"
    />
```

Note: Don't care about `YTPlayer not found` error. Just build!

## Thanks
- [MriDx](https://medium.com/@mridx/youtubestandaloneandroid-play-youtube-videos-in-portrait-mode-in-android-react-native-hack-edd0fdce6088)
- Param Aggarwal (paramaggarwal@gmail.com)
- David Ohayon ([@davidohayon669](https://twitter.com/davidohayon669))

## License

MIT License
