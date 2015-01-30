Preferences: Data Fields (Version 3.1)
***

_Select:_ `Menu Bar -> Tools -> Options...` to get to the 'Options' Popup.

The 'Data Fields' preferences cover three different areas:

* [Fields](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Preferences_Data-Fields#fields) - here you define the list of additional fields available to either store additional activity data and to add/overwrite activity data.

* [Notes Keywords](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Preferences_Data-Fields#notes-keywords) - defines the rules, how your activities are "colored" in the calendar(s), in the activity list of the 'Diary' view and in the activities section of the 'Activities' view.

* [Processing](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Preferences_Data-Fields#processing) - allows the configuration of the 'Fix/adjust/correct' tools build into GoldenCheetah.

### Fields

![Preferences - Datafields - Fields](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/PreferencesDataFields_Fields.jpg)

The data fields are structured by 'Screen Tab's which then appear on the 'Activities' view in the 'Details' and 'Summary and Details' charts. Please do also read the description of the ['Details' Chart](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_Activities#details).

* `Screen Tab` - groups the fields on different tabs 
* `Field` - name of the field - there are 2 cases to consider (1) you to add a completely new field: then make sure that it has a name, which is not used elsewhere in GoldenCheetah (2) you want to make an existing field of GoldenCheetah editable, then please use exactly the field name here and make sure that you assign the correct field type

_Important Note: For case (1) - a completely new field, it is recommended to use only "0-9", "a-z" or "A-Z" and "space" in the field name. Only those characters are recognized as part of a 'field name' by the 'Filter' tool in GoldenCheetah. If you use any other character e.g. "-" or a language specific character like "ä", you will not be able to create any 'Filter' queries for this new field._

* `Type` - technical type of a field - in case of existing GoldenCheetah fields, please use the correct field type (to understand the field types, please have a look at the standard examples GoldenCheetah is providing).
* `Values` - is a way to restrict and simplify the input into fields of type 'Text' and 'Short Text' - by adding a list of values, seperated by "," for a specific field, only those values can be entered into that particular field
* `Diary` - if checked, the concatenated contents of all checked fields is show in the 'Activities' view - 'Side Bar' -> 'Activities Pane' and also in the 'Diary' view - 'Calendar' chart.

_Note: You can use this to enter data for activities, where certain data was not captured at all, or to overwrite/correct certain values_

### Notes Keywords

![Preferences - Datafields - NotesKeywords](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/PreferencesDataFields_NotesKeywords.jpg)

The section 'Notes Keywords' defines which field / field content is used to determine the color shown for a activity in e.g. the calendar view.

* `Field` - you need to select ONE text field, which will contain the keywords relevant to set the colors - the drop-down list offers all Text, Short Text and Textbox field maintained under 'Fields'.
* `Use for Background` - if checked, the color is not applied to the text, but to the text background (this provides a behavior similar to GoldenCheetah 3.0x).
* `Keyword` - this is the main keyword to determine the color - (which is set in field 'Color') - when comparing the keywords with your texts, Upper/Lower case writing is ignored (so 'FTP' is treated equally to 'ftp' or 'fTp').
* `Color` - is set using a 'Color Chooser' dialog box which is opened by "mouse-click" on the color box.
* `Related Notes Words` - is useful, if you want more than one keyword to have the same color, instead of adding them one-by-one to the keyword list, you can just create one entry to define the color and enter all other keywords, separated by "," into this field.

### Defaults

new in 3.11 

### Processing

![Preferences - Datafields - Processing](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/PreferencesDataFields_Processing.jpg)

GoldenCheetah provides a number of fix/adjust/correct tools which are configured here. For further details, please read [Special Topics: Activity processing](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Special-Topics_Activity-Processing)

BACK: [Preferences: Overview](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Preferences_Overview)
