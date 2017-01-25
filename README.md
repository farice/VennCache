# VennCache

<p align="center">
<img src="https://img.shields.io/badge/made%20with-%3C3-orange.svg">
</p>

VennCache is a fork of Kingfisher that seeks to create an ideal caching system for iOS applications that require blazing speeds. This means it's slightly heavier than Kingfisher, but will support important features to creating a high-speed environment like progressive JPEGs and short video caching. This is ideal for social media applications; hence, the name VennCache--this is the cache we use for our app Venn (coming soon).

> Kingfisher is a lightweight, pure-Swift library for downloading and caching images from the web. This project is heavily inspired by the popular [SDWebImage](https://github.com/rs/SDWebImage). It provides you a chance to use a pure-Swift alternative in your next app.

Thanks @onevcat for the awesome library!

## Features

- [x] Asynchronous image downloading and caching.
- [x] `URLSession`-based networking. Basic image processors and filters supplied.
- [x] Multiple-layer cache for both memory and disk.
- [x] Cancelable downloading and processing tasks to improve performance.
- [x] Independent components. Use the downloader or caching system separately as you need.
- [x] Prefetching images and showing them from cache later when necessary.
- [x] Extensions for `UIImageView`, `NSImage` and `UIButton` to directly set an image from a URL.
- [x] Built-in transition animation when setting images.
- [x] Extensible image processing and image format support.

The simplest use-case is setting an image to an image view with the `UIImageView` extension:

```swift
let url = URL(string: "url_of_your_image")
imageView.kf.setImage(with: url)
```

Kingfisher will download the image from `url`, send it to both the memory cache and the disk cache, and display it in `imageView`. When you use the same code later, the image will be retrieved from cache and shown immediately.

## Requirements

- iOS 8.0+ / macOS 10.10+ / tvOS 9.0+ / watchOS 2.0+
- Swift 3 (Kingfisher 3.x), Swift 2.3 (Kingfisher 2.x)

Main development of Kingfisher will support Swift 3. Only critical bug fixes will be made for Kingfisher 2.x.

[Kingfisher 3.0 Migration Guide](https://github.com/onevcat/Kingfisher/wiki/Kingfisher-3.0-Migration-Guide) - If you are upgrading to Kingfisher 3.x from an earlier version, please read this for more information.

## What's next?

- [ ] Progressive JPEGs

- [ ] Short video caching (.mov)

## Other

### License

VennCache is released under the MIT license. See VennCache_LICENSE for details.

Kingfisher is released under the MIT license. See Kingfisher_LICENSE for details.


