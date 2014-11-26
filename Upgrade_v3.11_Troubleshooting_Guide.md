Upgrade Troubleshooting (Version 3.11)
***

# Information

Backup your 'Athlete' data first!Please read carefully before proceeding! With Version 3.11 the 'Athlete' directory has been refactored by adding a set of subdirectory which hold the different types of GoldenCheetah files. 

The new structure is:
-> Activity/Ride files: <samp>/activities</samp><br>"
-> Configuration files: <samp>/config</samp><br>"
-> Download files: <samp>/downloads</samp><br>"
-> Import files: <samp>/imports</samp><br>"
-> Workout related files: <samp>/workouts</samp><br>"
-> Cache files: <samp>/cache</samp><br>"
-> Calendar files: <samp>/calendar</samp><br>"
-> Log files: <samp>/logs</samp><br>"
-> Temp files: <samp>/temp</samp><br><br>"

The upgrade process will create the new directory structure and move the existing files to the new directories as needed. During the upgrade all activity/ride files will be converted to GoldenCheetah's native file format .JSON and moved to the <br><samp>/activities</samp> folder. The source files are moved to the <samp>/imports</samp> folder.

Starting with version 3.11 all downloads from devices or imported activity/ride files will be converted to GoldenCheetah's file format during import/download. The original files will be stored - depending on the source -                     in <samp>/downloads</samp> or <br><samp>/imports</samp> folder.

Please make sure that you have done a backup of your athlete data before proceeding with the upgrade. We can't take responsibility for any loss of data during the process. 

# Troubleshooting


