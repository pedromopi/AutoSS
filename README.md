# Description

Automatically takes timed screenshots on iOS.

It won't use any official screenshot interface, so theoretically it will not be detected as a screenshot by apps.

It probably won't work on apps that disallow screenshots, such as streaming services (during streaming), due to the nature of how this view is displayed.

Developed for rootless environments. Tested on iPhone 13/iOS 15.3.

# Usage

Enable the tweak in settings and set the desired interval time for capturing your screen.

Screenshots will be saved to `/var/mobile/Documents/Screenshots`. 

Options might require two resprings to apply.

# Features

## Ignore duplicated screenshots

When this option is enabled, if the device's screen is the same as the last captured one, it will not be saved. It's useful when you leave your device stuck on some screen. Be aware that if even one single byte is different, it will be saved nonetheless, which includes, of course, the time changing in the status bar. Another handy use is when you SSH into your device and lock it, as it would keep taking screenshots of a wallpaperless lock screen.

## Screenshot quality

The quality of the resulting image, expressed as a value from 1 to 100. The value 1 represents the maximum compression (or lowest quality) while the value 100 represents the least compression (or best quality). Useful for saving storage. Based on compressionQuality from UIImageJPEGRepresentation.
