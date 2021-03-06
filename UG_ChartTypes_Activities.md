Chart Types: Activities view (Version 3.2)
***

The 'Activities' view offers 'Chart Types' which work on a single activity. The activity in focus can be selected in various ways, e.g. through the 'Side Bar' -> 'Activities' pane, but also by selecting a activity on the 'Navigator' or 'Calendar' on the 'Diary' view.

* [Activity Summary](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#activity-summary)
* [Details](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#details)
* [Summary and Details](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#summary-and-details)
* [Editor](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#editor)
* [Performance](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#performance)
* [Critical Mean Maximals - similar to 'Trends View' - for a single activity](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Trends#critical-mean-maximal)
* [Histogram](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#histogram)
* [Pedal Force vs Velocity](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#pedal-force-vs-velocity)
* [Heartrate vs Power](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#heartrate-vs-power)
* [Google Map / Bing Map](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#google-map--bing-map)
* [2d Plot](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#2d-plot)
* [3d Plot](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#3d-plot)
* [Aerolab Chung Analysis](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#aerolab-chung-analysis)

## Activity Summary
A summary chart has a fixed structure, which displays a summary about the current activity you a looking at.

* Contents Section are:
  * Totals, Average, Maximums, Metrics, Model information - the 'Metrics' shown are configurable through 'Preferences' -> 'Metrics' -> 'Summary'
* Power Zones - the power zones used are those valid for the date the activity took place - they are configured in 'Preferences' -> 'Athlete'
* Heart Rate Zones - the heart rate zones used are those valid for the date the activity took place - they are configured in 'Preferences' -> 'Athlete'

## Details

The activity 'Details' allow to view, change and enter activity specific data. Some of the fields are pre-populated based on the activity file data (e.g. 'Start Date' and 'Start Time').

The fields available in 'Details' are mainly determined by the configuration done in [Preferences->Data Fields](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Preferences_Data%20Fields#fields)

Here the 'Workout' Tab as an example to show the relationship between configuration and input fields:

![Activity Details - Workout Tab](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Activity_Details-Workout.jpg)

![Activity Details - Workout Settings](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Activity_Details-Workout-Config.jpg)

_Note: The sequence of the 'Tab's on the 'Details' screen and the sequence of the fields per 'Tab' is exactly the sequence of the field and tabs in the configuration. When adding a field to the configuration, GoldenCheetah needs a few seconds to re-check / adjust it's internal structures and to re-create the screens (by adding the new field)._

_Note: GoldenCheetah comes with a set of field preferences, which already contain a number of additional fields for activity specific data, as well as a proposal on fields for the 'Metric' tab. Since for some of these field specific logic is implemented in GoldenCheetah, it is NOT recommended to remove any of the pre-defined fields, as it might cause unexpected behavior._

## 'Metric' Tab

The 'Metric' tab is pre-populated with a number of metrics (as defined in the 'Preferences->Data Fields'). 

![Activity Details - Metric](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Activity_Details-Metric.jpg)

To enter or overwrite a 'Metric' value, please check the check-box next to the metric to open the input field for this metric. Only if you then input a value different to '0', this value will be taken as the metric value for this activity (and overwrite any value coming from your activity data).

## 'Extra' Tab

The 'Extra' Tab is a set of 'Read Only' fields, which are automatically generated based on your configuration. You do not find the 'Extra' Tab in the list of 'Tabs' in 'Preferences->Data Fields', but you find fields like 'Calendar Text' or 'Data' in the list (without an specific 'Tab' assigned).

![Activity Details - Extra](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Activity_Details-Extra.jpg)
 
Some important fields are:
* 'Calendar Text' - generated text which also appears in the 'Diary' view - 'Calendar' chart
* 'Change History' - log of changes done to the activity file
* 'Data' - info which data series are available for the activity (each character represents a data series)
  * 'T' - time
  * 'D' - distance
  * 'S' - speed
  * 'P' - power
  * 'H' - heart rate
  * 'C' - cadences
  * 'N' - torque
  * 'A' - altitude
  * 'G' - GPS
  * 'L' - slope
  * 'W' - wind speed
  * 'E' - temperature
  * 'V' - left/right balance 
*  ... other fields are self-explanatory

## Summary and Details

Combines [Summary](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#activity-summary) and [Details](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#details) in one chart.

## Editor

The 'Editor' chart provides all the activity file data in a spreadsheet/list format. The default view contains columns for all data series captured from your head-unit, as well as any data series derived.

As the name states, it does not only display the data, but you can also 'Edit' the data here. The multiple options available in the 'Editor' chart are described here:

![Editor - Complete View]  (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Activity_Editor-View.jpg)

### Icon Functions

![Editor - Icons](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Activity_Editor-Icons.jpg)

* `Save` - saves the activity data (with all changes/adjustments done)
* `Undo` - if active, there have been changes done to the activity series data (shown in the editor), those changes are reverted - if there are multiple changes done separately - then can be undone separately by pressing 'Undo' multiple times
* `Redo` - if active, you have been 'Undo'ing changes before - they can be re-applied be 'Redo'
* `Find` - opens a 'Search' dialog box - which allows to find specific values or value ranges in the series data - you can define search rules, the values to search and the data series to search in. As a result you get a list of search hits in the dialog box and the values fulfilling the search criteria are marked (with a different background color) in the 'Editor' data list. "Mouse-Click" on a result line in the dialog box, moves the data view to the specific search hit.
* `Anomalies` - when choosing, GoldenCheetah does a number consistency analysis on the available data points / data series. The analysis performed and their messages are:
  * 'Invalid recording gap' - there is a gap in recording of more than 1 second (gap)
  * 'Distance goes backwards' - like the description says
  * 'Suspiciously high cadence' - cadence detected is above 150
  * 'Suspiciously high heartrate' - heart rate detected is above 200
  * 'Suspiciously high speed' - speed detected is above 100 
  * 'Out of bounds value' - either latitude or longitude have invalid values 
  * 'Non-zero torque but zero cadence' - like the description says
  * 'Data spike candidate' - uses the 'Fix Power Spikes...' analysis and configuration settings to find power data spikes

'Anomalies' are listed in a 'Dialog box' - "Mouse-Click" on a text line in the dialog box, moves the data view to the specific anomaly in the editor data list.

## First Column - Context Menu

![Editor - First Column Menu](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Activity_Editor-Context_1st_Column.jpg)

* `Undo`, `Redo` - see above

***

* `Cut` - cuts the selected data section to the clipboard - 'Cut' is only available if you have selected COMPLETE rows
* `Copy` - copies the selected data section to the clipboard - 'Copy' works for any selection of cells
* `Paste` - pastes the clipboard data at chosen place - 'Paste' does not care for data consistency - (e.g. you can paste power values to the latitude cell)
* `Paste Special` - is aimed mainly to paste data from outside GoldenCheetah (e.g. from an Excel Spreadsheet) to a data series - you have different settings to tell GoldenCheetah how this data is structured (quite similar to 'Paste Special' features in other software products)
* `Clear Contents` - sets the cell in the marked data section to '0'

***

* `Delete Row` - deletes the current or the selected range of rows
* `Insert Row` - inserts an empty row at the current selection

## Column Header - Context Menu

![Editor - Column Header Menu](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Activity_Editor-Context_Header_Row.jpg)

* `Undo`, `Redo` - see above

***

* `Cut`, `Copy`, `Paste`, `Paste Special`, `Clear Contents` - see above

***

* `Remove Column` - removes the selected column 
* `Add Column` - opens a list of the available columns - only columns which are not yet visible on the editor chart can be added


## Data area - Context Menu

![Editor - Data area Menu](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Activity_Editor-Context_Data.jpg)


* `Undo`, `Redo` - see above

***

* `Cut`, `Copy`, `Paste`, `Paste Special`, `Clear Contents` - see above

***

* `Smooth Anomaly` - re-calculates the value of the selected cell as the average of the neighbors (previous and next data point in time) 


## Performance

This chart type provides all the graphs for your activity data series. In addition to data series which are captured by the head-unit directly, GoldenCheetah also delivers some derived series like 'Delta' series.

![Performance](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Performance-Overview.jpg)

## Performance Basic
* Basic Settings
  * `Shading` - here you select if, and how your power data curve is shown
  * `X-Axis `- choose if your activity X-Axis is plotted 'by time' or 'by distance'
  * `Smooth` - smooths the graphs - the value set here is used for all curves 

* View Settings
  * `Stack`, `By Series`
      * if 'Stack is NOT checked -  the 'By Series' setting is ignored and all curves are plotted in one diagram
     * if 'Stack' is checked and 'By Series' is checked - all curves are plotted in separate diagrams one above the other
      * if 'Stack' is checked and 'By Series' is NOT checked - all curves are plotted in one diagram, and the X-Axis is stretched over multiple lines
 
  * `Stack Zoom `- zooms the Y-Axis sizes for all diagrams (only takes effect if 'Show Stack' is checked)
  * `Full Plot` - if checked, in addition to the curves, an additional diagram (containing all the curves of the activity data series) is displayed at the lower border of the 'Activities' view - with this you also get the ability to zoom into the X-Axis - the button for zooming are below the 'Full Plot' curve
  * `Overlay` - if checked, it adds a small overlay window to the diagram, in which selected interval data is displayed
  * `Grid` - if checked, it adds a grid to the chart

### Performance Curves
* Data series settings
  * `Delta Series `- predefined delta series (calculated as '(Current_data_point_Value - Previous_data_point_Value) / (Time_between_the_data_points)')
  * `Left/Right `- Left leg / Right leg dependent data series (only provided by some power meter / head-unit combinations today)
  * `Data Series `- you can check the data series available from your head unit
  * `Metrics` - predefined metrics which use the data series and calculate data along the complete activity

## Special Features of the 'Performance' chart

* **References line** - for power and power related charts, you can add references lines to your chart

You can create a reference line via 'Mouse-Click (Hold) and Drag' from the Y-Axis label area. You can also do a 'Double-Click' on this area to open a dialog box to '+' (add) and '-' (remove) references lines.

_Note: References Lines are not supported for any non-power related chart like e.g. Heart Rate._

`Mouse-Click (Hold) and Drag`

![Performance - Reference Line](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Performance_Create_Ref_Line.gif)


`Double-Click`

![Performance - Reference Line](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Performance_Edit_Ref_Line.gif)


* **Scaling Y-Axis** - by 'Single Mouse-Click' into the Y-Axis label area, you get two sliders handles which you can drag (up and down) to change the scale of the Y-Axis of that specific chart (only in 'Stacked' mode)

`Single Mouse-Click`

![Performance - Scaling Y-Axis](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Performance_Scale_Y-Axis.gif)

* **Interactive marking of intervals** - can be done be 'Mouse-Click (Hold) and Drag' in the charts - the intervals is valid/visible for all curves - the feature works independent of stack-view active or not

`Mouse-Click (Hold) and Drag`

![Performance - Select Interval](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Performance_Select_Interval.gif)

* **Show single curves** - (only in non-stacked mode) - by 'Mouse-Over' on a Y-Axis label for a curve, only this particular curve is shown on the chart

`Mouse-Over`

![Performance - Show single curve](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Performance_Isolate_Series.gif)

* **Zoom into curves** - (only in non-stacked mode) - allows to select rectangle plot areas to zoom in - zooming can be done multiple times

`Shift + Left Mouse Button` - to select an area and zoom in when releasing

`Right Mouse Button` - to zoom out 1 level

`Crtl + Right Mouse Button` - to zoom out to full view

![Performance - Show single curve](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Performance_ZoomInOut.gif)



## Critical Mean Maximal

[Similar to 'Trends View' - for a single activity](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Trends#critical-mean-maximal)

## Histogram

![Activity Histogram](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Activity_Histogram.jpg)

* `Data Series Box` - selection of activity data series to be analysed
* `Time` - choose between 'Absolute Time' or 'Percentage Time'
* `Log Y` - if checked, shows the time axis (here Y) in log scale
* `With zeros` - if checked, also zeros are considered in the plot
* `Shade zones` - if checked, the power and HR zones are shown (available for data series: 'Power', 'Watts per Kilogram' and 'Heartrate') 
* `Show in zones` - if checked shows the data according to your zone settings (available for data series: 'Power', 'Watts per Kilogram' and 'Heartrate')
* `Use polarized zones` - you need to have 'Show in zones' checked as well - if checked, shows for 'Power' and 'Watts per Kilogram' series the distribution to 3 program defined zones (I = 0 to 85% of CP, II = 85 to 100% of CP and III > 100% of CP)

* `Bin width `- both input field and slider to set the value - defined the X-Size of data range accumulated into one bar of the diagram (the size defined here has no influence if 'Show in zones' is checked)

_Note: 'Bin width', 'Shade Zones' and 'Show in Zones' are also available in the drop down area on the upper border of the graphics view pane._

## Pedal Force vs Velocity

This chart provides a so called 'Quadrant Analysis' of Pedal Force vs Pedal Velocity.

![Pedal Force vs Velocity](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/PedalForce_vs_Velocity.jpg)

* Definition of the quadrants is done by the input of 'Watts' and 'RPM
  * `Watts` - a curve through the chart which is reflects the entered power 
  * `RPM` - the cadence for which the curve is split into quadrants

* `Crank Length` - determines the correct values and scale for the X-Axis (defaulted from your 'Preferences -> Athlete' data)
* `Shade Zones` - if checked, the power zones are shown
* `Merge Intervals` - if checked (and 'Frame Interval' is NOT checked) - shows the intervals selected in the 'Side Bar' but not the complete data points
* `Frame Intervals` - if checked - shows all data points - and highlights the intervals selected in the 'Side Bar'

## Heartrate vs Power

This chart shows the distribution of HR and the distribution of power for the whole activity (on X-Axis (Power) / on Y-Axis (Heart Rate) - along with the HR/Power data points during the activity.

![HR vs Power](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/HR_vs_Power.jpg)

The distribution of HR and Power is shown proportional, but not with a specific scale. The mouse-over information on the bars is only relevant for the dimension (Power or Heart rate) of the axis. The seconds value is of no means.

The set of colored points / the colored line in the center of the chart shows the development of the Power/Heart rate relationship over the time of the activity. The determination approach and the relation to the chart parameters is outlined here:

* Power/Heart rate data points for the plot are
  * `Smooth` the activity data points (every second) are first "smoothed" by calculating the moving average value over the time period (in seconds) defined in this parameter
  * Only data points where the heart rate is above 50 and power is between 50 and 500 watts are further considered
  * `HR Delay` shifts the heart rate by the given value (in seconds) - that means for a data point recorded at second in the rade "X" the heart rate from second 'X+HR Delay" is assigned
  * To reduce the number of data points shown on the plot, only every 10th point is plotted

* Other chart parameters are:
  * `Join Points` - if checked, instead of single data points they are plotted as a complete line
  * `Shade Zones` - if checked, adds the power zone shading
  * `Show Full Plot` - if checked, also the activity (power and heart rate curves only) are shown at the bottom of the view

* The coloring of the power/heart rate plot (along the activity time) follows a special logic. The available data points are segmented into 36 subsequent groups. Each group is assigned a separate color, which is determined from an HSV color code. The HSV coloring covers all colors in a "circle style". Each segment of the activity data points segment is plotted in a color of the circle (see HSV colors) - starting at 'Yellow' and moving by an angle of 10 degrees (direction see 'Arrow') to determine the color for each new segment.

![HR vs Power Colors](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/HR_vs_Power_Colors.jpg)

The Power@150 value is estimation of your PWC150 value based on activity data. PWC150 (Physical Work Capacity at HR 150) is a measure in diagnostics - it follows a tiered test protocol but ends with the HR of its name (here 150). For further details, please use the search engine of your choice with the given key words.

## Google Map / Bing Map

If GPS data is available, the activity is shown on a Google Map, or a Bing Map. _Note: You need to be connected to the internet._

The functionality provided on the maps differs on what Google or Bing is offering (e.g. multiple views, zoom, rotate). GoldenCheetah itself adds capabilities to:

* Show Start/End point of the track - special icons for start/end point of track appears
* Show Intervals - by marking one or more interval in the 'Side Bar'- 'Intervals' pane, the part of the track belonging to the intervals is 'highlighted'. The start points of all intervals are always marked in a track - and you can also 'Mouse-Click' on the markers to 'highlight' and interval (only for Google).
* Color - the color of the track gives an indication about the Power Zone you have been riding a certain track - colors are the same like in the color shading of the power-curves

## 2d Plot

The '2d Plot' - also called 'Scatter Plot' - displays the activity data as a collection of points, each having the value of data series determining the position on the X-Axis and the value of the other data series determining the position on the Y-Axis.

![2d Plot](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/2d_Plot.jpg)

* `X-Axis` - drop-down list box with the available data series (e.g. Power,...)
* `Y-Axis` - drop-down list box with the available data series (e.g. Power,...)
* `Ignore Zero` - if checked, data points which are '0' are not plotted
* `Show Grid` - if checked, a grid is displayed in the plot area
* `Frame Intervals` - if checked, and you select one or more intervals in the 'Side Bar', the data points belonging to the interval are highlighted


## 3d Plot

The '3d Plot' displays the activity data in a 3d graphics - which you can zoom and rotate.

![3d Plot](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/3d_Plot.jpg)

* `Analyse` - offers a number of default-settings for X,Y,and Z-Axis which you can use - the setting 'User Defined' is the option to defined the Axis individually (after applying a default setting, you can still change the Axis settings as well)
* `X-Axis` - drop-down list box with the data series (e.g. Power,...)
* `Y-Axis` - drop-down list box with the data series (e.g. Power,...)
* `Z-Axis` - drop-down list box with the data series (e.g. Power,...)
* `Color` - drop-down list box with the data series (e.g. Power,...) - can be considered as a 4th dimension of the chart
* `Graphic Type` - drop-down list box to choose the visualization variant ('Bar', 'Grid', 'Surface' or 'Dots')
* `Bin Width` - both input field and slider to set the value - which is the width of the plotted chart segments
* `Ignore Zero` - if checked, data points which are '0' are not plotted
* `Show Grid` - if checked, a grid is displayed in the plot area
* `Frame Intervals` - if checked, and you select one or more intervals in the 'Side Bar', the data points belonging to the interval are highlighted
* `Legend` - if checked, the legend for the chart is shown

You can rotate the 3d graphics in all 3 directions with you mouse. As well as adding an 'layer' to the 'Z-Axis':

![Rotate](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Activity_3d-rotate.gif)

You can add an analysis layer to the 'Z-Axis':

![Layer](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Activity_3d-analyis-layer.gif)

## Aerolab Chung Analysis

The 'Aerolab' chart provides a tool to use the Robert Chung's Virtual Elevation method to derive CdA and CRR from a power file. 

![Aerolab](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Aerolab.jpg)

For the theory on this, sample test protocols for the power/activity file you need for an analysis see [Dr Chung's document describing the theory and practice of 'Virtual Elevation'](https://github.com/GoldenCheetah/GoldenCheetah/blob/master/doc/contrib/ChungVE.pdf?raw=true).


BACK: [Chart Types: General](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_General)