# WebRTCAndroid
This is an Android Studio reference project for WebRTC based video and voice calling app. (https://appr.tc)

<img src="screenshots/screenshot1.png" width=200/><img src="screenshots/screenshot2.png" width=200/><img src="screenshots/screenshot3.png" width=200/>

For downloading the latest source follow the instructions given [here](https://webrtc.org/native-code/android/). 

## Modifications

1. The code has been split into library and app modules for easy reference. 
2. Changes incorporated for requesting runtime permissions and targetSdkVersion updated to 27 (Oreo).
3. Added dependency
```
implementation 'org.webrtc:google-webrtc:1.0.+'
```

## Miscellaneous

The app connects to AppRTC server hosted by Google. If you wish to deploy your own server then follow the instructions given [here](https://github.com/webrtc/apprtc).

