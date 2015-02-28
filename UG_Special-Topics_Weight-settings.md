Special Topics: Weight settings (Version 3.2)
***

Weight can be maintained in 3 ways:
* Every athlete is setup with a weight value - this is the fallback value should no other weight measure be available. It can be found under [Preferences: Athlete](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Preferences_General)

* The 'Weight' field can be maintained for every activity. This is found on the 'Workout' tab in the details screen by default. Any entry here will be used for this activity ONLY.
If 'Weight' is not listed then you will need to add this to the 'Workout' tab - [How to add a Metric to the Details screen](https://github.com/GoldenCheetah/GoldenCheetah/wiki/FAQ-METRICS#how-do-i-add-a-metric-to-the-details-screen-so-i-can-overactivity-it-). NB Ensure weight is defined as "Double".  

* You can download weight from a withings scale. This is performed manually via the menu option `'Tools->Get Withings Data...'`. This is then used to update the local measures
database.

_Note: When calculating W/KG the activity specific value is used if present, if not we then fall back to the last Withing measure that was collected, and if that is not available we then fall back to the default value for the athlete. The weight from Withings and weight from the activity can both be plotted separately in
the 'Metric Trends' chart(s) of 'Trends' view._


BACK: [Special Topics: Overview](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Special-Topics_Overview)