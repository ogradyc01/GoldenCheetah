Chart Types: Trends view (Version 3.1)
***

The 'Trends' view offers 'Chart Types' which work on a range of rides. The rides which are considered when opening a chart here selected based on the 'Date Range' selected - as well as the actual 'Search/Filter' settings. 

_Note: Both selection criteria 'Date Range' and 'Search/Filter' can also be configured within a concrete chart of the 'Chart' bar. This means the more general settings of the 'Side Bar' are ignored in such cases._

* [Metric Trends] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#metric-trends)
* [Collection Tree Map] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#collection-tree-map)
* [Critical Mean Maximal] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#critical-mean-maximal)
* [Distribution] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#distribution)
* [Summary] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#summary)

## Metric Trends

The long term metrics provided by the 'Metrics Trends' covers all pre-defined metrics but allows also to add self-defined 'Best value' metrics as well as 'Estimate' metrics.

### Basic Settings

The first screen of the dialog box to add a 'Metric Trends' chart are the basic settings. To ease the configuration, you will see the results of your configuration already in the 'Preview' section on the left side of the dialog box. This simplifies configuration without a lot navigation between the settings and the resulting chart.

![Metric Trends - New Basic] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/MetricTrends_New_Basic.jpg)

* [Filter] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Special-Topics_SearchFilter) - define chart specific 'Search/Filter' criteria 
* [Date Range] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#date-range-selection) - define chart specific 'Date Range' settings
* `Group by` - defines the default grouping setting of the metrics - you can interactively change the grouping when displaying the chart
* `Data Table` - if checked, not curves, but a table with the data / curve values used is shown
* `Show Stack` - if checked, the different curves are shown separately one above the other (see also 'Stack Zoom')
* `Shade Zones` - if checked / and the chart has a power related metrics - shows the power-zones
* `Show Legend` - if checked, shows the legend of the curves included in the chart
* `Show Events` - if checked, shows events (if events are defined)
* `Stack Zoom` - zooms the diagrams if 'Show Stack' is checked

### Presets

GoldenCheetah comes with a number of 'Presets' for your charts - when creating a new 'Athlete' the presets are taken over to the athlete's library - and from that point on, any changes, enhancements of this presets are athlete specific.

![Metric Trends - New Basic] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/MetricTrends_New_Preset.jpg)

The 'Presets' view of the dialog box is multi-functional, so besides using a 'Preset' to configure a new chart, the dialog box offers a full set of 'Preset' administration functions.

* Using a preset
  * `Apply` - applies the settings of the currently selected preset in the list (= takes over the 'Curves' defined in the 'Preset')

* Maintain presets
  * `Rename` - change the name
  * `Delete` - removes/delete a preset
  * `Move Up` - moves the selected preset 'up' in the list
  * `Move Down` - moves the selected preset 'down' in the list

_Note: Since the presets available here are also used in the 'Library' chart, these functions can be helpful to setup your personal list of presets / charts for this view. (see [Side Bar - Trends View] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Trends-view#charts))_

* Get more presets
  * `Import...` - imports an XML File with presets - the imported presets are ADDED to the current preset - the import does not check of duplicates,... (_Note: since the file format of the XML is specific to GoldenCheetah and also contains "serialized" for certain configuration settings, manual creation of a valid XML file is not recommended (and will most likely not work)_)
  * `Export...` - exports ALL presets available in the list to an XML File (_Note: Only by using the 'Export...' function you get a valid XML file which can be imported to other GoldenCheetah installations. Please observe - since the file format might differ between GoldenCheetah version, you can only expect this to work when using the same GoldenCheetah version.)
  * `Add current` - adds the chart definition (curves, settings,...) you are currently working on, to the 'Preset' list as a new preset. (Basically this feature provides a 'Create Preset' function using the settings in focus.

### Curves

The curves are what is actually shown on the charts. The curves can either come from presets, or are defined here by adding them. Also editing / adjustments of existing curves is possible.

![Metric Trends - New Curves] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/MetricTrends_New_Curve.jpg)

* `Edit` - changes the settings of the selected curve
* `+` - opens the dialog to add a new curve
* `-` - removes a curve
* `User sidebar chart settings` - if checked, any curve settings are ignored, and the created chart serves as a proxy for the [Side Bar - Charts] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Trends-view#charts))

### Curves - Details - Metric

'Metric's are pre-defined in GoldenCheetah. Each metric determines the data to be shown in the curve/diagram.

![Metric Trends - New Curve - Metric] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/MetricTrends_New_Curve_Edit.jpg)

For the further settings see: [Curve Settings] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#curve-settings)

### Curves - Details - Best

'Best's are user-defined metrics. 'Best' delivers curves which show the best value / for a defined period in time / for a defined data series.

![Metric Trends - New Curve - Metric] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/MetricTrends_New_Curve_Edit_Best.jpg)

Supported data series are visible in the drop-down list - starting with `Power`,...

For the further settings see: [Curve Settings] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#curve-settings)


### Curves - Details - Estimates

'Estimate's are metric curves derived based on the CP models. 

![Metric Trends - New Curve - Metric] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/MetricTrends_New_Curve_Edit_Estimates.jpg)

As parameter you need to choose the CP model to use and the data series to estimate on that model. Since not all models support all data series, depending on the selected model, some data series cannot be selected.

For the further settings see: [Curve Settings] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#curve-settings)

## Collection Tree Map

The 'Collection Tree Map' is an very useful tool to analyse how your rides distribute - e.g. regarding your "Workout Codes", or equipment (if you maintain it).

What the graphics does is a 2-dimensional map where you can 
* define the 2 Dimensions (here called 'First' and 'Second') and
* define the metrics used to calculate the size of a tree/map-segment.

What GoldenCheetah does is to summarize the selected metrics for all selected rides ('Date Range' and 'Filter' is considered) and shows for each separate value combination of the configured dimensions, a tile which goes in line with the accumulated metric value for the tile.

_Note: Possible dimensions for 'First' and 'Second' are all text fields from the rides - details (as defined in the preferences). So like for 'Search/Filter' only if you maintain data and the values are consistent, you will get useful output here._

_Note2: Unlike 'Search/Filter' the field content is treated as 'Case Sensitive'_

The example summarizes 'TSS' values, first by 'Workout Code' and second by 'Keywords' (which in the example data was to defined the bicycle used for a workout).

![Collection Tree Map - First] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/CollectionTree_First.jpg)

![Collection Tree Map - Second] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/CollectionTree_Second.jpg)

***

If you do a 'Mouse-Click' on one of the tiles, the list of rides which added up to this tile are shown - together with their metric values. You can scroll through the list to get some ride detail information displayed.

![Collection Tree Map - Rides] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/CollectionTree_RidePopup.jpg)


## Critical Mean Maximal

This curve, also called 'MMP' curve is again one of the central and assumed 'Standard' ways for analyzing power. Here only the handling / available option are described.

![CP] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/CriticalMeanMaximal_Basic.jpg)

As in most other charts, also here you have several options, and the options partly relate to each other. Knowing which combinations are supported (and also which not) - is important to maximize the use of the chart.

* [Filter] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Special-Topics_SearchFilter) - define chart specific 'Search/Filter' criteria 
* [Date Range] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#date-range-selection) - define chart specific 'Date Range' settings
_Note: On the 'Rides View' the 'Date Range' parameter are a drop-down list, where you can select 'Date Range' which are then considered in the 'Bests' calculation._
* `Data series `- here you have multiple sets of data which can be analyzed in the 'MMP' curve style. Important to know is that you also need to check 'Show Bests' to show the curve for any of the 'Data Series' - otherwise you might see only the 'CP Model' curve (for 'Data Series' = 'Power', or an empty chart for any other 'Data Series').
* `Power Shading `- if checked, shows the power zones, along the curve. Only has effect for 'Data Series' = 'Power'.
* `Show Grid`- if checked, the plot area get's a grid for easier analysis
* `Show Bests `- if checked, shows the 'MMP' curve (the best value for point of duration of the X-Axis) for the 'Data Series' selected
* `Show as percentage` - only for single rides on the 'Rides' view - if checked, it shows not the absolute values, but the percentage of the actual ride value in relation to 'Bests'
* `Show curve heat` - shows the number of rides, whose maximal power duration is within 10% of the best
* `Show curve heat by date` - ...
* `Shade Intervals` - only for single rides on the 'Rides' view - shows separate curves for an interval, if you select it on the 'Side Bar' - multiple selection of intervals is possible

![CP Model] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/CriticalMeanMaximal_CP_Model_Extended.jpg)

You can show the theoretical CP curve, based on one of GoldenCheetah's models, by going to the `CP Model` tab in the configuration, selecting one of the available models and either using the default parameters (of the model) or adjusting them to your needs.

## Distribution

This chart type allows to show the distribution of either 'Ride Data Samples' or 'Ride Metric' in different dimensions. 

![Distribution - Ride Data] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Distribution - Ride Data Samples.jpg)

When choosing 'Ride Data Samples' the selected data series applies to the X-Axis, where the time is shown on the Y-Axis:

* [Filter] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Special-Topics_SearchFilter) - define chart specific 'Search/Filter' criteria 
* [Date Range] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#date-range-selection) - define chart specific 'Date Range' settings
* 'Plot' section 
  * `Ride Data Samples` has to be checked for this variant
  * `Data Series Box` - Selection of available ride data series
* 'Show' section
  * `Time` - select between 'Absolute Time' or 'Percentage Time'
  * `Log Y` - if checked, shows the time axis (here Y) in logarithmic scale
  * `With zeros` - if checked, also zeros are considered in the plot
  * `Shade zones` - only for single rides on the 'Rides' view - if checked, the power and HR zones are shown (available for data series: 'Power', 'Watts per Kilogram' and 'Heart rate') 
  * `Show in zones` - if checked shows the data according to your zone settings (available for data series: 'Power', 'Watts per Kilogram' and 'Heart rate')
  * `Use polarized zones` - you need to have 'Show in zones' checked as well - if checked, shows for 'Power' and 'Watts per Kilogram' series the distribution to 3 fix defined zones (I = 0 to 85% of CP, II = 85 to 100% of CP and III > 100% of CP)

* `Bin width `- both input field and slider to set the value - defines the X-Size of data range accumulated into one bar of the diagram (the size defined here is not used if 'Show in zones' is checked)

_Note: 'Bin width', 'Shade Zones' and 'Show in Zones' are also available in the drop down area on the upper border of the graphics view pane._

***

![Distribution - Ride Metrics] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Distribution - Ride Metrics.jpg)

When choosing 'Ride Metrics' you can select both X-Axis and Y-Axis metrics from the provided lists. Besides the metrics the only other parameter is the `Color` for drawing and the `Bin width` (like before).

## Summary

A summary chart is chart with fixed structure, which displays a summary about the selected 'Date Range'. 'Search/Filter' settings are considered when creating the charts.

* Contents Section are:
  * Totals, Average, Maximums, Metrics, Model information - the 'Metrics' shown are configurable through 'Preferences' -> 'Metrics' -> 'Summary'
  * Athlete Best - the fields shown are configurable through 'Preferences' 
  * Power Zones - the power zones as configured in 'Preferences', considering the 'Date Range' settings (as far as they fit to the date ranges in your power zone settings)
  * Heart Rate Zones - the heart rate zones as configured in 'Preferences', considering the 'Date Range' settings (as far as they fit to the date ranges in your power zone settings)
  * "##" Rides - ride list - the fields shown are configurable through 'Preferences' -> 'Metrics' -> 'Summary'

* Configuration of 'Summary' chart itself offers:
  * [Filter] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Special-Topics_SearchFilter) - define chart specific 'Search/Filter' criteria 
  * [Date Range] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#date-range-selection) - define chart specific 'Date Range' settings


## Date Range Selection

![Date Range] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/ChartsGeneral_DateRange.jpg)

* `Current selection` - uses the date range active in the 'Date Ranges' pane of the 'Side Bar'
* `Current selection thru today` - uses the date range active, (like the one before), but limits the 'to-date' to the current date
* `From 'date' to today` - starts with the defined 'date' and ends today
* `Between 'from' and 'to'` - does what is says
* `Last 'x' (days, weeks, months or years)` - goes backward the given time frame
* T`his (week, month, year) prior 'x'` - subtracts a number of (weeks, months, years) from the actual (week, month, year) to define the new date range (e.g. "This 'month' prior '3'" - means the time range 3 month back - so if it is 'July', date range will be 'April'). 


## Curve Settings

The 'Curve' settings configure how a 'Metric', 'Best', or 'Estimate' curve is plotted in your diagram. 

![Curve - Settings] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/MetricTrends_New_Curve_Details.jpg)

* General
  * `Name` - is a user defined name for the curve 
  * `Axis/Label / Units` - is the description shown on the axis labels

* Style and Color
  * `Style` - is the plot style (you can have a line, dots, bars,...)
  * `Symbol` - is an additional marker for the single data point - works for the style, where adding a symbol makes sense
  * `Stack` - is special - it works only for curves where the style is set to 'Bar' AND you need to define more that one curve where style is 'Bar' - when checking 'Stack' for such 2 or more curves then, there is just ONE bar which contains the different curve data as sections in the bar 
  * `Color` - the color to be used for the curve (to select a color, "Mouse-Click" on the color box to open a 'Color Chooser' dialog box
  * `Fill curve` - fills the area "below" the curve with a color shade

* Special Options
  * `Highlight Highest` - puts markers on the curve for the 'X' highest values (if '0' - no point is marked)
  * `Highlight Lowest` - puts markers on the curve for the 'X' lowest values (if '0' - no point is marked)
  * `Highlight Outliers` - puts markers on the curve for the 'X' outliers (if '0' - no point is marked)
  * `Baseline` - sets a value for the curve which is considered as '0' regarding the Y-Axis scale (Example: If you set 100 as the 'Baseline' for your TSS curve, any value above 100 will be treated as positive, every value below 100 negative so 150 TSS shows +50 on the Y-Axis, 70 TSS shows -30 on the Y-Axis.)
  * `Trend Line` - 'No trend Line' or 'Linear Trend' or 'Quadratic Trend' decides if a 'Trend Line' for the curve data is shown at all, and if yes, how the trend is calculated
  * `Smooth Curve` - makes curves with many small peaks/changes better readable/understandable  
  * `Data labels` - if checked, also the value for a data point is shown in the plot

***

BACK: [Chart Types: General] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_General)