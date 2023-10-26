<img src="https://related.chat/hud/q01.gif" width="80"> <img src="https://related.chat/hud/z01.gif" width="80"> <img src="https://related.chat/hud/z02.gif" width="80"> <img src="https://related.chat/hud/z03.gif" width="80"> <img src="https://related.chat/hud/z04.gif" width="80"> <img src="https://related.chat/hud/z05.gif" width="80"> <img src="https://related.chat/hud/z06.gif" width="80"> <img src="https://related.chat/hud/z07.gif" width="80"> <img src="https://related.chat/hud/z08.gif" width="80"> <img src="https://related.chat/hud/z09.gif" width="80"> <img src="https://related.chat/hud/z10.gif" width="80"> <img src="https://related.chat/hud/z11.gif" width="80"> <img src="https://related.chat/hud/z12.gif" width="80"> <img src="https://related.chat/hud/z13.gif" width="80"> <img src="https://related.chat/hud/z14.gif" width="80"> <img src="https://related.chat/hud/z15.gif" width="80"> <img src="https://related.chat/hud/z16.gif" width="80"> <img src="https://related.chat/hud/z17.gif" width="80"> <img src="https://related.chat/hud/z18.gif" width="80"> <img src="https://related.chat/hud/z19.gif" width="80"> <img src="https://related.chat/hud/z20.gif" width="80"> <img src="https://related.chat/hud/z21.gif" width="80"> <img src="https://related.chat/hud/q02.gif" width="80"> <img src="https://related.chat/hud/q03.gif" width="80"> <img src="https://related.chat/hud/q04.gif" width="80"> 

## WHAT'S NEW

For detailed changes, please refer to the [Change log](CHANGELOG.md).

## OVERVIEW

**ProgressHUD** is a convenient and intuitive HUD tool designed specifically for iOS. It enables seamless presentation of concise alerts or notifications to users of your app in a simple and non-disruptive way.

## INSTALLATION

‼️ In case you're using Xcode 14.3.1 or an earlier version, stick with [13.8.6](https://github.com/relatedcode/ProgressHUD/releases/tag/13.8.6) ‼️

### CocoaPods

[CocoaPods](https://cocoapods.org) is a dependency manager for Swift and Objective-C Cocoa projects.

To incorporate the **ProgressHUD** library into your Xcode project utilizing CocoaPods, please reference it within your `Podfile` as shown below:

```ruby
pod 'ProgressHUD'
```

### Swift Package Manager

[Swift Package Manager](https://swift.org/package-manager) is a tool for managing the distribution of Swift code.

To add **ProgressHUD** as a dependency to your project, follow these steps:

1. Open your Swift project in Xcode.
2. Navigate to `File` -> `Add Package Dependencies...`.
3. Paste `https://github.com/relatedcode/ProgressHUD.git` into the search bar.
4. Choose the version you want to use and click `Add Package`.

### Manually

If you prefer not to use any of the dependency managers above, you can integrate **ProgressHUD** into your project manually. Just copy all the `*.swift` files from the `ProgressHUD/Sources` folder into your Xcode project.

## QUICK START

```swift
ProgressHUD.banner("Banner title", "Banner message to display.")
```

```swift
ProgressHUD.banner("Banner title", "Message to display.", delay: 2.0)
```

```swift
ProgressHUD.bannerHide()
```

```swift
ProgressHUD.animate("Some text...")
```

```swift
ProgressHUD.animate("Some text...", interaction: false)
```

```swift
ProgressHUD.animate("Please wait...", .ballVerticalBounce)
```

```swift
ProgressHUD.succeed()
```

```swift
ProgressHUD.succeed("Some text...", delay: 1.5)
```

```swift
ProgressHUD.failed()
```

```swift
ProgressHUD.failed("Some text...")
```

```swift
ProgressHUD.progress(0.15)
```

```swift
ProgressHUD.progress("Loading...", 0.42)
```

```swift
ProgressHUD.symbol(name: "box.truck")
```

```swift
ProgressHUD.symbol("Some text...", name: "sun.max")
```

```swift
ProgressHUD.dismiss()
```

```swift
ProgressHUD.remove()
```

## REQUIREMENTS

- iOS 13.0+
- Xcode 15.0+

## CUSTOMIZATION

You can customize attributes like color, font, image, animation type, size, and more by using these methods:

```swift
ProgressHUD.animationType = .circleStrokeSpin
```

```swift
ProgressHUD.colorHUD = .systemGray
```

```swift
ProgressHUD.colorBackground = .lightGray
```

```swift
ProgressHUD.colorAnimation = .systemBlue
```

```swift
ProgressHUD.colorProgress = .systemBlue
```

```swift
ProgressHUD.colorStatus = .label
```

```swift
ProgressHUD.mediaSize = 100
ProgressHUD.marginSize = 50
```

```swift
ProgressHUD.fontStatus = .boldSystemFont(ofSize: 24)
```

```swift
ProgressHUD.imageSuccess = UIImage(named: "success.png")
ProgressHUD.imageError = UIImage(named: "error.png")
```

A comprehensive list of the predefined enums:

```swift
public enum AnimationType: CaseIterable {
	case none
	case activityIndicator
	case ballVerticalBounce
	case barSweepToggle
	case circleArcDotSpin
	case circleBarSpinFade
	case circleDotSpinFade
	case circlePulseMultiple
	case circlePulseSingle
	case circleRippleMultiple
	case circleRippleSingle
	case circleRotateChase
	case circleStrokeSpin
	case dualDotSidestep
	case horizontalBarScaling
	case horizontalDotScaling
	case pacmanProgress
	case quintupleDotDance
	case semiRingRotation
	case sfSymbolBounce
	case squareCircuitSnake
	case triangleDotShift
}
```

```swift
public enum LiveIcon {
	case succeed
	case failed
	case added
}
```

## LICENSE

MIT License

Copyright (c) 2023 Related Code

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
