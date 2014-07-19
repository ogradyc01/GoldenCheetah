Special Topics: Setting the athlete library (Version 3.1)
***

Overall GoldenCheetah configuration is explaind here: [Preferences: Overview] (http://github.com/GoldenCheetah/GoldenCheetah/wiki/Preferences_Overview)

A special setting when starting with GoldenCheetah is setting your 'Athlete Library'. This library is actually a directory in your file system. You can either enter a directory name manually in the entry field next to 'Athlete Library' or you use `Browse` to select one.

When changing your library, the athlete(s) of your current library (in case of an emptry entry the GoldenCheetah default library) cannot longer be accessed through 'Menu Bar' function to 'Open' an existing athlet. The 'Athlete Library' which is actively used when you run GoldenCheetah can be retrieved by 

_Select:_ `Menu Bar -> Help -> About GoldenCheetah` This opens a popup like below, which shows the current path of your 'Athlete Library'

[Preferences - General] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/PreferencesGeneral.jpg)

GoldenCheetah is not removing your old 'Athlete Library' or deleting any athlete data stored in it. After changing your 'Athlete Library' you can alway switch back to the previous one, but there is currently no feature to move or copy athletes from one library to another.

After selecting a new 'Athlete Library' which is recommended to be an EMPTY directory of your system, you need either to manually takeover your data from the previous library. Or you start with a new athlete in your new library.

When pressing `Save` on the info popup after changing the 'Athlete Library', GoldenCheetah will restart for the change to take effect. If you changed to an empty 'Athlete Library' the 'Choose an Athlete' popup appears, allowing you to create a new athlete. Further information see: [First Steps: Your first athlete](https://github.com/GoldenCheetah/GoldenCheetah/wiki/First-Steps_Your-first-athlete)

 _Note: It is recommended to use either use only one athlete library OR if you need multiple athlete libraries, to use distinct athlete names - even across the libraries. Reason is that parts of the configuration data is currently stored 'per athlet', but not 'per libary/athlet'. Meaning if you use the same athlet name in multiple libraries they will share the athlet dependent parts options/configuration, but not the same rides,..._