---
layout: post
title: "React Native Text Size & Font Scaling"
category: React Native
---

A default behavior of `<Text>` components in React Native is to honor the `Text Size` accessibility setting on iOS. You may, or may not desire your `<Text>` components to respect this setting. To disable font scaling on a `<Text>` component, set it's `allowFontScaling` prop to `false`.

```html
<Text allowFontScaling={false}>
  Hi! I won't change unless you tell me too :)
</Text>
```

```html
<Text>
  Hi! I will change if the OS tells me to :P
</Text>
```

_**Note:** As of the date of this post, font scaling isn't present in the iOS Simulator; only on a physical device. That makes it much easier to miss this during development. Also, keep in mind that when using icon fonts such as those in [react-native-vector-icons](https://github.com/oblador/react-native-vector-icons), font scaling will also affect your icons._

## Default Text Size

<div class="image-wrapper">
  <img
    src="/images/posts/react-native-ios-text-size-default.png"
    alt="React Native Text Size Default"
    width="300"
  />
</div>

## Large Text Size

<div class="image-wrapper">
  <img
    src="/images/posts/react-native-ios-text-size-large.png"
    alt="React Native Text Size Large"
    width="300"
  />
</div>

## Larger Text Size

<div class="image-wrapper">
  <img
    src="/images/posts/react-native-ios-text-size-larger.png"
    alt="React Native Text Size Larger"
    width="300"
  />
</div>

## Small Text Size

<div class="image-wrapper">
  <img
    src="/images/posts/react-native-ios-text-size-small.png"
    alt="React Native Text Size Small"
    width="300"
  />
</div>
