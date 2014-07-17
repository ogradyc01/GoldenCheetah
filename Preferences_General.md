Preferences: General (Version 3.1)
***

_Select:_ `Menu Bar -> Tools -> Options...` to get to the 'Options' Popup.

Here you configure several important parameters which are used by GoldenCheetah in different places. 

![Preferences General] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/PreferencesGeneral.jpg)

* Language: This is the language the GoldenCheetah UI comes up. When changing the language this is only taking effect with the next start of GoldenCheetah. When you start GoldenCheetah for the first time on your PC, the system locale (usually the language your operating system is set up) is used as default.

_Note: GoldenCheetah is translated in multiple languages, which you find on the drop-down list. In case texts are not translated for a certain language GoldenCheetah uses the 'English' default texts._

* Crank Length: Is an important parameter for some of the metrics calcated in GoldenCheetah. So maintain carefully.

_Note: As of today the Crank Length is defined for all users and not individual per user._

* Wheelsize: is the default value for the wheelsize use in the 'Train' view (e.g. if not device specific wheelsize is configured) - and the wheelsize used in 'Train' view where not specific wheelsize can be configured

* Use Garmin Smart Recording / Smart Recording Threshold (sec): Garmin devices have a feature called 'Smart Recording', where data points are not stored per second, but in variable intervals. In order to read such files and understand how to handle the gaps, GoldenCheetah can fill such gaps (by interpolating the missing data points). To enable this you need to activate 'Use Garmin Smart Recording' and defined the threshold (in seconds) upto which GoldenCheetah shall consider a data gap to be a smart recording gap - which then is filled. If 'Use Garmin Smart Recording' is off - gaps are filled with 'Zeroes'.

* Elevation hysteresis (meters): This value is used to smooth the small changes in altitude. The default value is 3m. Since different programs use different hysteresis values, the elevation calculated by GoldenCheetah and other programs deviate. If such differences are important, you can adjust the hysteresis.

_Note: The value is defined for all users._

* STS average (days) / LTS average (days): STS (Short Term Stress) and LTS (Long Term Stress) days are the time constants used in the calculation of STS and LTS in the PMC charts 

_Note_: STS and LTS value is stored per user. 

* PMC Stress Balance Today: If flaged, the training of a certain day is considered in the SB value of this day already. If not flaged, the SB change would take effect on the next day. 

* Athlete Library: See detailed description here: [Setting the athlete library](https://github.com/GoldenCheetah/GoldenCheetah/wiki/Special-Topics:-Setting-the-athlete-library)

* Workout Library: Directory to store the 'Train' view related files,... 



