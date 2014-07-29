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

## Editor

## Performance

## Critical Mean Maximals

[Similar to 'Trends View' - for a single ride] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#critical-mean-maximal)

## Histogram

[Similar to 'Trends View' - for a single ride] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_Trends#distribution--histogram)

## Pedal Force vs Velocity

## Heartrate vs Power

## Google Map / Bing Map

## 2d Plot

## 3d Plot

## Aerolab Chung Analysis

BACK: [Chart Types: General] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/ChartTypes_General)