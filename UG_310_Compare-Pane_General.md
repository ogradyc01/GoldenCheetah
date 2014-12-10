Compare Pane: General (Version 3.1)
***

The compare pane is a very powerful new feature of GoldenCheetah 3.1 - depending on the view you are on (Trends or Rides) it allows the comparison of 
* Date Ranges (Trends View) or 
* Rides and/or Intervals (Rides View) - which can even be mixed.

The handling of the compare pane is the same for both views, here the common concepts - based on a 'Rides' view example:

## Selection of data for comparison

The selection of data to be compared works in same way for 'Rides', 'Intervals' and 'Date Ranges'. It's a "Drag&Drop" concept - as shown below. You do not even need to open the 'Compare Pane', but just "Drag&Drop" the first item to compare to the bottom of the 'Main View':

![Compare Pane: Drag & Drop] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/ComparePane_DragDrop.gif)

_Note: You can select items ('Rides', 'Intervals' and 'Date Ranges') not only from the athlete you are currently working with, but also from other athletes - for this you need to open the other athlete in a separate window to be able to "drag&drop" items._

## ON/OFF, sorting and Clear 

* To activate the comparison the selected items ('Rides', 'Interval' or 'Date Ranges'), you need to push the `OFF` button in the 'Compare Pane'. With this the charts in the main view change into a comparison mode and the button changes to `ON`. Pressing the button again ends the compare mode.
* Using the 'Check boxes' on the left border of the 'Compare Pane' allow to include/exclude single items from the comparison. The first item is always checked as the comparison reference.
* You can also sort the items by 'mouse-click' on the respective column header. With the sort, also the reference items changes (but is always the first item in the list).
* The `Clear` button removes all items from list. 

_Note: Comparison views have been implemented for most of the charts - but only for those, where a comparison makes sense. E.g. there is no comparison for the Google/Bing map chart._

![Compare Pane] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/ComparePane_Pane.jpg)

## Columns in the compare pane

* Trends view - pre-defined columns are 'Athlete', 'From', 'To', 'Duration' and 'Distance'. The other data fields are those metrics defined in `Preferences->Data Fields->Summary`.
* Rides view - pre-defined columns are 'Athlete', 'Date', 'Time', 'Duration' and 'Distance'. The other data fields are those metrics defined in `Preferences->Data Fields->Intervals`.

BACK: [General UI] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_310_General_UI-Layout-and-terminology)


