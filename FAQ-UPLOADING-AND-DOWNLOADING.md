## UPLOADING AND DOWNLOADING


### How to fix permission denied ?

When downloading from a Joule, Osynce, Powertap, SRM or Moxy over a serial port on Linux you may see a permission denied error -- this is because you are not a member of the "dialout" user group that owns the serial device.

To fix it add the user to the dialout group on the command line. This is done with the command "sudo usermod -a -G dialout _USERNAME_" where _USERNAME_ is replaced with your login name. You will need to logout and log back in again for the change to take effect.

### Why does upload to TrainingPeaks keep failing?

The Sport field in TrainingPeaks must have very specific values, although this is not
documented in the XML Schema. We recommend using a sport of "Bike" if you plan on
uploading rides to training peaks.



### Why does download from TrainingPeaks say I need a premium account?

Training Peaks only allow paid up members to get access to their data. If you are
using a free service they do not let you retrieve your data.



### What settings do I need to get GoldenCheetah to upload to my Google Calendar?

The upload to Google Calendar uses their CalDAV API, and as such needs to specify a
collection. This means when entering the details in the passwords pane of preferences
you should use the following for the caldav url:

<https://www.google.com/calendar/dav/xxxx@@gmail.com/events/>

Where xxxx is your username. The username will need to be repeated in the username
field and obviously set the password too.


### When setting up my Withings wifi scales where do I get the userid and key ?

You will need to login to your Withings account (<http://my.withings.com>) and
click on the 'share' button at the top of the dashboard. From there you will get a
popup box with lots of options.

If you click on 'share on my website' you will be greeted with a number of code
snippets you can embed in a web page. If you look closely in the top right hand
corner there will be a box containing the user id and public key. These are the
two values you need to enter into the options dialog.

You will now be able to retrieve withings data via the tools menu.
