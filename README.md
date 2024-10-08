# Go Home With You

Welcome to Go Home With You - a Flutter project designed to help you safely navigate your way back home.

## Overview

Go Home With You is a mobile application developed using Flutter, available for both iOS and Android platforms. The primary purpose of this application is to provide users with a reliable tool to navigate their way home safely, ensuring a smooth and secure journey.

## Features

-   Easy-to-use interface
-   GPS navigation to guide you home
-   Customizable settings for preferred routes
-   Safety features such as alarm system for emergencies
-   Integration with public transportation options

## Usage

Once installed, launch the Go Home With You app on your device. Enter your home address or set it as a default in the settings. The app will provide you with navigation instructions to guide you safely home.

## Setting Up Firebase

Before you proceed, it's essential to set up Firebase for your project. Follow the image below to configure Firebase fields:



![alt文本](https://github.com/sanoisaboy/Go_home_with_you/blob/Sunny/image/firebase.png)

(It is important to set the collection name `userdata`).

## Set up Google API Key

### Android 

Specify your API key in the application manifest android/app/src/main/AndroidManifest.xml

```bash
   <manifest ...
      <application ...
            <meta-data android:name="com.google.android.geo.API_KEY"
                  android:value="YOUR KEY HERE"/>
```

### IOS

Specify your API key in the application delegate ios/Runner/AppDelegate.swift:

```bash
import UIKit
import Flutter
import GoogleMaps

@UIApplicationMain
@objc class AppDelegate: FlutterAppDelegate {
  override func application(
    _ application: UIApplication,
    didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?
  ) -> Bool {
    GMSServices.provideAPIKey("YOUR KEY HERE")
    GeneratedPluginRegistrant.register(with: self)
    return super.application(application, didFinishLaunchingWithOptions: launchOptions)
  }
}
```

## Getting Started


To get started with Go Home With You, follow these simple steps:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/YunJ-Chang/Go_home_with_you.git
    ```
2. **Navigate to the Project Directory**:
    ```bash
    cd go-home-with-you
    ```
3. **Install Dependencies**:
    ```bash
    flutter pub get
    ```
4. **Install Dependencies**:
   Run the Application:

    _Connect your device/emulator_
    _Execute the following command_

    ```bash
    flutter run --dart-define=google_api_key="YOUR GOOGLE API KEY" --dart-define=firebase_api_key="YOUR FIREBASE API KEY"
    ```
## Pictures of Interface
 - Login Interface, Search location, Map, and Path deviation detection  
<img width="20%" src="https://github.com/user-attachments/assets/4b3fce4b-dd72-482f-9d02-dac3c6042281"/><img width="20%" src="https://github.com/user-attachments/assets/3b05f961-bd50-4655-a240-feb92422b95f"/><img width="20%" src="https://github.com/user-attachments/assets/adaea082-9e93-4448-9fa9-baf1e2c2403f"/><img width="20%" src="https://github.com/user-attachments/assets/a7b9855a-b72d-4372-aeff-7e29bb7e7d07"/>

## Author

- Author:
  - CHIH-HSUAN, SHEN
  - Yun-Chieh, Chang
  - Min-Yu, Liang
  - Hao-Wei, LU
- Contact:
  - s890919@gmail.com
  - jill1006.chang@gmail.com
  - kanggoking@gmail.com
  - haoweilu.go@gmail.com
