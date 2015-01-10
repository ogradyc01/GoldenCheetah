## METRICS


### What is the difference between xPower, NP and Daniels EqP?

They all serve the same purpose -- to express the variable power you have generated over
a given period of time as a single value. This is so you can quantify the intensity of
the ride and therefore the training stress of the ride.

In practice, NP and xPower are largely the same, whilst Daniels EqP place much higher
emphasise on upper intensity work. For more info on xPower see Dr Skiba's paper on BikeScore
<http://www.physfarm.com/bikescore.pdf>



### What is the difference between CP and FTP?

CP represents the power an athlete can sustain for a very long time, without fatigue, in theory. It is calculated using a model and time to exhaustion tests of 2 and 12 or 20 minutes. Functional Threshold Power (FTP) is an estimate of the power an athlete can sustain for about 60 minutes or a 40km TT. There is no formal model or protocol for establishing it, most people use rules of thumb like FTP is 95% of 20 minute power, or they use the best power from a 40km TT. 

In practice, CP and FTP are usually close to each other. But since it is very difficult for an athlete to maintain the desired intensity FTP 'reality' tends to result in a number that is much lower than CP 'theory'. Often users will consider the two as the same.

In GC we compute TSS and BikeScore using your 'CP' value. If you set it to your FTP value
TSS will be accurate, BikeScore is likely to be lower. And if you set it to your CP value
BikeScore will be accurate, but TSS will be overstated.



### Why does my CP chart show higher watts for a longer duration?

A higher power average for a longer time is possible if an effort has been "book ended".
If, for example, you did a massive 30 second effort, followed by freewheeling for 29:30
then another massive 30 second effort, then your best average for a continuous 30 minutes
would in fact be lower that your best average for a continuous 30minutes and 30 seconds.
(Thanks for Jon Hill from the Golden Cheetah Users mailing list for this example).



### Can I set a different CP/FTP for different reasons e.g. CP/FTP on a trainer?

We allow you to override the CP value for a specific ride by setting the "CP" field to
the value you wish to use for the ride in question. We do not have a concept of 'separate'
Cps for different purposes -- you will need to specify the CP when the data is imported
into GC. But this allows you to make manual adjustments.

We provide this functionality at user request -- we do not endorse the concept of multiple
CP values. But we do recognise the ongoing debate regarding physiological stress from
working on a trainer vs on the road.


### How do I seed the CTL for my PMC?

You can seed the starting CTL (we call it LTS, for long term stress) when you define a
season. That way it is re-usable in a number of places. To do this you edit the season
(date range) in the Home View and can set the Starting LTS.

### Why is elevation different in GoldenCheetah to my other training software / website?

Different programs will use different hysteresis values to smooth the small changes in
altitude. In GC we use a hysteresis value of 3m.

If this is of great concern you can adjust the hysteresis value in preferences under the
general tab.



### Why is a metric e.g. TSS or average power different in GoldenCheetah to Garmin Connect?

The algorithms for calculating TSS, AP etc are static. They are implemented exactly the
same way in GoldenCheetah, Garmin Connect, TrainingPeaks etc. The algorithms are extremely
simple and not prone to difficulty in implementation.

However, how each application treats pauses and stops or loss of data accounts for most
differences. In GoldenCheetah we always calculate AP,TSS etc including stop time. Other
applications choose to ignore or smooth segments of short duration.

In addition, if there are anomalies in your data, with large gaps or even time going
backwards, this will drastically affect GoldenCheetah's calculations.

We NEVER attempt to interpret data anomalies -- if the results are not as you would expect
you will need to correct the data. We do not 'silently' fix the data for you. There is no
secret sauce in GoldenCheetah, we are open and transparent with your data.



### How do I set the metrics shown for intervals in the various summaries?

In the GoldenCheetah preference pane under the Metrics tab you can choose the metrics
that will be shown in the ride summary charts and the metrics that will be shown in the
interval summary in the analysis sidebar.



### How do I add a metric to the details screen (so I can override it) ?

If the metric you want (e.g. TSS) is not shown then you will need to add it via the
GoldenCheetah preferences pane. On Mac this is from the menu option
GoldenCheetah->Preferences whilst on Windows and Linux it is under Tools->Options.

You will need to select 'Data Fields' option from preferences toolbar and then the
'fields' tab. You will see a list of fields that are associated with a particular screen
tab. If you scroll down you should find entries for the 'Metrics' screen tab, you can
insert a new entry here with the '+' button. You should make sure the new entry is
called exactly the same thing as the metric in question.

For 'TSS' this is relatively straight forward. For others, e.g. 'Average Heart Rate' you
must make sure that the name includes spaces etc. Once your metric has been added to the
configuration you should save that and return to the details screen where you can now
maintain it.

If you are creating a manual entry then there is no 'details' tab in the dialog. Once
you have created the entry (and again in this case TSS can be entered in the dialog)
you should go to the details tab to maintain any other specific fields. The manual entry
dialog is designed to be simple and accept only the most common of entries.



### Can you calculate gradient, virtual power or other derived series from the ride data?

Not in 3.1. We have implemented virtual power, slope and some other derived series in v3.11
which is due for release Q1 2014.



### Can I export metrics or access the metric database GC uses?

The metrics are stored within a Sqlite 3 Database called 'metricDBv3' that can be found
in the athlete directory. You can use any Sqlite 3 tools to query and work with the db.

Alternatively you can export the db in its entirety using the Activity->Export Metrics
as CSV to export to a format you can use in a spreadsheet program.
