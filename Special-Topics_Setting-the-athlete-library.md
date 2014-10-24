Special Topics: Setting the athlete library (Version 3.1)
***

Overall GoldenCheetah configuration is explained here: [Preferences: Overview] (http://github.com/GoldenCheetah/GoldenCheetah/wiki/Preferences_Overview)

A special setting when starting with GoldenCheetah is setting your 'Athlete Library'. This library is actually a directory in your file system. You can either enter a directory name manually in the entry field next to 'Athlete Library' or you use `Browse` to select one.

When changing your library, the athlete(s) of your current library (in case of an empty entry the GoldenCheetah default library) cannot longer be accessed through 'Menu Bar' function to 'Open' an existing athlete. The 'Athlete Library' which is active/valid when you run GoldenCheetah can be retrieved by 

_Select:_ `Menu Bar -> Help -> About GoldenCheetah` - this opens a dialog box similar to the one below, which shows the path of your currently active 'Athlete Library'

![Help - About] (https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/Help_About.JPG)

When changing your 'Athlete Library' path, GoldenCheetah is not removing your old 'Athlete Library' or deleting any athlete data stored in it. After changing your 'Athlete Library' you can always switch back to the previous one, but there is currently no feature to move or copy athletes from one library to another.

After selecting a new 'Athlete Library', which is recommended to be an EMPTY directory of your system, you need either to manually takeover your data from the previous library. Or you start with a new athlete in your new library.

When pressing `Save` on the info popup after changing the 'Athlete Library', GoldenCheetah will restart for the change to take effect. If you changed to an empty 'Athlete Library' the 'Choose an Athlete' dialog box appears, allowing you to create a new athlete. Further information see: [First Steps: Your first athlete](https://github.com/GoldenCheetah/GoldenCheetah/wiki/First-Steps_Your-first-athlete)

 _Note: It is recommended to either use only one athlete library OR if you need multiple athlete libraries, to use different athlete names - even across the libraries. Reason is that parts of the preferences of GoldenCheetah is currently stored 'per athlete', but not 'per library/athlete'. If you use the same athlete name in multiple libraries, this athlete will share the athlete dependent preferences, but not the same rides,..._

BACK: [Overview] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Main-Page_Users-Guide)