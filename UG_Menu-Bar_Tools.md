Menu Bar: Tools (Version 3.2)
***

![Tools Menu](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/MenuBar_Tools.jpg)

The tools menu contains functions which either manipulate rides or relate to additional features GoldenCheetah is providing.

* `Options...` - only on Linux and Windows this opens the preferences pane. Since it is an application on it's own it will remain open, even when you have closed the main window. [Preferences Details](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Preferences_Overview)
* `CP and W' Estimator...` - opens a dialog to estimate your CP and W' based on a short and long power best. If 3 minutes and 20 minutes best are used the result aligns with Monod/Scherer algorithm. Other algorithms which are also available in GoldenCheetah are not supported by the Estimator now. 
* `Air Density (Rho) Estimator..`. opens a tool for estimation Air Density based upon temperature and air pressure. This is useful when working with Aerolab.

***

* `Get Withings Data...` - downloads all measure from your Withings weight scale. You need to configure your user id and public key in the [Preferences: Passwords]
(https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Special-Topics_Upload_Download-to_from-external-web-sites) section for this to work.

***
* `Create a new workout...` - opens a workout wizard to create a new "Train" view workout. 
* `Download workouts from ErgDB...` - opens a dialog to select and download "Train" view workouts from the internet ErgDB web-site.
* `Import workouts or videos ...` - opens a file dialog to select and import a workout or a video into your "Train" workout library.
* `Scan disk for videos and workouts...` opens a file dialog to scan directories for workouts and videos and import them into your "Train" workout library.

***

* `Upload Ride to Calendar` - will create a calendar entry to a CalDAV based calendar (e.g. Google Calendar). You need to configure and authorize the access in [Preferences: Passwords](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Special-Topics_Upload_Download-to_from-external-web-sites).
* `Refresh Calendar` - will read entries from your CalDAV calendar to display on the calendar view. Configuration is the same is in the "Upload Ride to Calendar" function.
* `Create Heat Map` - create a HTML showing a heat map of the selected rides on a map - the HTML is created for use outside GoldenCheetah under the name "HeatMap.htm" - the folder can be chosen in the creation dialog box.
* `Export Metrics as .CSV` - exports the available metrics data for all rides as .CSV file for external processing

***

* `Find intervals...` - opens a dialog to find intervals in the current ride. The same functionality is also available from the "Side Bar: Intervals" view. 

BACK: [Menu Bar:Functions](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Menu-Bar_Functions)