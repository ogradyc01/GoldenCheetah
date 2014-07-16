Side Bar: Rides view (Version 3.1)
***

![SideBar General] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/SideBar_Rides.JPG)

The 'Side Bar' for the 'Diary' view offers two different panes - als illustrated above.

* [Calendar] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Rides-view#calendar)
* [Rides] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Rides-view#rides)
* [Intervals] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Rides-view#intervals)

***

## Calendar

The calendar allows to select the ride, you want to investigate by "clicking on it", as well as monthly "scrolling" through your data. Days for which rides exist, are colored as defined preferences `Options->Data Fields->Notes Keywords`. 

## Rides

The rides pane shows all rides which have been uploaded to GoldenCheetah for the specific athlete. It offers multiple functions to sort, group - but also functions which are as well available through 'Menu Bar' functions.

### Rides - main functions

![Rides - menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/SideBar_Rides-Rides_Menu.jpg)

* Delete Ride - same like `Menu Bar->Activity->Delete Ride...`
* Split Ride -  same like `Menu Bar->Activity->Split Ride...`
* Upload Ride to Calendar - same like 'Menu Bar->Tools->Upload Ride to Calendar'
* Find Intervals... - opens a dialog with criteria to find intervals for a ride (details see 'Intervals' section on this WiKi page)
***
* Show Column Chooser - opens a screen which contains all available fields for a ride. You can "drag&drop" the fields to the column header of the 'Rides' pane to add additional columns here (details see 'Rides - column header' section of this Wiki page)
* Group By -> <List of visible column> - you can group your rides by each of the fields - depending on the field type grouping is realized to produce senseful groupings of a field (just try it out). Grouping is only supported for one field at a time - when you have grouped, you need to "ungroup" first before choosing a different field. The "ungroup" is at the same menu position than grouping.
* Expand All - if you have collapsed the rides within a single group or by using 'Collapse All' - this function makes them all visible again
* Collapase All - this function hides all rides for the different groups and you will only see the group headers

_Note: Could can also collapse and expand the rides for a single group, by "double-click" in the group header._

### Rides - column header

![Rides - columns] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/SideBar_Rides-Rides_Columns.jpg)

When you open the context menu on the column header of the 'Rides' pane, you have three options:

* Remove Column - does what it says - removes the choosen column from the rides pane
* Show in groups - does the same like "Group By->...." as explained above for choosen column 
* Column Chooser - opens a screen which contains all available fields for a ride. You can "drag&drop" the fields to the column header of the 'Rides' pane to add additional columns here. Any new column added will appear most left on the rides pane. You can also re-order and resize the columns.

![Rides - add columns] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/SideBar_Rides_Columns_Add_Column.gif)

Here the re-ordering and resizing in more detail:

![Rides - move/resize columns] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/SideBar_Rides_Columns_Move_Resize.gif)

## Intervals

Depending which source data format you are using, you might or might not have interval pre-defined with every ride after the upload. (E.g. for Garmin - FIT the Laps defined during your ride are created as 'Intervals' in GoldenCheetah).

![Intervals - Overview] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/SideBar_Rides-Intervals_Overview.jpg)

The interval pane has two areas - the list of intervals and the interval data. The fields shown in the data section are defined in your preferences `Options->Metrics->Intervals`.

![Intervals - Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/SideBar_Rides-Intervals_Menu.jpg)

The intervals menu offers the following functions:

* Find Intervals... - explained in the separate section below
* Sort Intervals - sorts the intervals 'by starting time'
***
* Zoom to interval / Zoom out - shows the interval in detail and the full ride in the 'Main View' - 'Ride' chart

![Intervals - Zoom] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/SideBar_Rides-Intervals_Zoom.gif)

* Edit Interval - opens a dialog to edit interval details:

![Intervals - Edit] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/SideBar_Rides-Intervals_Edit_Interval.jpg)

* Delete Interval - remove the interval from the ride




### Intervals - find intervals



BACK: [Side Bar: General] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_General-handling)