Special Topics: Ride Processing (Version 3.1)
***

GoldenCheetah provides a number of tools to fix/adjust/correct ride data. The adjustments can either be executing manually for a specific ride, or automatically during import of rides.

The configuration of the available tools is done in ['Preferences' -> 'Data Fields'] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_310_Preferences_Data-Fields#processing)

* If you set a tool to 'Manual' in the preferences, you have to run it manually per ride through `Tools-><name of the tool>`. The values set in preferences then are taken as defaults, which you can still override in a dialog box, when running the tool.

* If you set a tool to 'Auto' in the preferences, the tool is executed with the parameter settings from 'Preferences' for each ride import you are doing. You can still run the tool manually with different parameters after the import is done.

_Note: The fixes/changes are only done to the ride file stored in GoldenCheetah format (.json) - GoldenCheetah does not manipulate any of original data files._

## General: Undo/Redo

Any changes to the ride data done by the tools explained below, are not immediately stored. There are basically three ways to 'Undo' then changes of processing tools:

* 'Leave without Saving' - you can always end GoldenCheetah without saving your ride data - (depending on your settings GoldenCheetah will ask / or not, if you have done any changes). When going this way ALL changes done since last saving of the ride file is lost.

* 'Revert to Saved version' - on the 'Side Bar' -> 'Rides' pane, the context menu changes when ride data has changed - it then also offers a 'Revert to saved version' function.

* 'Undo/Redo' - in the 'Rides' view - 'Editor' chart, you have an explicit 'Undo/Redo' feature available. Every run of a tool is collected into an 'Undo' stack, which can then be used to get back to the version of data before running the tool. You can also 'Redo' the changes - which re-applies the changes (only if you did an 'Undo' before. See also [Rides - Editor] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_310_ChartTypes_Rides#editor)

## Tool: Adjust Torque

Adjusting torque values allows you to uplift or degrade the torque values when the calibration of your power meter was incorrect. It takes a single parameter: 

* `Torque Adjust` - this defines an absolute value in poinds per square inch or newton meters to modify values by. Negative values are supported. (e.g. enter "1.2 nm" or "-0.5 pi").

## Tool: Fix GPS errors

Remove GPS errors and interpolate positional data where the GPS device did not record any data, or the data that was recorded is invalid.

* No parameters.

## Tool: Fix Gaps in Recording

Many devices, especially wireless devices, will drop connections to the bike computer. This leads to lost samples in the resulting data, or so-called drops in recording. In order to calculate peak powers and averages, it is very helpful to remove these gaps, and either smooth the data where it is missing or just replace with zero value samples

This function performs this task, taking two parameters:

* `Tolerance` - this defines the minimum size of a recording gap (in seconds) that will be processed. Any gap shorter than this will not be affected.
* `Stop` - this defines the maximum size of gap (in seconds) that will have a smoothing algorithm applied. Where a gap is shorter than this value it will be filled with values interpolated from the values recorded before and after the gap. If it is longer than this value, it will be filled with zero values.

## Tool: Fix HR Spikes

Occasionally heart rate sensors will erroneously report high values for heart rate or drop out (0). This function will look for spikes and dropouts in heart rate data and replace the erroneous data by interpolating the data from either side of the point in question

It takes a single parameter:

* `Absolute Max` - this defines an absolute value for heart rates, and will smooth any values above this absolute value that have been identified as being anomalies (i.e. at odds with the data surrounding it).

## Tool: Fix Power Spikes

Occasionally power meters will erroneously report high values for power. For crank based power meters such as SRM and Quarq this is caused by an erroneous cadence reading as a result of triggering a reed switch whilst pushing off. This function will look for spikes/anomalies in power data and replace the erroneous data by smoothing/interpolating the data from either side of the point in question

It takes the following parameters:

* `Absolute Max` - this defines an absolute value for watts, and will smooth any values above this absolute value that have been identified as being anomalies (i.e. at odds with the data surrounding it)
* `Variance (%)` - this will smooth any values which are higher than this percentage of the rolling average wattage for the 30 seconds leading up to the spike.

BACK: [Special Topics: Overview] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_310_Special-Topics_Overview)