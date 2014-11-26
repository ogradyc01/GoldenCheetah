Upgrade Troubleshooting (Version 3.11)
***

# Information

With Version 3.11 the 'Athlete' directory has been refactored by adding a set of subdirectory which hold the different types of GoldenCheetah files. 

The new structure is:
- Activity/Ride files: <samp>/activities</samp>
- Configuration files: <samp>/config</samp>
- Download files: <samp>/downloads</samp>
- Import files: <samp>/imports</samp>
- Workout related files: <samp>/workouts</samp>
- Cache files: <samp>/cache</samp>
- Calendar files: <samp>/calendar</samp>
- Log files: <samp>/logs</samp>
- Temp files: <samp>/temp</samp>

The upgrade process creates the new directory structure and moves the existing files to the new directories as needed. During the upgrade all activity/ride files are converted to GoldenCheetah's native file format .JSON and moved to the <br><samp>/activities</samp> folder. The source files are moved to the <samp>/imports</samp> folder.

Starting with version 3.11 all downloads from devices or imported activity/ride files are converted to GoldenCheetah's file format during import/download. The original files are (depending on the source)                     in <samp>/downloads</samp> or <br><samp>/imports</samp> folder.

We assume that you have backed up your athlete data before you started the upgrade process. Even though the upgrade process has carefully been implemented and tested we can't take responsibility for any loss of data during the process. 

# Troubleshooting


