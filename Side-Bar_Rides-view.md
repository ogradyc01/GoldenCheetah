Side Bar: Rides view (Version 3.1)
***

![SideBar General] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/SideBar_Rides.JPG)

The 'Side Bar' for the 'Rides' view offers three different panes - as illustrated above.

* [Calendar] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Rides-view#calendar)
* [Rides] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Rides-view#rides)
* [Intervals] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Rides-view#intervals)

***

## Calendar

The calendar allows to select the ride you want to investigate by "clicking on it", as well as monthly "scrolling" through your data. Days for which rides exist, are colored following the preferences `Options->Data Fields->Notes Keywords` color rules. 

## Rides

The rides pane shows all rides which have been uploaded to GoldenCheetah for the specific athlete. It offers multiple functions to sort, group - and also functions which your can also reach through 'Menu Bar' functions.

### Rides - main functions

![Rides - menu] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/SideBar_Rides-Rides_Menu.jpg)

* `Delete Ride` - same like `Menu Bar->Activity->Delete Ride...`
* `Split Ride` -  same like `Menu Bar->Activity->Split Ride...`
* `Upload Ride to Calendar` - same like 'Menu Bar->Tools->Upload Ride to Calendar'
* `Find Intervals...` - opens a dialog box with criteria to find intervals for a ride (details see 'Intervals' section on this Wiki page)
***
* `Show Column Chooser` - opens a screen which contains all available fields for a ride. You can "drag&drop" the fields to the column header of the 'Rides' pane to add additional columns here (details see 'Rides - column header' section of this Wiki page)
* `Group By -> <List of visible column>` - you can group your rides by each of the fields - depending on the field type different grouping logic is implemented to produce useful groupings results (just try it out). Grouping is supported for one field at a time - when you have grouped, you need to "ungroup" first before choosing a different field. The "ungroup" is at the same menu position like grouping.
* `Expand All` - if you have collapsed the rides within a single group or by using 'Collapse All' - this function makes them all visible again
* `Collapse All` - this function hides all rides for the different groups and you will only see the group headers

_Note: You can also collapse and expand the rides for a single group, by "mouse double-click" in the group header._

### Rides - column header

![Rides - columns] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/SideBar_Rides-Rides_Columns.jpg)

When you open the context menu on the column header of the 'Rides' pane, you have three options:

* `Remove Column` - does what it says - removes the selected column from the rides pane
* `Show in groups` - does the same like "Group By->...." as explained above for selected column 
* `Column Chooser` - opens a dialog box which contains all available fields for a ride. You can "drag&drop" the fields to the column header of the 'Rides' pane to add additional columns here. Any new column added always appears as most left column on the rides pane. You can also re-order and resize the columns.

![Rides - add columns] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/SideBar_Rides_Columns_Add_Column.gif)

Here the re-ordering and resizing in more detail:

![Rides - move/resize columns] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/SideBar_Rides_Columns_Move_Resize.gif)

## Intervals

Depending which source data format you are using, you might or might not have intervals pre-defined for your ride(s) after importing/uploading. (E.g. for Garmin - .FIT the Laps created in a ride are created as 'Intervals' in GoldenCheetah).

![Intervals - Overview] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/SideBar_Rides-Intervals_Overview.jpg)

The interval pane has two areas - the list of intervals and the interval data. The fields shown in the data section are defined in your preferences `Options->Metrics->Intervals`.

![Intervals - Menu] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/SideBar_Rides-Intervals_Menu.jpg)

The intervals menu offers the following functions:

* `Find Intervals...` - explained in the separate section below
* `Sort Intervals` - sorts the intervals 'by starting time'
***
* `Zoom to interval / Zoom out` - shows the interval in detail and the full ride in the 'Main View' - 'Ride' chart

![Intervals - Zoom] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/SideBar_Rides_Intervals_Zoom.gif)

* `Edit Interval` - opens a dialog to edit interval details:

![Intervals - Edit] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/SideBar_Rides-Intervals_Edit_Interval.jpg)

* `Delete Interval` - removes the selected interval from the ride

_Note: The interval list allows "multi-selection" by using `SHIFT+Mouse-Click` or `CRTL+Mouse-Click`(on Windows 7 - other OS might use different keys for that). If you have selected multiple intervals, it depends on the function, if it's applied to all intervals, or only to the currently active intervals. E.g. 'Delete Interval' deletes ALL marked intervals, while 'Edit Interval" opens the dialog box for the interval currently marked by the mouse-cursor._


### Intervals - find intervals

There are multiple way to define intervals - one is to just mark the in the 'Main View' - 'Ride' chart with a "mouse-drag" - which then automatically creates an interval in the list (with a pre-defined name.)

The other way is to search for specific data to be analysed as intervals. The rules for finding intervals this way are configured in the 'Find Intervals..." dialog:

![Intervals - Edit] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/SideBar_Rides-Intervals_Find.jpg)

Since this dialog is mostly self-explanatory just a view details here:

* Choose a method first - 'Peak Power' or 'Ascent' or 'W'(Energy)' or 'Time/Distance'
* Enter the search criteria (which is different per method)
* Press `Find` to fill the 'Results' list
* Edit the 'Results' list by deselecting those entries you do NOT want to be added to your ride as an 'Interval'
* Press `Add to Ride`

And you will have set of new intervals (based on your criteria) available.

_Note: Interval information is stored with your ride data. So you need to save your ride if you want to keep you intervals._

BACK: [Side Bar: General] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_General-handling)