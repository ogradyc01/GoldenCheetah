Preferences: Athlete (Version 3.2)
***

_Select:_ `Menu Bar -> Tools -> Options...` to get to the 'Options' Popup.

The athlete specific data allows to change the settings you have done when creating a new athlete and also completes them by setting up the 'Power' and 'Heartrate' zones for the athlete.

_Note: All on this view is stored for the current athlete._

![Preferences: Athlete - About](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/PreferencesAthlete.jpg)

![Preferences: Athlete - Measures](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/PreferencesAthlete_Measures.jpg)

![Preferences: Athlete - Auto Import](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/PreferencesAthlete_Autoimport.jpg)

In the `About` tab you can change some basic settings, and add a picture for the athlete (if you want to). To add a picture, just click on the 'picture' area to open a 'File Selector' dialog box. You can select image files of types (.png, .bmp, .jpg). If your file selector does not show any files, use the operating system dependent search syntax in the 'File Name' field. (e.g. in Windows its "*.*). When selecting a picture it's automatically loaded and copied to your athlete specific data in the 'Athlete Library'.

Fields which you have to maintain on this view are:

* `Weight` - set the default weight, which is used in metrics calculation and display

For 'Weight' please also check: [Special Topics: Weight settings](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Special-Topics_Weight-settings) 


* `Crank Length` - is an important parameter for some of the metrics calculated in GoldenCheetah. So maintain correctly. Known use is to calculate AEPF and CPV both in Scatter Plot and PfPv Plot. In PfPv Plot you can overwrite the value used to plot as required, in the Scatter Plot the preference is used.

_Note: As of today the Crank Length is defined for all athletes and not individual per athlete._

* `Wheelsize` - is the default value for the wheel size in GoldenCheetah used in the 'Train' view (e.g. if not a device specific wheel size is configured) - and the wheel size used in 'Train' view in (some) for which no explicite wheel size can be maintained


* `STS average (days) / LTS average (days)` - STS (Short Term Stress) and LTS (Long Term Stress) days are the time constants used in the calculation of STS and LTS in the PMC charts 

_Note_: STS and LTS values are stored per athlete._

* `PMC Stress Balance Today` - if checked, the training of a certain day is considered in the SB value of this day already. If not checked, the SB change will take effect on the next day. 

The next three tabs `Power Zones`, `Heartrate Zones`, and `Pace Zones` allow you to setup the training zones for the athlete. GoldenCheetah allows a time dependent and very flexible definition of zones for 'Power' and 'Heartrate' as well as the definition of 'Pace Zones' separate for 'Run' and 'Swim' activities. In this documentation we assume that you are familiar with the concepts behind training zones and will just explain how zones are configured.

The last tab `Auto Import` allows the configuration of a number of directory which are scan for activity/activity files when Golden Cheetah is started. When found, showing the list and automatically importing new activities to GoldenCheetah.

* [How-to: Configure Training Zones](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Preferences_Athlete_Training-Zones)

BACK: [Preferences: Overview](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Preferences_Overview)
