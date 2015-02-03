Upgrade Troubleshooting (Version 3.2)
***

# Information

With Version 3.2 the 'Athlete' directory has been refactored by adding a set of sub-directory which hold the different types of GoldenCheetah files. 

The new structure is:
- Activity/Ride files: <samp>/activities</samp>
- Configuration files: <samp>/config</samp>
- Download files: <samp>/downloads</samp>
- Import files: <samp>/imports</samp>
- Backups of Activity/Ride files: <samp>/bak</samp>
- Workout related files: <samp>/workouts</samp>
- Cache files: <samp>/cache</samp>
- Calendar files: <samp>/calendar</samp>
- Log files: <samp>/logs</samp>
- Temp files: <samp>/temp</samp>
- Temp for Activities: <samp>/tempActivities</samp>
- Train View recordings: <samp>/recordings</samp>
- Quarantined files: <samp>/quarantine</samp><br>

The upgrade process creates the new directory structure and moves the existing files to the new directories as needed. During the upgrade all activity/ride files are converted to GoldenCheetah's native file format .JSON and moved to the <br><samp>/activities</samp> folder. The source files are moved to the <samp>/imports</samp> folder.

Starting with version 3.2 all downloads from devices or imported activity/ride files are converted to GoldenCheetah's file format during import/download. The original files are (depending on the source)                     in <samp>/downloads</samp> or <br><samp>/imports</samp> folder.

We assume that you have backed up your athlete data before you started the upgrade process. Even though the upgrade process has carefully been implemented and tested we can't take responsibility for any loss of data during the process. 

# Troubleshooting

Please be aware that upgrades process is done for an athlete until it finally reports success, which is that the upgrade reports ZERO errors (there still may be some information messages). This is to ensure that you take care on the problems and fixed them actively instead of just putting them aside and at a later stage find out that portions of your training data has not been upgraded - and therefore is not visible in GoldenCheetah any more.

We saw multiple issues while moving and converting the data and want to give some hints how to fix the problems.

## Read first

Before you start to manually clean up the problems - we recommend to backup also the intermediate stage of your athlete data - to be able to go back to that stage in case of mistaken deletions, etc.

## Files in athlete directory cannot be deleted

A frequent problem is that source files in the athlete directory cannot be deleted after they have been copied to the appropriate sub-directory. Since we have chosen an 2-step process (1st we copy the file to the sub-directory, 2nd we delete the file on the source directory) - this problem does (in the known cases) not affect the integrity of the upgraded athlete data. 

Why does this happen: We have seen cases where deletion of files did not work if the athlete directory was on dropbox, we have seen single files which could not be deleted (without any clear reason). There might also be authorization problems, etc. - so various reasons possible.

_What to do:_

_Check if the file exists in the respective sub-directory - if yes, delete the source file manually._

## Activity files fail to convert to GoldenCheetah .JSON

The Upgrade process uses the same conversion procedure which is used by all other part of GoldenCheetah. Still we found cases where a file could not be converted during upgrade - which converted perfectly fine when using the manual "Import from ..." feature of GoldenCheetah.

_What to do:_

_Import the non-converted files manually through "Import from ..." - if this import works fine and the ride/activity get visible in your rides list, just MOVE the file manually to /imports or /downloads sub-directory (to keep the original)._

## Activity files - Invalid File name for upgrade conversion

When importing / downloading a file to GoldenCheetah (before 3.2) the original file type was kept, but the file name was converted following the convention "YYYY_MM_DD_HH_MM_SS.***". Since not all original file types do not contain day/time of the activity in their data, this is the way to have a consistent source for this important information across all activity files on GoldenCheetah. And it makes sure that the file names are distinct and do not conflict/overlap.

If - for whatever historic reason - still activities file(s) exist in the athlete's activity folder which DO NOT follow this convention they are NOT considered in the conversion to .JSON + stored in /activities but are reported as erroneous and will stay unchanged in the athlete directory.

_What to do:_

_Variant a) Rename the file name to follow the required convention (here you have to make sure that date/time are correct) and restart GoldenCheetah to re-check/re-run the upgrade process_

_Variant b) Try to import the file into GoldenCheetah again using manual "Import from ..." - the import creates the .JSON in /activities. If the import is SUCCESSFUL we recommend to MOVE the file manually to /imports or /downloads sub-directory (to keep the original)._

## Files cannot not be moved to the sub-folders

Depending on OS/File Source/... there are cases where a file cannot be moved the the sub-folder, or the file can be moved, but the source file cannot be deleted - so the upgrade process reports errors.

_What to do:_

_Check the files and errors - as they are reported in the upgrade log. In case a file is properly moved, but cannot be deleted - make a backup copy of the file to another place (just in case) and remove the file manually. If the file could neither be copied nor moved - check the file properties - and the type of file. Depending if you still need the file / or it was a file not required by GoldenCheetah any more (make a backup copy as well) and delete._

_Note: The responsibility if a file is required or not / if you delete it is totally yours. - Sorry - please use the information given here to make your decision_

...