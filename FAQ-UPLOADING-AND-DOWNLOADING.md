## UPLOADING AND DOWNLOADING


### How to fix permission denied ?

When downloading from a Joule, Osynce, Powertap, SRM or Moxy over a serial port on Linux you may see a permission denied error -- this is because you are not a member of the "dialout" user group that owns the serial device.

To fix it add the user to the dialout group on the command line. This is done with the command "sudo usermod -aG dialout _USERNAME_" where _USERNAME_ is replaced with your login name. You will need to logout and log back in again for the change to take effect.

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

<https://apidata.googleusercontent.com/caldav/v2/xxxx@@gmail.com/events/>


Where xxxx is your username. The username will need to be repeated in the username
field and obviously set the password too.

**NOTE**: that the previous address has now been deprecated, those were of the form <https://www.google.com/calendar/dav/xxxx@@gmail.com/events/>


### When setting up my Withings wifi scales where do I get the userid and key ?

As of Nov 2015 Withings are migrating to a new web interface and some of the old functionality is still in transition. It is quite hard to find the details as a result !

This is the advice provided by Withings to get to the old functionality you need.

```
You should still be able to access it by following these steps:

Login to https://healthmate.withings.com
Click on your email address in the upper right corner of screen and select Settings from the dropdown menu
Under Devices click the button to Configure a WBS01
On the next screen click My Dashboard
You'll arrive at the old interface with the Share option
Please note that this interface is no longer supported so we would not be able to account for any potential software bugs. We are working to migrate as many features of this interface as possible over to the new interface, though I do not have a timeline that I am able to provide at the moment.


Withings Customer Service | Inspire Health```

If you click on 'share on my website' you will be greeted with a number of code
snippets you can embed in a web page. If you look closely in the top right hand
corner there will be a box containing the user id and public key. These are the
two values you need to enter into the options dialog.

You will now be able to retrieve withings data via the tools menu.