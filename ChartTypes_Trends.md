Chart Types: Trends view (Version 3.1)
***

The 'Trends' view provides 'Chart Types' which work on a more than one ride. The rides which are considered when opening a chart here selected based on the 'Date Range' selected - as well as the actual 'Search/Filter' settings. 

_Note: Both selection criteria 'Date Range' and 'Search/Filter' can also be configured within a concrete chart of the 'Chart' bar. This means the general settings done in the 'Side Bar' are ignored in such cases._

* [Metric Trends] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#metric-trends)
* [Collection Tree Map] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#collection-tree-map)
* [Critical Mean Maximal] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#metric-critical-mean-maximal)
* [Distribution] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#distribution)
* [Summary] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#summary)

## Metric Trends

The long term metrics provided by the 'Metrics Trends' covers all pre-defined metrics but allows also to add self-defined 'Best value' metrics as well as 'Estimate' metrics.

### Basic Settings

The first screen of the dialog to add a Metric Trends chart are the basic settings. To ease the configuration, you will see the results of your configuration already in teh 'Preview' section on the left side of the dialog box. This allows easy configuration without a lot navigation between the settings and the resulting chart.

![Metric Trends - New Basic] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/MetricTrends_New_Basic.jpg)

* [Filter] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Special-Topics_SearchFilter) - define chart specific 'Search/Filter' criteria 
* [Date Range] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#date-range-selection) - define chart specific 'Date Range' settings
* Group by - defines the default grouping setting of the metrics - you can change the grouping using the chart
* Data Table - if checked, not curves, but a table with the data used is shown
* Show Stack - if checked, the different curves are shown separately own above the other (see also 'Stack
* Shade Zones - if checked / and the chart has a power related metrics - show the power-zones
* Show Legend - if checked, show the legend of the curves included in the chart
* Show Events - if checked, show events (if events are defined)
* Stack Zoom - zooms the diagrams if 'Show Stack' is checked

### Presets

GoldenCheetah comes with a set of 'Presets' for you charts - when creating a new 'Athlete' the presets are taken over to the athlete's library - and from that point on any changes, enhancements of this presets are athlete specific.

![Metric Trends - New Basic] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/MetricTrends_New_Preset.jpg)

The 'Presets' view of the dialog box is multi-functional, so besides using a 'Preset' to configure a new chart, the dialog box offers a full set of 'Preset' administration functions.

* Using a preset
  * `Apply` - applies the settings of the selected presets (= takes over the 'Curves' defined in the 'Preset')

* Maintain presets
  * `Rename` - change the name
  * `Delete` - removes/delete a preset
  * `Move Up` - moves the selected preset 'up' in the list
  * `Move Down` - moves the selected preset 'down' in the list

_Note: Since the presets available here are also used in the 'Library' chart, these functions can be helpful to setup your list of presets / charts for this view. (see [Side Bar - Trends View] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Trends-view#charts))_

* Get more presets
  * `Import...` -
  * `Export...` -
  * `Add current` -

### Curves

The curves are what is actually shown on the charts. The curves can either come from presets, or are defined here by adding new charts. Also editing / adjustments of existing curves is possible.

![Metric Trends - New Curves] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/MetricTrends_New_Curve.jpg)

* `Edit` - changes the settings of the selected curve
* `+` - opens the dialog to add a new curve
* `-` - removes a curve
* `User sidebar chart settings` - if checked, any curve settings are ignored, and the created chart serves as a proxy for the [Side Bar - Charts] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Trends-view#charts))

### Curves - Details - Metric

'Metric's are pre-defined in GoldenCheetah. Each metric determines the data to be shown in the graph.

![Metric Trends - New Curve - Metric] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/MetricTrends_New_Curve_Edit.jpg)





### Curves - Details - Best

'Best's are a kind of definable metrics. Best will  

![Metric Trends - New Curve - Metric] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/MetricTrends_New_Curve_Edit_Best.jpg)


### Curves - Details - Estimates

![Metric Trends - New Curve - Metric] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/MetricTrends_New_Curve_Edit_Estimates.jpg)




## Collection Tree Map

![Collection Tree Map - First] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/CollectionTree_First.jpg)


![Collection Tree Map - Second] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/CollectionTree_Second.jpg)


![Collection Tree Map - Rides] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/CollectionTree_RidePopup.jpg)


## Critical Mean Maximal

![CP] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/CriticalMeanMaximal_Basic.jpg)


![CP Model] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/CriticalMeanMaximal_CP_Model_Extended.jpg)


![CP Speed] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/CriticalMeanMaximal_Speed.jpg)


## Distribution

![Distribution - Ride Data] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Distribution - Ride Data Samples.jpg)


![Distribution - Ride Metrics] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Distribution - Ride Metrics.jpg)

## Summary

## Date Range Selection

![Date Range] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/ChartsGeneral_DateRange.jpg)

## Curve Settings

The 'Curve' settings configure how a 'Metric', 'Best', or 'Estimate' is plotted in your diagram. 

![Curve - Settings] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/MetricTrends_New_Curve_Edit.jpg)

* Name - is a user defined name for the curve
* Axis/Label / Units - is the description shown on the axis labels
* Style - is the plot style 
* Symbol - is 
* Stack - 
* Color - the color to be used for the curve (to select a color, "Mouse-Click" on the color box to open a 'Color Chooser' dialog box
* Fill curve - fills the area "below" the curve with a color shade
* Highlight Highest - puts markers on the curve for the 'X' hightest values (if '0' - no point is marked)
* Highlight Lowest - puts markers on the curve for the 'X' lowest values (if '0' - no point is marked)
* Highlight Outliers - puts markes on the curve for the 'X' outliers (if '0' - no point is marked)
* Baseline
* `No trend Line` or 'xxx or 'xxx'
* Smooth Curve - 
* Data lables - 

***

BACK: [Chart Types: General] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_General)