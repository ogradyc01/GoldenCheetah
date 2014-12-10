Menu Bar: Activity (Version 3.1)
***

![Activity Menu] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/MenuBar_Activity.jpg)

GoldenCheetah uses the term "Activity" and "Ride" in a mostly similar way. This is because the main functionality of GoldenCheetah is aimed to analyse ride data (with power). One more term to introduce here is "Workout" - a workout is a prescribed activity plan (e.g. 3x5 minutes at L5).

So most of the functions in this menu relate to rides. Here the list:

* `Download from device...` [explained here] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_310_First-Steps_Download-or-import)
* `Import from file...` [explained here] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_310_First-Steps_Download-or-import#importing-from-a-file)
* `Manual ride entry...` - Opens a dialog box to manually create a ride in Golden Cheetah. You can set a number of metrics and metadata. The stress figures can either be estimated or manually entered.

***

* `Export...` - Opens a dialog box to export the currently selected ride. You can choose the directory and the file format - _Note: The file formats are implemented to best knowledge - but since formats evolve or other software does different interpretation there is a risk, that exported files cannot be interpreted, even if the software claims to be able to read a particular format._
* `Batch export...` - In addition to "Export..." allows the selection of multiple files to be exported.
* `Export Metrics as CSV...` - Exports the metric database into a CSV file. _Note: The metric database is a SQLite database - which can also be read by appropriate SQLite tools. Any manipulation of the data from outside GoldenCheetah is not recommended/supported._

***

* `Upload/Download` [Special Topics: Upload_Download to_from external web-sites] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_310_Special Topics_Upload_Download to_from external web-sites)

***

* `Save ride` - does what is says. Important to know - metrics are only updated, once the ride is saved and only based on saved data. _Note: When closing GoldenCheetah, the system checks if are still any changed but unsaved rides and shows those in a dialog box - offering to save, discard or going back to GoldenCheetah._
* `Delete ride...` - deletes the ride after confirmation in a dialog popup. _Note: Any deleted rides are really deleted - GoldenCheetah does not provide an "un-delete" or "history" function here._
* `Split ride...` - opens the split ride wizard, which searches for breaks in an ride and then allows to split the ride into separate rides. (Useful when forgetting to stop recording.)
* `Merge rides...` - opens the merge ride wizard, which allows to merge two different files from the same ride into a single file. (Useful when having 2 different recordings - e.g from 2 devices and you want to merge the data into one ride).

BACK: [Menu Bar: Functions] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_310_Menu-Bar_Functions)
