## This is a fork so that it can be published on jitpack

I did not change a single line of code (except for the errors I introduced myself), this is a fork for which i merged the pr from hilpitome

the original did not build, and the pull request fixing it never got merged so this is it

To make this work you need to change this

``` implementation 'com.emredavarci:circleprogressbar:1.0.4' ```

to this

``` implementation 'com.github.julian-oliveri:CircleProgressbar-JitPackFix:v1.0.2' ```

I wont be providing support for this but at least it compiles

## The original readme

# CircleProgressBar

![https://github.com/emre1512/CircleProgressBar](https://img.shields.io/badge/platform-Android-green.svg?style=flat-square)
![https://github.com/emre1512/CircleProgressBar](https://img.shields.io/badge/API-16+-orange.svg?style=flat-square)
![https://www.apache.org/licenses/LICENSE-2.0](https://img.shields.io/badge/licence-Apache%20v2.0-blue.svg?style=flat-square)
![https://github.com/emre1512/CircleProgressBar](https://img.shields.io/badge/version-v1.0.4-ff69b4.svg?style=flat-square)

A simple library for creating circular progressbars for Android.

## Examples

![](https://media.giphy.com/media/l0EoBe4BwiR8MIKXu/giphy.gif)

## Installation

- Get it via gradle: ``` implementation 'com.emredavarci:circleprogressbar:1.0.4' ```
## Usage

1) Add CircleProgressBar to your layout

```xml
    <com.emredavarci.circleprogressbar.CircleProgressBar
    	xmlns:cpb="http://schemas.android.com/apk/res-auto"
        android:id="@+id/progressBar"
        android:layout_width="150dp"
        android:layout_height="150dp"
        cpb:progressColor="#e76130"
        cpb:backgroundColor="#e7b330"
        cpb:dimension="14"
        cpb:backgroundWidth="8"
        cpb:textSize="18sp"
        cpb:roundedCorners="true"
        cpb:suffix="%"
        cpb:prefix=""
        cpb:progressText="Loading..."
        cpb:maxValue="100"
        cpb:progressTextColor="#f9916b"/>
```

2) Get it from your activity/fragment etc.

```java
	CircleProgressBar progressBar = (CircleProgressBar) findViewById(R.id.progressBar);
	progressBar.setProgress(progress1);
```

You can modify it programmatically if you want

<b>Setters</b>

```java
	progressBar.setProgress(progress); 		// set progress value
	progressBar.setMaxValue(100); 			// set progress max value
	progressBar.setStrokeWidth(10); 		// set stroke width
	progressBar.setBackgroundWidth(10); 		// set progress background width
	progressBar.setProgressColor("#FF6FD99D"); 	// set progress color
	progressBar.setBackgroundColor("#FFF9916B"); 	// set progress backgorund color
	progressBar.setText(String.valueOf(progress)); 	// set progress text
	progressBar.setTextColor("#FF6FD99D"); 		// set text color
	progressBar.setSuffix("%"); 			// set suffix
	progressBar.setPrefix(""); 			// set prefix
```

<b>Getters</b>

```java
	progressBar.getProgress();			// get progress value
	progressBar.getProgressPercentage();		// get progress percentage
	progressBar.getMaxValue();			// get progress max value
	progressBar.getStrokeWidth();			// get stroke width
	progressBar.getBackgroundWidth();		// get progress background width
	progressBar.getProgressColor();			// get progress color
	progressBar.getBackgroundColor();		// get progress backgorund color
	progressBar.getText();  			// get progress text
	progressBar.getTextColor();			// get text color
	progressBar.getSuffix();			// get suffix
	progressBar.getPrefix();			// get prefix
```

## LICENSE

Copyright 2017 M. Emre Davarci

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.






