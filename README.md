<<<<<<< HEAD
# VennCache

<p align="left">
<img src="https://img.shields.io/badge/made%20with-%3C3-orange.svg">
</p>

VennCache is a fork of Kingfisher that seeks to create an ideal caching system for iOS applications that require blazing speeds. This means it's slightly heavier than Kingfisher, but will support important features to creating a high-speed environment like progressive JPEGs and short video caching. This is ideal for social media applications; hence, the name VennCache--this is the cache we use for our app Venn (coming soon).

> Kingfisher is a lightweight, pure-Swift library for downloading and caching images from the web. This project is heavily inspired by the popular [SDWebImage](https://github.com/rs/SDWebImage). It provides you a chance to use a pure-Swift alternative in your next app.
=======
<p align="center">

<img src="https://raw.githubusercontent.com/onevcat/Kingfisher/master/images/logo.png" alt="Kingfisher" title="Kingfisher" width="557"/>

</p>

<p align="center">
<a href="https://travis-ci.org/onevcat/Kingfisher"><img src="https://img.shields.io/travis/onevcat/Kingfisher/master.svg"></a>
<a href="https://github.com/Carthage/Carthage/"><img src="https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat"></a>
<a href="https://swift.org/package-manager/"><img src="https://img.shields.io/badge/SPM-ready-orange.svg"></a>
<a href="http://onevcat.github.io/Kingfisher/"><img src="https://img.shields.io/cocoapods/v/Kingfisher.svg?style=flat"></a>
<a href="https://raw.githubusercontent.com/onevcat/Kingfisher/master/LICENSE"><img src="https://img.shields.io/cocoapods/l/Kingfisher.svg?style=flat"></a>
<a href="http://onevcat.github.io/Kingfisher/"><img src="https://img.shields.io/cocoapods/p/Kingfisher.svg?style=flat"></a>
<a href="https://codebeat.co/projects/github-com-onevcat-kingfisher"><img alt="codebeat badge" src="https://codebeat.co/assets/svg/badges/A-398b39-669406e9e1b136187b91af587d4092b0160370f271f66a651f444b990c2730e9.svg" /></a>
<a href="https://pledgie.com/campaigns/34143"><img src="https://img.shields.io/badge/Donate-Pledgie-green.svg"></a>
</p>
>>>>>>> onevcat/master

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

## What's next?

- [ ] Progressive JPEGs

<<<<<<< HEAD
- [ ] Short video caching (.mov)

## Other

=======
We prepared a [wiki page](https://github.com/onevcat/Kingfisher/wiki). You can find tons of useful things there.

* [Installation Guide](https://github.com/onevcat/Kingfisher/wiki/Installation-Guide) - Follow it to integrate Kingfisher into your project.
* [Cheat Sheet](https://github.com/onevcat/Kingfisher/wiki/Cheat-Sheet)- Curious about what Kingfisher could do and how would it look like when used in your project? See this page for useful code snippets. If you are already familiar with Kingfisher, you could also learn new tricks to improve the way you use Kingfisher! 
* [API Reference](http://onevcat.github.io/Kingfisher/) - Lastly, please remember to read the full whenever you may need a more detailed reference.

## Other

### Future of Kingfisher

I want to keep Kingfisher lightweight. This framework will focus on providing a simple solution for downloading and caching images. This doesn’t mean the framework can’t be improved. Kingfisher is far from perfect, so necessary and useful updates will be made to make it better.

### Developments and Tests

Any contributing and pull requests are warmly welcome. However, before you plan to implement some features or try to fix an uncertain issue, it is recommended to open a discussion first. 

The test images are contained in another project to keep this project repo fast and slim. You could run `./setup.sh` in the root folder of Kingfisher to clone the test images when you need to run the tests target. It would be appreciated if your pull requests could build and with all tests green. :)

### About the logo

The logo of Kingfisher is inspired by [Tangram (七巧板)](http://en.wikipedia.org/wiki/Tangram), a dissection puzzle consisting of seven flat shapes from China. I believe she's a kingfisher bird instead of a swift, but someone insists that she is a pigeon. I guess I should give her a name. Hi, guys, do you have any suggestions?

### Contact

Follow and contact me on [Twitter](http://twitter.com/onevcat) or [Sina Weibo](http://weibo.com/onevcat). If you find an issue, just [open a ticket](https://github.com/onevcat/Kingfisher/issues/new). Pull requests are warmly welcome as well.

>>>>>>> onevcat/master
### License

VennCache is released under the MIT license. See VennCache-LICENSE for details.

Kingfisher is released under the MIT license. See Kingfisher-LICENSE for details.


