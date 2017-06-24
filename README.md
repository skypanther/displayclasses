Display Classes
==============

<p style="border: 1px solid #000;background-color:#455A64;color:white;padding:8px;"><strong>Note:</strong> This doc is pretty much superseded by Google''s listing of devices, physical size, density, etc. at <a href="https://design.google.com/devices/" style="color:white;">https://design.google.com/devices/</a> </p>

My little attempt to catalog device sizes, display classes, and related critical graphics detail for Android and iOS apps.


# Android

Android [defines](http://developer.android.com/guide/practices/screens_support.html#range)
a set of six generalized densities:

- ldpi (low) ~120dpi
- mdpi (medium) ~160dpi
- hdpi (high) ~240dpi
- xhdpi (extra-high) ~320dpi
- xxhdpi (extra-extra-high) ~480dpi
- xxxhdpi (extra-extra-extra-high) ~640dpi

## Android device details

If you have real devices please check numbers using utils like [ScreenInfo](https://github.com/mportuesisf/ScreenInfo)

|Brand / Device  |Class|PPI|logical Density Factor |platform Height|platform Width|
|-------|---|-----------|----|------------------|----|----|----|
|Google Nexus One  |hdpi  |252| | | |
|Google Nexus S  |hdpi  |233| | | ||
|Google Nexus 6 [\[1\]](#footnote1) |xxxhdpi  |560| |1440 |2560 |
|Google Nexus 7 2012  |mdpi|213|1.331250072|1205|800|
|Google Nexus 7 2013  |xhdpi  |323|2 |1920 |1104 |
|Google Nexus 4  |xhdpi  |318| | | |
|Google Nexus 9 [\[1\]](#footnote1) |xhdpi  |288| |2048 |1536 |
|Google Nexus 10  |xhdpi  |299| | | |
|HTC Wildfire  |mdpi  |125| | | |
|HTC Desire  |hdpi  |252| | | |
|HTC Desire S  |hdpi  |252| | | |
|HTC Sensation  |hdpi  |256| | | |
|HTC Desire X  |hdpi  |233| | | |
|HTC One S  |hdpi  |256| | | |
|HTC One V  |hdpi  |252|1.5|800|480|
|HTC Nexus One  |hdpi  |252| | | |
|HTC One X  |Xhdpi  |312| | | |
|HTC One  |xxhdpi  |469| | | |
|HTC One X+  |xhdpi  |312| | | |
|HTC One M8  |xxhdpi  |441| | | |
|LG Optimus one  |mdpi  |180| | | |
|LG Optimus S    |mdpi  |180| | | |
|LG Optimus V   |mdpi  |180| | | |
|LG F70  |mdpi  |199| | | |
|LG G2 mini  |hdpi  |234| | | |
|LG L90  |hdpi  |234| | | |
|LG G Pad  |hdpi  |273| | | |
|LG Nexus 4  |xhdpi  |318| | | |
|LG Nexus 5  |xxhdpi  |455| 3|1794 |1080 |
|LG G2 mini  |hdpi  |234| | | |
|Micromax Canvas 2 A110  |hdpi  |196| | | |
|Micromax Canvas Doodle A111  |hdpi  |185| | | |
|Micromax Canvas 2 + A110Q  |hdpi  |196| | | |
|Micromax Canvas HD A116  |xhdpi  |294| | | |
|Micromax Canvas 4 A210  |xhdpi  |294| | | |
|Micromax Canvas Magnus A117  |xhdpi  |294| | | |
|Micromax Canvas Turbo  |xxhdpi  |441| | | |
|Nokia N1||326 ||2048|1536|
|OnePlus One|xxhdpi|480|3|1920|1080|
|Samsung Galaxy Y  |ldpi| |0.75 | | |
|Samsung Galaxy Ace  |mdpi  |165| | | |
|Samsung Galaxy S  |hdpi  |233| 1.5|800 |480 |
|Samsung Galaxy S2  |hdpi  |240|1.5 |800 |480 |
|Samsung Galaxy S3  |xhdpi  |320|2 |1280|720 |
|Samsung Galaxy S4  |xxhdpi  |440|3|1920|1080|
|Samsung Galaxy S5  |xxhdpi  |432|3| 1920|1080 |
|Samsung Galaxy S6  |  |577| | 2560|1440 |
|Samsung Galaxy Nexus  |xhdpi  |316|2| | |
|Samsung Galaxy Tab 10  |mdpi  |149|1 |1280 |800 |
|Samsung Galaxy Tab 2 10  |mdpi  |149| | | |
|Samsung Galaxy Tab 4 10.1  |mdpi  |149 | |1280 |800 |
|Samsung Galaxy Tab Pro 8.4   |  |359 | |2560 |1600 |
|Samsung Galaxy Tab Pro 10.1  |  |299 | |2560 |1600 |
|Samsung Galaxy Tab Pro 12.2  |  |247 | |2560 |1600 |
|Samsung Galaxy Tab S 8.4   |  |359 | |2560 |1600 |
|Samsung Galaxy Tab S 10.5  |xhdpi  |288 | |2560 |1600 |
|Samsung Nexus 10 inch tablet  |xhdpi  |299| | | |
|Samsung Note  |xhdpi  |285| |1280 |800 |
|Samsung Note 2  |xhdpi  |267| |1280 |720 |
|Samsung Note 3  |  |388 | |1920 |1080 |
|Samsung Note 4  |  |515 | |2560 |1440 |
|Sony Xperia mini    |mdpi  |192| | | |
|Sony Xperia P  |hdpi  |275| | | |
|Sony Xperia S  |xhdpi  |342| | | |
|Sony Xperia J  |hdpi  |245| | | |
|Sony Xperia Arc  |hdpi  |233| | | |
|Sony Xperia Pro  |hdpi  |265| | | |
|Sony Xperia Z  |xxhdpi  |441| | | |
|Sony Xperia Z2  |xxhdpi  |424| | | |
|Motorola Droid  |mdpi  |265| | | |
|Motorola Defy  |hdpi  |265| | | |
|Motorola Razr XT910  |hdpi  |256| | | |
|Motorola Moto G  |xhdpi  |326| | | |
|Motorola Moto X  |xhdpi  |312| | | |


<a id="footnote1"></a>
  [1]: <http://android-developers.blogspot.com/2014/10/getting-your-apps-ready-for-nexus-6-and.html>


### Notes:

 * Ti.Platform.displayCaps.dpi represents Androids densityDpi which corresponds to the theoretical resolutions of the various density classes (low, medium, high, etc.). In other words, this value doesn't represent a device's true DPI. For that, look to Ti.Platform.displayCaps.xdpi and ydpi.
 * Ti.Platform.displayCaps.platformHeight does not include the height of the ActionBar.

### Android app icons

[Android](http://developer.android.com/design/style/iconography.html) says

> Launcher icons on a mobile device must be 48x48 dp.

That means to look good on all devices, you must prepare 5 icons with 1, 1.5x, 2x, 3x, and 4x scales as follows. These are placed in the res/drawable-DPICLASS folders.

* 48 × 48 pixels (mdpi)
* 72 × 72 pixels (hdpi)
* 96 × 96 pixels (xhdpi)
* 144 × 144 pixels (xxhdpi)
* 192 × 192 pixels (xxxhdpi)

See <http://iconhandbook.co.uk/reference/chart/android/> and also <https://github.com/google/material-design-icons>.


# iOS

iOS doesn't use display classes in the same way as Android. But it does have a similar notion of display independent pixels (called points) and pixel multipliers (that @2x/@3x suffix).

## Device details
|Device  |Class|PPI|Pixel multiplier |height (points)|width (points)|height (pixels)|width (pixels)|
|-------|---|-----------|----|------------------|----|----|----|
|iPhone 3/3GS  |low  |163|@1x |480 |320 |480 |320|
|iPhone 4/4s  |high  |326<sup>(1)</sup>|@2x |480 |320 |960 |640 |
|iPhone 5/5c/5S  |high  |326|@2x |568 |320 |1136 |640 |
|iPhone 6  |??  |326|@2x |667 |375 |1334 |750 |
|iPhone 6+<sup>(2)</sup> |??  |401|@3x |736 |414 |2208 |1242 |
|iPad 1-3  |low  | |@1x |1024 |768 |1024 |768 |
|iPad 4, Air  |high  |264 |@2x |1024 |768 |2048 |1536 |
|iPad Mini    |low  |163 |@1x |1024 |768 |1024 |768 |
|iPad Mini 2,3|high |326 |@2x |1024 |768 |2048 |1536 |
|iPad Pro<sup>(3)</sup>| ?? | 264 |@2x |? |? |2732 |2048 |


<sup>(1)</sup> some references say the iPhone 3 - 6 all have a 163 PPI display, while other sources give the data above.<br/>
<sup>(2)</sup> actual display is downsampled to 1080 x 1920, see http://www.paintcodeapp.com/news/iphone-6-screens-demystified for more info<br/>
<sup>(3)</sup> iPad Pro specs from http://www.imore.com/ipad-pro-specs The pixel multiplier is just my guess based on the PPI.

# Generating more data

Please help generate data for this table. Fork the repo, determine your device specifics, make your change, and submit a PR.

### Appcelerator Titanium

```js
// FOR ANDROID drop this into your app/alloy.js file or Resources/app.js
// while it will work for iOS, it doesn't output all the necessary
// info for the above table
Ti.API.info('displayCaps: '+JSON.stringify(Ti.Platform.displayCaps));

// or more to get just the info as in the table here:
var densities = {
  low: 'ldpi',
  medium: 'mdpi',
  high: 'hdpi',
  xhigh: 'xhdpi',
  xxhigh: 'xxhdpi',
  xxxhigh: 'xxxhdpi'
};
Ti.API.info('Density class: ' + densities[Ti.Platform.displayCaps.density]);
if(Ti.Platform.osname == 'iphone') {
  Ti.API.info('Density: ' + Ti.Platform.displayCaps.density);
} else {
  Ti.API.info('Logical density factor: ' + Ti.Platform.displayCaps.logicalDensityFactor);
}
Ti.API.info('DPI: ' + Ti.Platform.displayCaps.dpi);
Ti.API.info('Height: ' + Ti.Platform.displayCaps.platformHeight);
Ti.API.info('Width: ' + Ti.Platform.displayCaps.platformWidth);
// ready for cutting and pasting into your fork/PR of this repo
Ti.API.info('|model_name|' +
	 (Ti.Platform.displayCaps.logicalDensityFactor || Ti.Platform.displayCaps.density) + '|' +
	 densities[Ti.Platform.displayCaps.density] + '|' +
	 Ti.Platform.displayCaps.dpi + '|' +
	 Ti.Platform.displayCaps.platformHeight + '|' +
	 Ti.Platform.displayCaps.platformWidth + '|'
);
```

# Acknowledgments

The seed of the idea and the starting point data for this came from http://qualitytestingtips.blogspot.com/2013/08/ldpi-mdpi-hdpi-xhdpi-xxhdpi.html with additional data from the Titans, particularly https://gist.github.com/iotashan/4a6a347547a9c49a3a68

Many thanks to @paulvi for his help in adding details and clarity to this reference.

License: MIT

(it's just facts, so can't be copyrighted or protected really, not that I want to. so have at it, do what you want with it.)

