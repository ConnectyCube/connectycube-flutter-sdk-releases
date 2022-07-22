[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner2-direct.svg)](https://stand-with-ukraine.pp.ua)

# ConnectyCube Flutter SDK Releases

This repository contains changelog and links to Flutter products released by ConnectyCube.

If you have any questions, comments, or issues related to any products distributed via this repository then please raise an issue here on GitHub repository  
or contact the team by emailing support@connectycube.com.

## SDK overview

ConnectyCube helps you implement real-time chat, video chat, push notifications and user authorization to any app with ease - no server side implementation required.  
You can concentrate fully on your mobile app development. Our Flutter SDK provides you with many helpful methods to build the chat and video chat from the client side.

This page presents a quick overview of the SDK’s functionalities and logic, then let you go through the easy steps of implementing ConnectyCube in your own app.

ConnectyCube Flutter SDK can be used on the following OS:

- Android
- iOS

## Create ConnectyCube app

Register a FREE ConnectyCube account at [https://connectycube.com/signup](https://connectycube.com/signup), then create your 1st app and obtain an app credentials.  
These credentials will be used to identify your app.

All users within the same ConnectyCube app can communicate by chat or video chat with each other, across all platforms - iOS, Android, Web, etc.

## When building a new app

If you are just starting your app and developing it from scratch, we recommend to use our Code Samples projects.

[Download Code Samples (coming soon)](https://developers.connectycube.com/flutter/code-samples)

These code samples are ready-to-go apps with an appropriate functionality and simple enough that even novice developers will be able to understand them.

## When integrating SDK into existing app

If you already have an app, do the following for integration.

### Connect SDK

#### 1. Depend on it

Add this to your package's `pubspec.yaml` file:

```yaml
dependencies:
  connectycube_sdk: ^x.x.x
```

`x.x.x` is a latest version of [connectycube_sdk](https://pub.dev/packages/connectycube_sdk/versions) on [pub.dev](https://pub.dev) repository.

#### 2. Install it

You can install packages from the command line:

with Flutter:

```shell
flutter pub get
```

Alternatively, your editor might support flutter pub get. Check the docs for your editor to learn more.

#### 3. Import it

Now in your Dart code, you can use:

```dart
import 'package:connectycube_sdk/connectycube_sdk.dart';
```

### Initialize

Initialize framework with your ConnectyCube application credentials. You can access your application credentials  
in [ConnectyCube Dashboard](https://admin.connectycube.com):

```dart
String appId = "";
String authKey = "";
String authSecret = "";

init(appId, authKey, authSecret);
```

### Configuration

An additional configs can be passed via `CubeSettings`:

```dart
CubeSettings.instance.isDebugEnabled = true; // to enable ConnectyCube SDK logs; 
CubeSettings.instance.setEndpoints(customApiEndpoint, customChatEndpoint); // to set custom endpoints
```

### Now integrate messaging & calling capabilities

Follow the API guides on how to integrate chat and calling features into your app:

- [Messaging API documentation](https://developers.connectycube.com/flutter/messaging)
- [Calling API documentation (coming soon)](https://developers.connectycube.com/flutter/videocalling)

## SDK Changelog

The complete SDK changelog is available on [ConnectyCube pub.dev](https://pub.dev/packages/connectycube_sdk#-changelog-tab-) page.

## Contact

You can reach the ConnectyCube team at any time by emailing [support@connectycube.com](mailto:support@connectycube.com).

## License

ConnectyCube SDK for Flutter is licensed under the ConnectyCube SDK License.
