# ActivityIndicatingNavigationItem

_UINavigationItem subclass that indicates activity with UIActivityIndicator for right and left  bar button items._

![Platform iOS](https://img.shields.io/badge/platform-iOS-blue.svg)
[![CocoaPods compatible](https://img.shields.io/cocoapods/v/ActivityIndicatingNavigationItem.svg)](https://cocoapods.org/pods/ActivityIndicatingNavigationItem)
[![MIT license](http://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/longhorn499/ActivityIndicatingNavigationItem/raw/master/LICENSE.md)


## Description

A UINavigationItem subclass you can use to easily animate loading on either side. 

- Useful for indicating activity with system "Save" or "Done" bar buttons
- Common in iOS UI/UX design when tapping a bar button saves or loads information

<img src="https://raw.githubusercontent.com/longhorn499/ActivityIndicatingNavigationItem/master/Screenshots/Animating.gif"/>

## Installation

With [CocoaPods](https://cocoapods.org), add ActivityIndicatingNavigationItem to your Podfile:

```
pod 'ActivityIndicatingNavigationItem'
```

Then install with `pod install`.

Or you can manually import the files from the Source folder.


## Usage

If you're using a Storyboard, set the name of the Class and Module, then create an outlet:

``` swift
@IBOutlet weak var activityIndicatingNavigationItem: ActivityIndicatingNavigationItem!
```

Or set up programmatically:

``` swift
let activityIndicatingNavigationItem = ActivityIndicatingNavigationItem.init(title: "Edit Profile", indicatorStyle: .white)
```


Start animating side:

``` swift
activityIndicatingNavigationItem.startAnimating(.right)
```

Stop animating:

``` swift
activityIndicatingNavigationItem.stopAnimating(.right)
```


## Configuration

Changing the activity indicator style  (default style is `gray`):

````swift
activityIndicatingNavigationItem.indicatorStyle = .white
````

Changing the activity indicator color (can also update in Storyboard):

````swift
activityIndicatingNavigationItem.indicatorColor = .blue
````

## Requirements

Written in Swift 4.0, requires iOS 10.0 and above, Xcode 9.0 and above.


## Credits

Created by [Kevin Johnson](http://www.johnsonkevin.com).


## License

Available under the MIT license. See the LICENSE file for more info.
