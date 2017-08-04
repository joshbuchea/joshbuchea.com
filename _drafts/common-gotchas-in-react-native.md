---
layout: post
title: Common Gotchas in React Native
category: React Native
---

## Gotchas

- Disable Dead Code Stripping (iOS)
- defaultProps, truthy values, & styles don't all play nice together
- TextView + padding don't behave as expected (Android) https://github.com/facebook/react-native/issues/3233
- NavigatorIOS --> Navigator
- Font Scaling (iOS)
- Keyboard Spacer
- White flash between splash and app load

### Disable Dead Code Stripping (iOS)

fdsfd

### Font Scaling (iOS)

React Native Docs: Specifies should fonts scale to respect Text Size accessibility setting on iOS.

A default behavior of `<Text>` components in React Native is to honor the `Text Size` accessibility setting on iOS. You may, or may not desire your `<Text>` components to respect this setting. To disable font scaling on a `<Text>` component, set it's `allowFontScaling` prop to `false`.

```html
<Text>Hi! I will change if the OS tells me to :P</Text>
```

```html
<Text allowFontScaling={false}>Hi! I won't change :)</Text>
```

I found a solution,Text.defaultProps.allowFontScaling=false, it works, it is global
