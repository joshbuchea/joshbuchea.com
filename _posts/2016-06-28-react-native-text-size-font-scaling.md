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

_**Note:** As of the publication date of this post, font scaling behavior isn't present in the iOS Simulator; only physical devices. That makes it much easier to miss this during development. Also, keep in mind that when using icon fonts like [react-native-vector-icons](https://github.com/oblador/react-native-vector-icons), font scaling will also affect your icons._

<div class="image-wrapper">
  <img
    src="/images/posts/react-native-font-size-text-scaling.gif"
    alt="React Native Text Size & Font Scaling"
    width="300"
  />
</div>
