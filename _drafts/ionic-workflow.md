---
layout: post
title: "Ionic Workflow"
---

# Ionic Workflow

## Start Project

`ionic start [dir name] [sidemenu|tabs|blank] --appname "[APP NAME]" --id "[com.example.appname]"`

## Add Platform

### iOS

iOS platform is added automatically after running `ionic start`

### Android

`ionic platform add android`

## Add Plugins

`ionic plugin add [plugin name/id]`

Adding plugins will automatically register the plugin within the `package.json` under `cordovaPlugins` key.

@todo: code block from package.json

Now if you reinstall from scratch (when "platform" and "plugins" folders are missing) Ionic will be able to add plugins back automatically.

## Splashscreens & Icons

All you need to do is creating two files (either .psd, .ai or .png) within the `resources` directory (create if not exist). One named `icon` that needs to follow `this template` and the other named `splash` that needs to follow `this template`.

`ionic resources`

## Ionic Build
## Ionic Run
## Ionic Serve
### Live reload & Console logs
## Ionic View

## Performance

* collection-repeat vs ng-repeat
* Disable $log.debug
* Disable ng-binding classes/attributes
* WebView (Crosswalk & WKWebView)
	* Greater Performance
	* Avoid device fragmentation
	* Provide a feature rich experience on all Android 4.x devices
	* Easily debug with Chrome DevTools

## App Store Submission

Email from iTunes Connect regarding Missing Push Notification Entitlement:

Email w/ Subject Line: iTunes Connect: Your app "YOUR APP NAME HERE" (Apple ID: 0000000000) has one or more issues

"Dear developer,

We have discovered one or more issues with your recent delivery for "My IP - Network IP Address Lookup Utility - Public Internet & Local WiFi". Your delivery was successful, but you may wish to correct the following issues in your next delivery:

Missing Push Notification Entitlement - Your app appears to include API used to register with the Apple Push Notification service, but the app signature's entitlements do not include the "aps-environment" entitlement. If your app uses the Apple Push Notification service, make sure your App ID is enabled for Push Notification in the Provisioning Portal, and resubmit after signing your app with a Distribution provisioning profile that includes the "aps-environment" entitlement. See "Provisioning and Development" in the Local and Push Notification Programming Guide for more information. If your app does not use the Apple Push Notification service, no action is required. You may remove the API from future submissions to stop this warning. If you use a third-party framework, you may need to contact the developer for information on removing the API.

After you’ve corrected the issues, you can use Xcode or Application Loader to upload a new binary to iTunes Connect.

Regards,

The App Store team"
