## MOST COMMON QUESTIONS OF ALL


### How do I override / manually enter TSS for a ride?

The details chart on the analysis view allows you to override metrics on the metrics tab.
By default the most common metrics are listed, including average HR, distance and so on.
From v3.1 the default setup will also include TSS as a metric you can override here.

If the metric is not there you will need to configure GoldenCheetah to allow it to be shown.
This is simple to do and described in 3.9 below. The 3.1 upgrade process should have added it
to the Metric tab if it was not already there.

### How do I add or remove a chart?

To add a new chart to the view you can select from the hamburger menu on the right hand side of
the chart bar.

Depending upon which view you are on the charts available will differ. For example realtime
plots only appear on the Train view, whilst charts that work with individual rides will only
appear on the analysis view.

To remove a chart, when you mouse over a chart (in tabbed or tiled mode) the word 'More...'
will appear in the top left of the chart. This is a menu drop down, if you click on it
you will see a 'Close' option. This is the option to remove (close) the chart.

### Can I enter my weight and track/plot it?

Weight can be maintained in 3 ways;


* Every athlete is setup with a weight value -- this is the fallback value should no
other weight measure be available. It can be found under preferences and athlete.

* The 'Weight' field can be maintained in the details screen. This is found on the
'Workout' tab in the details screen by default. Any entry here will be used for this ride
ONLY. If 'Weight' is not listed then you will need to add this to the 'Workout' tab - [How to add a Metric to the Details screen] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/FAQ-METRICS#how-do-i-add-a-metric-to-the-details-screen-so-i-can-override-it-)

* You can download weight from a withings scale. This is performed manually via the
menu option Tools->Get Withings Data. This is then used to update the local measures
database.

When calculating W/KG the Activity value is used if present, if not we then fall back to
the last Withing measure that was collected, and if that is not available we then fall
back to the default value for the athlete.

The weight from withings and weight from the activity can both be plotted separately in
the LTM plots.



### How do I plot x sec power best?

In v3.1 it is now possible to plot custom durations for any data series on a metric
trends chart in the Trends view. You will need to add a curve for the data series
and select 'Best' instead of 'Metric' or 'Estimate' on the curve settings.

For v3.0 or earlier it is still not possible to plot custom durations for power bests. We are
looking to add this in version 3.1, but for now you can only plot 1s, 5s, 10s, 15s, 20s,
30s, 1min, 2min, 5min, 10min, 20min, 30min and 60min bests.



### I can't find Aerolab / Performance Manager?

By default we do not add these charts to the layout. Aerolab can be added to the Analysis
view via the '+' menu found to the right hand side of the GoldenCheetah scope bar.

The Performance manager has been deprecated in preference for using a trends chart
and we have added 3 PMC style charts to the chart library to help transition. 

We will be adding an 'interactive' PMC in v3.2 to support planning and this will allow
you to set goals and drag the curves/load to set and adjust your plan, before looking at
specific workouts -- but this won't be available till 2015.



### What happened to weekly summary?

It has been deprecated since the Diary view allows you to summarise by day, week and month
and add charts to the view that summarise for the selection. As the weekly summary was fixed
on specific charts and did not handle other selections (e.g. monthly) it has been deprecated
in view of the diary view.

At present you can treat the Diary view as you would have the weekly summary -- they offer
the same functionality. We expect the diary view to extend to planned workouts when we
implement planning functionality in v3.1.



### Where are all the chart settings?

All chart settings can be found under the drop down menu that appears in the top left hand
corner of a chart when you mouse over it, titled 'More...'. They will appear as a popup dialog box.

Additionally, when you move the cursor towards the title of a chart in a view that is tabbed
(not tiled) then a small selection of the most important settings for the chart will appear
for convenience.

### Where is the preferences / options panel?

On a Mac the configurations page can be found under 'GoldenCheetah -> Preferences' on the
main menu. Whilst on all other platforms it is found via 'Tools -> Options'.

We do this to match the general guidelines for the operating system.

### How do I change the colour of the rides on the calendar/list?

Activities are coloured according to keywords embedded in their details (metadata) you can
configure the field that is used and the values that are matched and the colours they are
shown in from the preferences pane via the 'Data Fields' toolbar option then select Notes
Processing. The keywords and related words are scanned for to determine if the associated
colour should be used for this ride.

They are processed in the order they are defined with the first match being returned. Take
care when using values such as 'TT' and 'race' since these can also be part of an English
word (e.g. ATTEMPT contains 'TT' and graceful contains 'race'.

### GoldenCheetah doesn't find my PowerTap/Joule/SRM on Ubuntu Linux.

If you're using the USB cradle (as opposed to the older, serial one), the FTDI driver sometimes
conflicts with the braille terminal in the default Ubuntu installation. Try unplugging the PT cradle
from the computer and uninstalling brltty: 
```
$ sudo apt-get remove brltty
```
Then plug the device back in and it should work.

### GoldenCheetah.dmg installation didn't seem to work.

Are you running OS X Snow Leopard (10.6) or later? You need to be. If you are, and you're still
having this problem, open Terminal (in Applications -> Utilities) and type this at the prompt:

/Applications/GoldenCheetah.app/Contents/MacOS/GoldenCheetah then press \<return>
and send an email to the mailing list with whatever it prints out. We'll help you debug it.
