---
layout: post
title: "React Native: Set RootView Background Color"
category: React Native
---

In the RootView of a React Native app, the default background color is white. We can change this to another color by following the steps below.

In this example we'll set the background color to **black**.

**Note:** _Changing the background color may resolve issues related to launch screen flicker/flash and background color during orientation change._

## iOS

**Open `AppDelegate.m` located in `PROJECT_DIR/ios/Appname/` for editing.**

**Locate snippet that looks similar to:**

    RCTRootView *rootView = [[RCTRootView alloc] initWithBundleURL:jsCodeLocation
                                                      moduleName:@"Appname"
                                               initialProperties:nil
                                                   launchOptions:launchOptions];




**Add the following line of code immediately after the previous snippet:**

```
rootView.backgroundColor = [UIColor blackColor];
```

**The resulting code block should look similar to:**

    RCTRootView *rootView = [[RCTRootView alloc] initWithBundleURL:jsCodeLocation
                                                    moduleName:@"Appname"
                                             initialProperties:nil
                                                 launchOptions:launchOptions];

    rootView.backgroundColor = [UIColor blackColor];

**The RootView background color has been changed on iOS!**

It is also possible to set the background color using RGBA values:

```
rootView.backgroundColor = [[UIColor alloc] initWithRed:.01f green:.75f blue:.54f alpha:1];
```

[UIColor](http://uicolor.xyz/#/hex-to-ui) is a handy website that can be used to convert HEX & RGB colors to UIColor for both Objective-C and Swift.

iOS steps were sourced from [Changing the React Native RootView Background Color (iOS and Android)](http://moduscreate.com/changing-the-react-native-rootview-background-color-ios-and-android/) by Jay Garcia. (I believe the Android information in this post may be out of date, which is why I didn't include steps for Android).
