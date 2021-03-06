Special Topics: Activity Processing (Version 3.2)
***

GoldenCheetah provides a number of tools to fix/adjust/correct activity data. The adjustments can either be executing manually for a specific activity, or automatically during import of activities.

The configuration of the available tools is done in ['Preferences' -> 'Data Fields'](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Preferences_Data-Fields#processing)

* If you set a tool to 'Manual' in the preferences, you have to run it manually per activity through `Tools-><name of the tool>`. The values set in preferences then are taken as defaults, which you can still overactivity in a dialog box, when running the tool.

* If you set a tool to 'Auto' in the preferences, the tool is executed with the parameter settings from 'Preferences' for each activity import you are doing. You can still run the tool manually with different parameters after the import is done.

_Note: The fixes/changes are only done to the activity file stored in GoldenCheetah format (.json) - GoldenCheetah does not manipulate any of original data files._

## General: Undo/Redo

Any changes to the activity data done by the tools explained below, are not immediately stored. There are basically three ways to 'Undo' then changes of processing tools:

* 'Leave without Saving' - you can always end GoldenCheetah without saving your activity data - (depending on your settings GoldenCheetah will ask / or not, if you have done any changes). When going this way ALL changes done since last saving of the activity file is lost.

* 'Revert to Saved version' - on the 'Side Bar' -> 'Activities' pane, the context menu changes when activity data has changed - it then also offers a 'Revert to saved version' function.

* 'Undo/Redo' - in the 'Activities' view - 'Editor' chart, you have an explicit 'Undo/Redo' feature available. Every run of a tool is collected into an 'Undo' stack, which can then be used to get back to the version of data before running the tool. You can also 'Redo' the changes - which re-applies the changes (only if you did an 'Undo' before. See also [Activities - Editor](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#editor)

## Edit tool: Add Torque

Derive torque when power and cadence data is available.

* No parameters.

## Edit tool: Adjust Torque

Adjusting torque values allows you to uplift or degrade the torque values when the calibration of your power meter was incorrect. It takes a single parameter: 

* `Torque Adjust` - this defines an absolute value in poinds per square inch or newton meters to modify values by. Negative values are supported. (e.g. enter "1.2 nm" or "-0.5 pi").

## Edit tool: Adjust Power

Adjusting power values allows you to uplift or degrade the power values by a percentage. It takes a single parameter:

* `Power Adjustment` - this defines percentage  to modify values by. Negative values are supported.

## Edit tool: Estimate Power

Derive estimated power data based on speed/elevation/weight etc.

* No parameters.

## Edit tool: Fix Elevation errors

Fix or add elevation data. If elevation data is present it will be removed and overwritten.
The elevation data is required from the MapQuest OpenElevation API: http://open.mapquestapi.com/elevation/

_Note: The web-site does not provide exact information which elevation source data is used. Some texts refer to SRTM data - so it's quite probably that this data is used. Accuracy of the service is not documented._

INTERNET CONNECTION REQUIRED.

* No parameters.

## Edit tool: Fix GPS errors

Remove GPS errors and interpolate positional data where the GPS device did not record any data, or the data that was recorded is invalid.

* No parameters.

## Edit tool: Fix Gaps in Recording

Many devices, especially wireless devices, will drop connections to the bike computer. This leads to lost samples in the resulting data, or so-called drops in recording. In order to calculate peak powers and averages, it is very helpful to remove these gaps, and either smooth the data where it is missing or just replace with zero value samples

This function performs this task, taking two parameters:

* `Tolerance` - this defines the minimum size of a recording gap (in seconds) that will be processed. Any gap shorter than this will not be affected.
* `Stop` - this defines the maximum size of gap (in seconds) that will have a smoothing algorithm applied. Where a gap is shorter than this value it will be filled with values interpolated from the values recorded before and after the gap. If it is longer than this value, it will be filled with zero values.

## Edit tool: Fix HR Spikes

Occasionally heart rate sensors will erroneously report high values for heart rate or drop out (0). This function will look for spikes and dropouts in heart rate data and replace the erroneous data by interpolating the data from either side of the point in question

It takes a single parameter:

* `Absolute Max` - this defines an absolute value for heart rates, and will smooth any values above this absolute value that have been identified as being anomalies (i.e. at odds with the data surrounding it).

## Edit tool: Set SmO2/tHb from Speed and Cadence

When recording from the Moxy in Speed and cadence mode the SmO2 and tHb data is sent as cadence and speed respectively. This tool will update the activity file to move the values from speed and cadence into the Moxy series.

* No parameters.

## Edit tool: Fix Power Spikes

Occasionally power meters will erroneously report high values for power. For crank based power meters such as SRM and Quarq this is caused by an erroneous cadence reading as a result of triggering a reed switch whilst pushing off. This function will look for spikes/anomalies in power data and replace the erroneous data by smoothing/interpolating the data from either side of the point in question

It takes the following parameters:

* `Absolute Max` - this defines an absolute value for watts, and will smooth any values above this absolute value that have been identified as being anomalies (i.e. at odds with the data surrounding it)
* `Variance (%)` - this will smooth any values which are higher than this percentage of the rolling average wattage for the 30 seconds leading up to the spike.

BACK: [Special Topics: Overview](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Special-Topics_Overview)