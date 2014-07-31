Chart Types: Rides view (Version 3.1)
***

The 'Rides' view provides 'Chart Types' which work on a single ride. The ride in focus can be selected in various ways, e.g. through the 'Side Bar' -> 'Rides' pane, but also by selecting a ride on the 'Navigator' or 'Calendar' on the 'Diary' view.

* [Ride Summary] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Rides#ride-summary)
* [Details] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Rides#details)
* [Summary and Details] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Rides#summary-and-details)
* [Editor] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Rides#editor)
* [Performance] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Rides#performance)
* [Critical Mean Maximals - similar to 'Trends View' - for a single ride] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#critical-mean-maximal)
* [Distribution / Histogram - similar to 'Trends View' - for a single ride] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#distribution--histogram)
* [Pedal Force vs Velocity] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Rides#pedal-force-vs-velocity)
* [Heartrate vs Power] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Rides#heartrate-vs-power)
* [Google Map / Bing Map] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Rides#google-map--bing-map)
* [2d Plot] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Rides#2d-plot)
* [3d Plot] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Rides#3d-plot)
* [Aerolab Chung Analysis] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Rides#aerolab-chung-analysis)

## Ride Summary
A summary chart is chart with fixed structure, which displays a summary about the current ride you a looking at.

* Contents Section are:
  *Totals, Average, Maximums, Metrics, Model information - the 'Metrics' shown are configurable through 'Preferences' -> 'Metrics' -> 'Summary'
* Power Zones - the power zones as configured in 'Preferences' for the date the ride took place
* Heart Rate Zones - the heart rate zones as configured in 'Preferences' for the date the ride took place

## Details

The ride 'Details' allow to view, change and enter ride specific data. Some of the fields are pre-populated with ride file data (e.g. 'Start Date' and 'Start Time').

The content of the 'Details' base on the configuration done in [Preferences->Data Fields] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Preferences_Data%20Fields#fields)

Here the 'Workout' Tab as an example to show the relationship:

![Ride Details - Workout Tab] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Ride_Details-Workout.jpg)

![Ride Details - Workout Settings] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Ride_Details-Workout-Config.jpg)

Important to know is: The sequence of the 'Tab's on the 'Details' screen and the sequence of the field per 'Tab' is the sequence of the configuration list. When adding or removing a field to the configuration, GoldenCheetah needs a few seconds to re-check / adjust it's interal structures and to re-create the screens (by adding the new field). 

_Note: GoldenCheetah comes with a set of field preferences, which already contain a number of additional fields for ride specific data, as well as a proposal on field for the 'Metric' tab. Since for some of these field specific logic is implemented in GoldenCheetah, it is clearly NOT recommended to remove any of the pre-defined fields._

## 'Metric' Tab

The 'Metric' tab is pre-populated with a number of metrics (as defined in the 'Preferences->Data Fields'). 

![Ride Details - Metric] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Ride_Details-Metric.jpg)

To enter or overwrite a 'Metric' value, please check the check-box next to the metric to open an input field for this metric. Only if you then input a value - different to '0' - the value will be taken as the metric value for this ride.

## 'Extra' Tab

The 'Extra' Tab is a set of 'Read Only' fields, which are automatically generated based on you configuration. You do not find the 'Extra' Tab in the list of 'Tabs' in 'Preferences->Data Fields', but you find field like 'Calendar Text' or 'Data' in the list (without an explicite 'Tab' assigned).

![Ride Details - Extra] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Ride_Details-Extra.jpg)
 
Some important fields are explained here
* 'Calendar Text' - generated text which also appears in the 'Diary' view - 'Calendar' chart
* 'Change History' - log of changes done to the ride file
* 'Data' - info which data series are available for the ride
*  ... other fields are self-explanatory

## Summary and Details

Combines [Summary] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Rides#ride-summary) and [Details] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Rides#details) in one chart.

## Editor

The 'Editor' chart provides all the ride file details in a list format. The default view contains columns for all data series captured from your head-unit, as well as any data series derived.

As the name states, it does not only display the data, but you can also 'Edit' the data here. The multiple options available in the 'Editor' chart are described here:

![Editor - Complete View]  (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Ride_Editor-View.jpg)

### Icon Functions

![Editor - Icons] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Ride_Editor-Icons.jpg)

* `Save` - Saves the ride
* `Undo` - if active, there have been changes to the ride series data (as shown in the editor), those changes are reverted - if there are multiple changes done separately - then can be undone separately by presssing 'Undo'
* `Redo` - if active, you have been 'Undo'ing changes - they can be re-applied be 'Redo'
* `Find` - opens a 'Search' dialog box - which can search for values in the series data, you can define search rules, the values to search and the data series where to search. As a result you get the list of search hits in the dialog box and the values fulfilling the search are marked in the 'Editor' data list. "Mouse-Click" on a result line in the dialog box, moves the data view to this hit.
* `Anomalies` - when choosing, GoldenCheetah does consistency check on the available data points / data series. The checks performed and their messages are:
  * 'Invalid recording gap' - there is a gap in recording of more than 1 seconds (gap)
  * 'Distance goes backwards' - like the description says
  * 'Suspiciously high cadence' - cadence detected is above 150
  * 'Suspiciously high heartrate' - heartrate detected is above 200
  * 'Suspiciously high speed' - speed detected is above 100 
  * 'Out of bounds value' - either latitude or longitude have invalid values 
  * 'Non-zero torque but zero cadence' - like the description says
  * 'Data spike candidate' - uses the 'Fix Power Spikes...' analysis and configuration settings to find power data spikes

'Anomalies' are listed in a 'Dialog box' - "Mouse-Click" on a text line in the dialog box, moves the data view to this anomaly.

## First Column - Context Menu

![Editor - First Column Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Ride_Editor-Context_1st_Column.jpg)

* `Undo`, `Redo` - see above

***

* `Cut` - cuts the marked data section to the clipboard - 'Cut' is only available if you have marked COMPLETE rows
* `Copy` - copies the marked data section to the clipboard - 'Copy' works for any selecton of cells
* `Paste` - pastes the clipboard data at choosen place - 'Paste' does not care for data consistency - (e.g. you can past power values to the latitude cell
* `Paste Special` - is aimed to paste data from outside GoldenCheetah (e.g. from an Excel Spreadsheet) to a data series, you have different settings to tell GoldenCheetah how this data is structured (quite similar to 'Past Special' features in other software products)
* `Clear Contents` - sets the cell in the marked data section to '0'

***

* `Delete Row` - delete the current or the selected range of rows
* `Insert Row` - inserts an emtpy row at the current selection

## Column Header - Context Menu

![Editor - Column Header Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Ride_Editor-Context_Header_Row.jpg)

* `Undo`, `Redo` - see above

***

* `Cut`, `Copy`, `Paste`, `Paste Special`, `Clear Contents` - see above

***

* `Remove Column` - remove the selected column 
* `Add Column` - opens a list of the available columns - only those columns not yet on the editor chart can be added


## Data area - Context Menu

![Editor - Data area Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Ride_Editor-Context_Data.jpg)


* `Undo`, `Redo` - see above

***

* `Cut`, `Copy`, `Paste`, `Paste Special`, `Clear Contents` - see above

***

* `Smooth Anomaly` - re-calculates the value of the selected cell as the average of the neighbors (previous and next data point in time) 


## Performance

This chart type provides all the graphs for your ride data series. In addition to data series which are captured by the head-unit directly, GoldenCheetah also delivers some derived series like 'Delta' series.

![Performance] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Performance-Overview.jpg)

* Basic Settings
  * `Shading` - here you select if, and how your power data curve is shown
  * `X-Axis `- either plot the ride 'by time' or 'by distance' on the X-Axis
  * `Smooth` - smoothes the graphs - the value set here is used for all curves 

* View Settings
  * `Stack`, `By Series`
      * if 'Stack is NOT checked -  the 'By Series' setting is ignored and all curves are plotted in one diagram
     * if 'Stack' is checked and 'By Series' is checked - all curves are plotted in separate diagrams one above the other
      * if 'Stack' is checked and 'By Series' is NOT checked - all curves are plotted in one diagram, and the X-Axis is streched over multiple lines
 
  * `Stack Zoom `- zooms the Y-Axis sizes for all diagrams if 'Show Stack' is checked
  * `Full Plot` - if checked, in addition to the curves, an additiona diagram, containing all the curves coming for 'Data Series' is displayed at the lower border of the 'Rides' view - with this you also get the ability to zoom into the X-Axis - the button for zooming are below the 'Full Plot' curve
  * `Overlay` - if checked, it adds a small overlay window to the diagram, in which selected interval data is displayed
  * `Grid` - if checked, it adds a grid to the chart

* Data series settings
  * `Delta Series `- prefined delta series (calculated as '(Current_data_point_Value - Previous_data_point_Value) / (Time_between_the_data_points)')
  * `Left/Right `- Left leg / Right leg dependent data series (only provided by some powermeter / head-unit combinations today)
  * `Data Series `- you can check the data series available from your head unit
  * `Metrics` - metrics which use the source data to calculate data along the complete ride

## Special Features for the 'Performance' chart

* references line (creation only in 'Stacked' mode, but visible on both
* scaling Y-Axis (only in 'Stacked' mode
* mouseover on Y-Axis in non-stacked mode
* marking intervals
* mouseover on curve for details





## Critical Mean Maximals

[Similar to 'Trends View' - for a single ride] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#critical-mean-maximal)

## Histogram

[Similar to 'Trends View' - for a single ride] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#distribution--histogram)

## Pedal Force vs Velocity

![Pedal Forcs vs Velocity] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/PedalForce_vs_Velocity.jpg)


## Heartrate vs Power

![HR vs Power] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/HR_vs_Power.jpg)


## Google Map / Bing Map

If GPS data is available, the ride is shown on a Google Map, or a Bing Map. You need to be connected to the internet.

The functionality provided on the maps differs on what Google or Bing are delivering (e.g. other views, zoom, rotate). GoldenCheetah itself adds capabilities to:

* Show Start/End point - special icons for start/end point of track appears
* Show Intervals - by marking one or more interval in the 'Side Bar'- 'Intervals' pane, the part of the track belonging to the intervals is 'highlighted'. The start points of all intervals are always marked in a track - and you can also 'Mouse-Click' on the markers to 'highlight' and interval (only for Google).
* Color - the color of the track gives an indication about the Power Zone you have been riding a certain track - colors are the same like in the color shading of the power-graphs 

## 2d Plot

The '2d Plot' - also called 'Scatter Plot' display the ride data as a collection of points, each having the value of data series determining the position on the X-Axis and the value of the other data series determining the position on the Y-Axis.

![2d Plot] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/2d_Plot.jpg)

* `X-Axis` - drop-down list box with the available data series (e.g. Power,...)
* `Y-Axis` - drop-down list box with the available data series (e.g. Power,...)
* 


## 3d Plot

![3d Plot] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/3d_Plot.jpg)



## Aerolab Chung Analysis

The 'Aerolab' chart provides a tool to use the Robert Chung's Virtual Elevation method to derive CdA and CRR from a power file. 

![Aerolab] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Aerolab.jpg)

For the theory on this, sample test protocols for the power file, please search for the tool and/or the method using a common search engine on the Web. There are many very good description out. So no reason to re-write all this to incorporate in the Wiki.


BACK: [Chart Types: General] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_General)