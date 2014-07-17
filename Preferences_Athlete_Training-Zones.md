Preferences: Athlete: Training Zones (Version 3.1)
***

_Select:_ `Menu Bar -> Tools -> Options...` to get to the 'Preferences' window.

Setting up the training zones for 'Power' and 'Heartrate' is done a a very similar way. Therefore here only the setup for 'Power' is described in details - and for 'Heartrate' just the small differences are outlined.

![Athlete - Power - Overview] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/PreferencesAthlete_Power_Overview.jpg)

### Create New (for Power):

* From Date: Each set of training zones is defined with a specific 'From Date' - as we assume your zones change over time. 

* Critical Power: This is your CP (abbreviation for CP60) - computed using the Scherer/Monod protocol using 3 and 20 minutes. A seconds threshold which is commonly used in power metrics is FTP (Functional threshold power). In GoldenCheetah all metrics (whether they are defined for CP, or for FTP) are computed using the value defined in the 'Critical Power' field. So depending on which metrics you want to use, you need to set this field accordingly (either th CP60 or FTP). In all UI texts in GoldenCheetah the value is referenced as 'CP' or 'Critical Power'. You need to consider which value you have used, if you compare metrics computed by GoldenCheetah to metrics calculated by other tools.

* W': (spoken W Prime) is (very simplified) the work you can deliver above CP (in Joules/kJ). It's important to be set and is also part of the CP estimator. ´Menu Bar -> xxx -> yyy´. There are some more metrics related to it e.g. 'Minimum W'bal' and 'Maximum W' match'.

* '+' or 'Add' button: Depending on your operating system, you will see either +/- buttons or Add/Delete buttons on the screen. '+' or 'Add' is used to create a new set of zones using the data you entered in the 'Create New' section of the screen. Newly added sets appear in the 'Zones Header' section. And if you select a line in the 'Zones Header' section, the 'Zones Details' section shows the different Zones for this line.

* '-' or 'Delete' button: The '-' or 'Delete' button removes the entry marked in the 'Zones Header' section from your defined zones. 

_Note: Any changes on of data is only stored if you press 'Save'. The system does not check on changes if you leave the screen with 'Close', but will just discard whatever you have changed._

The screen has two tabs again, namely 'Critical Power' and 'Default'. It's important to understand the concept of 'Default' as this can save you a lot of time.

### Zones/Default Tab

Before proceeding to the 'Zones Details' and editing them, it's very valuable and time saving to understand the purpose of the 'Default' tab.

![Athlete - Power - Default] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/PreferencesAthlete_Power_Default.jpg)

For 'Power' the 'Default' tab lists the common Power Zones Z1 to Z2 as a 'Short' text code, 'Long' descriptive text and the value 'Percent of CP'. This default is used as basis for any new zones you create on the 'Critical Power' tab. That means, if you want to have your zones created differently for all your zone entries in future, the 'Default' settings are the place to do these changes once.

At the lower/right corner of the screen, you also find the '+/-' or 'Add/Delete' buttons. With those you can Add new zones to your default, or you can remove zones. (Please observe: Maximum number of zones supported is 10). And you can also change both the 'Short' and 'Long' texts for a zone. This is done by moving the mouse cursor over the text to be changed and 'click' on the text. In case the line of the text you want to change was not active, the first click makes the line active, and a second click opens the text field for input.

_Note: Any changes of the default settings are automatically applied to all actual zones records, which are listed in the 'Zones Header' section, as long as you have not done any specific changes to that zone record in the 'Zones details' section. Zone records which have individual changes are display in 'Bold'._

### Zones Header

The 'Zones Header' section shows the zone records you have created sorted by 'From Date'. When creating all the 
detailed zones are created based on the definition configured in the 'Default' tab. In case you have changed any of the zone data in the 'Zone detail' section, this text for this records will be displayed in 'Bold' characters, and when selection such a record in the 'Zone Header' section an additional button 'Def' appears. By using this button you can reset the respective to 'Default'. 

![Athlete - Power - Def.] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/PreferencesAthlete_Power_Def.jpg)


### Zones Details

The 'Zones Details' work very similar to the 'Default' tab. You can change 'Short' and 'Long' text, you can add or remove zones and you can define the zone value. Difference here is that the value is not defined as 'Percent of CP' but as absolute 'Watts'.

If you edit anything in 'Zones Details' the zone record will immediately change to 'Bold' display to make you aware.

## Difference for Heartrate

The difference in zone creation for heartrate are quite small since the UI is mainly the same as for power. 

### Create New (for heartrate):

![Athlete - HR - Overview] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/PreferencesAthlete_HR_Overview.jpg)

* From Date: Each set of training zones is defined with a specific 'From Date' - as we assume your zones change over time. 

* Lactate Threshold: The lactate threshold heart rate (LTHR) (or anaerobic threshold (AT)) is the exercise intensity at which lactate (more specifically, lactic acid) starts to accumulate in the blood stream. The value entered here is - like CP for power - important for GoldenCheetah metrics calculations. (As it e.g. sets the border betwen aerobic and anaerobic exercises.)

* Rest HR: Heartrate when resting

* Max HR: Maximum heartrate

### Zones Details / Default Tab

Zones can be added, removed, renamed in same way as 'Power'. 

Values are:

* Default Tab - Percent of LT (Lactate threshold heartrate)
* Default Tab - Trimp k
* Zones Details - From BPM (Heartrate)
* Zones Details - Trimp k

Back: [Preferences: Athlete] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Preferences_Athlete)



 