## DATA

### Where is ride data stored?

By default data will be stored in operating system specific directories, assuming you have not changed the location in preferences.

On Apple OS X the data is stored in Library/GoldenCheetah/name in your home directory. On Linux the data is stored in .goldencheetah/name in your home directory. On Microsoft Windows application data folders seemingly change with each release, but typically will be found in AppData within your user home directory (which my be hidden by default).

To assist the about dialog lists the folder where ride data is stored.

### How do I split, merge or join files?

You can split a file by time using the activity->split ride menu item (or toolbar button).

To join two rides together (making one longer ride from two rides) you can copy rows
in the activity editor and paste special in the ride editor (right click) and then select
append mode.

If you wish to merge rides, in v3.1 there is a new Activity->Merge wizard that will walk
you through merging ride files and also provide the ability to synchronise timestamps.



### How can I find 'spikes' or specific values in activity data?

The activity editor has a function to find data on its toolbar. You can specify a range
or upper or lower limit and find values less than, greater than or between a range of values.

Additionally, the editor will scan the file looking for anomalies -- where the data
appears to be out of normal ranges. These are shown with a wiggly red line in the editor
and can also be listed by clicking on the anomalies icon on the editor toolbar.

If the anomalies icon is not enabled on the toolbar then there are no anomalies in the
currently selected ride.



### How can I fix 'spikes' or 'anomalies' in activity data?

You can either manually edit the values in the activity editor (there is full undo and
redo in the editor). Or you can use the fix tools that are listed under the tool menu
option (fix power spikes, fix gaps in recording, fix gps errors, fix torque.

Each of the fix tools opens a dialog that displays texts to explain what the fix tool does.



### How can I add/remove a field to edit on the details screen?

The fields (metadata) that is editable can be configured in the preferences pane under
the data fields tab. Where no screen is specified (its left blank) it will not be made
available.

GoldenCheetah ships with a number of fields defined in the config but with no screen set.
If you wish to use them simply set the screen tab to the tab you would like it to be
shown on. To remove a field set the field tab to blank.



### What are 'special fields' ?

There are a number of fields that when maintained in the details screen will be used
elsewhere in the code to calculate metrics or for other purposes.

Some examples include;

Weight - used in W/KG calculations, Sport and Workout code are
used  when exporting to other file formats, Identifier is used to assign a UUID to the
activity when it is uploaded to online services and so on.

There is a full list of special fields and their meaning in the Golden Cheetah user
guide appendices.



### How do I find/add/sort/delete/edit intervals ?

The context menu (on the right hand side of the splitter handle) for the interval
sidebar in Analysis view contains a number of options for working with intervals.

Additionally, you can click and drag on the performance (aka ride) plot to visually
define an interval.



### How can I export to a specific file format?

Activity->Export allows you to export the activity to csv, fitlog, gc (xml), json,
Training Peaks PWX or Garmin TCX format.



### Can I use GC to convert data from one format to another on the command line?

No. It is something we may add in v3.2



### Can I delete an athlete and all his/her data?

No. It must be done manually by removing the athlete directory via the operating
system. Please ensure you do this when GoldenCheetah is not running.
