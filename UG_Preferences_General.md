Preferences: General (Version 3.2)
***

_Select:_ `Menu Bar -> Tools -> Options...` to get to the 'Options' Popup.

Here you configure central parameters which are used by GoldenCheetah in different places. 

![Preferences General](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/PreferencesGeneral.jpg)

*  `Language` - this is the language the GoldenCheetah UI comes up. When changing the language this is only taking effect with the next start of GoldenCheetah. When you start GoldenCheetah for the first time on your PC, the system locale (usually the language your operating system is set up) is used as default.

_Note: GoldenCheetah is translated into multiple languages, which you find on the drop-down list. In case texts are not translated for a certain language GoldenCheetah uses the 'English' default texts._

* `Unit` - this is the Unit of Measurement (Metric or Imperial), which is used across GoldenCheetah (for all Athletes) in metrics calculation and display

* `Use Garmin Smart Recording / Smart Recording Threshold (sec)` - Garmin devices have a feature called 'Smart Recording', where data points are not stored per second, but in variable intervals. In order to read such files and understand how to handle the gaps, GoldenCheetah can fill such gaps (by interpolating the missing data points). To enable this you need to activate 'Use Garmin Smart Recording' and defined the threshold (in seconds) upto which GoldenCheetah shall consider a data gap to be a smart recording gap - which then is filled. If 'Use Garmin Smart Recording' is off - gaps are filled with 'Zero' values.

_Note: A recommendation is NOT too use any of such smart-recording features. Constant recording is the best way to obtain proper analysis results - not only on GoldenCheetah, but also in other analysis tools_

* `Elevation hysteresis (meters)` - this value is used to smooth the small changes in altitude. The default value is 3m. Since different programs use different hysteresis values, the elevation calculated by GoldenCheetah and other programs most likely deviate. If such differences are important for you, you can adjust the hysteresis and try to reach the value of the other program. _Note: Since other programs might also deviate in the algorithm used, there is no guarantee to find a value which delivers the same result for all activities._

_Note: The value is defined for all athletes_

* `Athlete Library` - see detailed description here: [Setting the athlete library](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Special-Topics_Setting-the-athlete-library)

* `Workout Library` - Directory to store the 'Train' view related files,... 

BACK: [Preferences: Overview](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Preferences_Overview)

