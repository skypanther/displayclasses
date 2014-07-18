Display Classes
==============

Android display classes and screen sizes

# Device details
|Brand / Device  |Class|PPI|logicalDensityFactor |platformHeight|platformWidth|
|-------|---|-----------|----|------------------|----|----|----|
|Google Nexus One  |hdpi  |252| | | |
|Google Nexus S  |hdpi  |233| | | |
|Google Nexus 7 2012  |hdpi  |216|1.331250072| | |
|Google Nexus 7 2013  |xhdpi  |323|2 |1920 |1104 |
|Google Nexus 4  |xhdpi  |318| | | |
|Google Nexus 10  |xhdpi  |299| | | |
|HTC Wildfire  |mdpi  |125| | | |
|HTC Desire  |hdpi  |252| | | |
|HTC Desire S  |hdpi  |252| | | |
|HTC Sensation  |hdpi  |256| | | |
|HTC Desire X  |hdpi  |233| | | |
|HTC One S  |hdpi  |256| | | |
|HTC One V  |hdpi  |252| | | |
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
|Samsung Galaxy Y  |ldpi  ||0.75 | | |
|Samsung Galaxy Ace  |mdpi  |165| | | |
|Samsung Galaxy S  |hdpi  |233| 1.5| | |
|Samsung Galaxy S2  |hdpi  |240|1.5 |800 |480 |
|Samsung Galaxy S3  |xhdpi  |320|2 |1280|720 |
|Samsung Galaxy S4  |xxhdpi  |440|3|1920|1080|
|Samsung Galaxy S5  |xxhdpi  |432|3| | |
|Samsung Galaxy Nexus  |xhdpi  |316|2| | |
|Samsung Galaxy Tab 10 inch tablet  |mdpi  |149|1 |1280 |800 |
|Samsung Galaxy Tab 2 10 inch tablet  |mdpi  |149| | | |
|Samsung Nexus 10 inch tablet  |xhdpi  |299| | | |
|Samsung Note  |xhdpi  |285| | | |
|Samsung Note 2  |xhdpi  |267| | | |
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

# Generating more data

Please help generate data for this table. Fork the repo, determine your device specifics, make your change, and submit a PR.

### Appcelerator Titanium

    // drop this into your app/alloy.js file or Resources/app.js
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
    Ti.API.info('Logical density factor: ' + Ti.Platform.displayCaps.logicalDensityFactor);
    Ti.API.info('DPI: ' + Ti.Platform.displayCaps.dpi);
    Ti.API.info('Height: ' + Ti.Platform.displayCaps.platformHeight);
    Ti.API.info('Width: ' + Ti.Platform.displayCaps.platformWidth);
    // ready for cutting and pasting into your fork/PR of this repo
    Ti.API.info('|model_name|' +
         densities[Ti.Platform.displayCaps.density] + '|' +
         Ti.Platform.displayCaps.dpi + '|' +
         Ti.Platform.displayCaps.logicalDensityFactor + '|' +
         Ti.Platform.displayCaps.platformHeight + '|' +
         Ti.Platform.displayCaps.platformWidth + '|'
    );

# Acknowledgments

The seed of the idea and the starting point data for this came from http://qualitytestingtips.blogspot.com/2013/08/ldpi-mdpi-hdpi-xhdpi-xxhdpi.html with additional data from the Titans, particularly https://gist.github.com/iotashan/4a6a347547a9c49a3a68

License: MIT

(it's just facts, so can't be copyrighted or protected really, not that I want to. so have at it, do what you want with it.)

