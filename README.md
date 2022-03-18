# WebRTCAndroid
This is an Android Studio reference project for WebRTC based video and voice calling app. (https://appr.tc)

<img src="screenshots/screenshot1.png" width=200/> <img src="screenshots/screenshot2.png" width=200/> <img src="screenshots/screenshot3.png" width=200/>

For downloading the latest source follow the instructions given [here](https://webrtc.org/native-code/android/). 

## Modifications

1. The code has been split into library and app modules for easy reference. 
2. Changes incorporated for requesting runtime permissions and targetSdkVersion updated to 27 (Oreo).
3. Added dependency to official prebuilt library available at JCenter 'org.webrtc:google-webrtc'.

## Miscellaneous

Update: As per https://github.com/webrtc/apprtc
> appr.tc has been shutdown. Please use the Dockerfile to run your own test/dev instance. 

The app connects to AppRTC server hosted by Google (which has been shutdown). If you wish to deploy your own server then follow the instructions given [here](https://github.com/webrtc/apprtc). Or you may use out-of-the-box docker image for AppRTC-Server available [here](https://hub.docker.com/r/piasy/apprtc-server/).

```
docker run --rm --net=host
-e PUBLIC_IP=xx.xxx.xx.xx
-it piasy/apprtc-server
```

> http://xx.xxx.xx.xx:8080 is the server url.

Once your server is up and running, you will need to specify the server url in the Settings screen of the app. Update 'Room server URL' under Miscellaneous settings.

<img src="screenshots/screenshot4.png" width=200/>
