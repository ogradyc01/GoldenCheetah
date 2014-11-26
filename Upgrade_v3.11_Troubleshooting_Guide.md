Upgrade Troubleshooting (Version 3.11)
***

# Information

With Version 3.11 the 'Athlete' directory has been refactored by adding a set of sub-directory which hold the different types of GoldenCheetah files. 

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

Please be aware that upgrades process is done for an athlete until it finally reports success, which is that the upgrade reports ZERO errors (there still may be some information messages). This is to ensure that you take care on the problems and fixed them actively instead of just putting them aside and at a later stage find out that portions of your training data has not been upgraded - and therefore is not visible in GoldenCheetah any more.

We saw multiple issues while moving and converting the data and want to give some hints how to fix the problems.

## Read first

Before you start to manually clean up the problems - we recommend to backup also the intermediate stage of your athlete data - to be able to go back to that stage in case of mistaken deletions, etc.

## Files in athlete directory cannot be deleted

A frequent problem is that source files in the athlete directory cannot be deleted after they have been copied to the appropriate sub-directory. Since we have chosen an 2-step process (1st we copy the file to the sub-directory, 2nd we delete the file on the source directory) - this problem does (in the known cases) not affect the integrity of the upgraded athlete data. 

Why does this happen: We have seen cases where deletion of files did not work if the athlete directory was on dropbox, we have seen single files which could not be deleted (without any clear reason). There might also be authorization problems, etc. - so various reasons possible.

What to do: Check if the file exists in the respective sub-directory - if yes, delete the source file manuall

## Ride/Activity files fail to convert to GoldenCheetah .JSON

The Upgrade process uses the same conversion procedure which is used by all other part of GoldenCheetah. Still we found cases where a file could not be converted during upgrade - which converted perfectly fine when using the manual "Import from ..." feature of GoldenCheetah.

What to do: Import the non-converted files manually through "Import from ..." - if this import works fine and the ride/activity get visible in your rides list, just move the file manually to /imports or /downloads sub-directory (to keep the original).

## Files cannot not be moved to the sub-folders

...