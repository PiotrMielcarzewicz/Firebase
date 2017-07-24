# Firebase-Carthage
[![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage)
[![GitHub release](https://img.shields.io/github/release/soheilbm/Firebase.svg)](https://github.com/soheilbm/Firebase/releases)

#### Unofficial Firebase support for Carthage.

----

## Warning
If you are encountering **Undefined symbols** reffering to Analytics Discrepancies, please look at issue [#10](https://github.com/soheilbm/Firebase/issues/10). Thanks to [@brianlenz](https://github.com/brianlenz).

## Usage
The iOS Example file is a sample of using core firebase (analytics). 

You need to add <b>GoogleService info plist</b> to your main project. (iOS Example project also needs Googleservice info plist)

## Installation

### Carthage

[Carthage](https://github.com/Carthage/Carthage) is a decentralized dependency manager that builds your dependencies and provides you with binary frameworks.

You can install Carthage with [Homebrew](http://brew.sh/) using the following command:

```bash
$ brew update
$ brew install carthage
```

To integrate Firebase into your Xcode project using Carthage, specify it in your `Cartfile`:

```ogdl
github "soheilbm/Firebase" 
```

Run `carthage update` to build the framework and drag the built `Firebase.framework` into your Xcode project.

- Add the -ObjC flag to "Other Linker Settings"
- Turn on ALWAYS_EMBED_SWIFT_STANDARD_LIBRARIES in your build settings.
- Drag each framework from the directory named after the SDK into the Project
   Navigator pane. Note that there may be no additional frameworks, in which
   case this directory will be empty. For instance, if you want the Database
   SDK, look in the Database folder for the required frameworks. In the dialog
   box that appears, make sure the target you want this framework to be added to
   has a checkmark next to it, and that you've selected "Copy items if needed.


"(~> X)" below means that the SDK requires all of the frameworks from X. You
should make sure to include all of the frameworks from X when including the SDK.

#### Analytics
  - FirebaseAnalytics.framework
  - FirebaseCore.framework
  - FirebaseInstanceID.framework
  - GoogleToolboxForMac.framework


#### AdMob (~> Analytics)
  - GoogleMobileAds.framework


#### AppIndexing (~> Analytics)
  - FirebaseAppIndexing.framework


#### Auth (~> Analytics)
  - FirebaseAuth.framework
  - GTMSessionFetcher.framework


#### Crash (~> Analytics)
  - FirebaseCrash.framework
  - Protobuf.framework


#### Database (~> Analytics)
  - FirebaseDatabase.framework


#### DynamicLinks (~> Analytics)
  - FirebaseDynamicLinks.framework


#### Invites (~> Analytics)
  - FirebaseDynamicLinks.framework
  - FirebaseInvites.framework
  - GTMOAuth2.framework
  - GTMSessionFetcher.framework
  - GoogleAPIClientForREST.framework
  - GoogleSignIn.framework
  - Protobuf.framework

  You'll also need to add the resources in the
  Resources directory into your target's main
  bundle.
  
  
#### Messaging (~> Analytics)
  - FirebaseMessaging.framework
  - Protobuf.framework


#### RemoteConfig (~> Analytics)
  - FirebaseRemoteConfig.framework
  - Protobuf.framework


#### Storage (~> Analytics)
  - FirebaseStorage.framework
  - GTMSessionFetcher.framework



### Current Version of Firebase libraries

           Carthage           | Version
----------------------------- | -------
Firebase                      | 4.0.4
FirebaseAnalytics             | 4.0.2
FirebaseAuth                  | 4.0.0
FirebaseCore                  | 4.0.4
FirebaseCrash                 | 2.0.0
FirebaseDatabase              | 4.0.0
FirebaseDynamicLinks          | 2.0.0
FirebaseInstanceID            | 2.0.0
FirebaseInvites               | 2.0.0
FirebaseMessaging             | 2.0.0
FirebasePerformance           | 1.0.3
FirebaseRemoteConfig          | 2.0.1
FirebaseStorage               | 2.0.0
GTMOAuth2                     | 1.1.4
GTMSessionFetcher             | 1.1.11
Google-Mobile-Ads-SDK         | 7.21.0
GoogleAPIClientForREST        | 1.3.0
GoogleSignIn                  | 4.0.2
GoogleToolboxForMac           | 2.1.1
Protobuf                      | 3.3.0
nanopb                        | 0.3.8



## Author

Soheil B.Marvasti


## License
I do not own this project.
