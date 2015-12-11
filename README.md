CircularFillableLoaders
=================

[![Platform](https://img.shields.io/badge/platform-android-green.svg)](http://developer.android.com/index.html)
[![API](https://img.shields.io/badge/API-15%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=15)
[![PayPal](https://img.shields.io/badge/paypal-donate-yellow.svg)](https://www.paypal.me/LopezMikhael)
[![Twitter](https://img.shields.io/badge/Twitter-@LopezMikhael-blue.svg?style=flat)](http://twitter.com/lopezmikhael)

This is an Android project allowing to realize a beautiful circular fillable loaders to be used for splashscreen for example.

USAGE
-----

To make a circular fillable loaders add CircularFillableLoaders in your layout XML and add CircularFillableLoaders library in your project.

XML
-----

```xml
<com.mikhaellopez.circularfillableloaders.CircularFillableLoaders
            android:id="@+id/circularFillableLoaders"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:src="@drawable/your_logo"
            app:border="true"
            app:border_width="12dp"
            app:progress="80"
            app:wave_amplitude="0.06"
            app:wave_color="#3f51b5" />
```

You must use the following properties in your XML to change your CircularImageView.


#####Properties:

* `app:progress`        (integer)   -> default 0
* `app:border`          (boolean)   -> default true
* `app:border_width`    (dimension) -> default 4dp
* `app:wave_color`      (color)     -> default BLACK
* `app:wave_amplitude`  (float)     -> default 0.05f (between 0.0 and 0.1)

JAVA
-----

```java
CircularFillableLoaders circularFillableLoaders = (CircularFillableLoaders)findViewById(R.id.yourCircularFillableLoaders);
// Set Progress
circularFillableLoaders.setProgress(60);
// Set Wave and Border Color
circularFillableLoaders.setColor(Color.RED);
// Set Border Width
circularImageView.setBorderWidth(10 * getResources().getDisplayMetrics().density);
// Set Wave Amplitude (between 0.00f and 0.10f)
circularFillableLoaders.setAmplitudeRatio(0.08);
```


LICENCE
-----

CircularImageView by [Lopez Mikhael](http://mikhaellopez.com/) is licensed under a [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0).
Based on a work at https://github.com/gelitenight/WaveView.
