Side Bar: Trends view (Version 3.1)
***

![SideBar General] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/SideBar_Trends.jpg)

The 'Side Bar' for the 'Trends' view offers five different panes - as illustrated above.

* [Date Ranges] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Trends-view#date-ranges)
* [Events] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Trends-view#events)
* [Filters] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Trends-view#filters)
* [Charts] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Trends-view#charts)
* [Summary] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_Trends-view#summary)

***

## Date Ranges

Date ranges define for which period in time data is shown/accumulated in the main view of 'Trends'. GoldenCheetah comes with a number of pre-defined 'Date Ranges' - which start with 'All Dates' and end with 'Last 12 months'. The predefined date ranges cannot be deleted or changed.

You can add you own data ranges - also called 'Seasons' in multiple ways.

* Pane Header Menu (all options)

![Add Season - Border Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Date_Range-Add_Season1.jpg)

* Context Menu - predefined seasons (only Add is possible)

![Add Season - Border Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Date_Range-Add_Season2.jpg)

* Context Menu - user defined seasons (all options)

![Add Season - Border Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Date_Range-Add_Season3.jpg)

In all cases, `Add Season` opens a popup to define your new season:

![Add Season - Details] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Date_Range-Add_Season_Details.jpg)

* `Name` - your season name
* `Type` - currently 3 types are possible (Season, Cycle, Ad-hoc) - as of now they are for information purpose only, there is no functionality associated
* `From` - the 'from date' of the season/date range
* `To` - the 'to date' of the season/date range
* `Starting LTS` - sets both the Long Term Stress (LTS) and Short Term Stress (STS) starting value for the PMC charts (independent of the PMC metrics used). 

_Note: Please observe, that the 'Starting LTS' value set in a season, is also considered when selecting a different 'Date Range' - so make sure that seasons, which shall not influence the overall PMC calculations, have the 'Starting LTS' set to '0' (so they are not considered in PMC calculation)_
* `Lowest SB` -  currently for information purposes only, no functionality associated 

_Note: Please observe that some charts can have their own date range defined in the chart specific settings. In such cases the 'Date Range' in the 'Side Bar' does not have any effect on the chart data._

### Other Functions on 'Date Ranges'

* `Edit Season` - allows to change season settings (same fields to 'Add Season')
* `Delete Season` - deletes the selected season (please observe - no additional dialog box - the season is immediately deleted)
* `Add Event` - creates an 'Event' for the selected season (see section 'Events' for more details)

## Events

Events are single dates which can be races,etc. Events are created and maintained for a user defined 'Date Range/Season', but are shown in the PMC charts independent of the selected 'Date Range'.

* `Pane Header Menu` - allows only to create events - the 'Season' for such an event is the actual selected season in the 'Date Range' pane. The popup does not appear/function is not possible, if the currently selected 'Date Range' is a system pre-defined range. (Events can only be created for user-defined seasons.)

![Add Event - Border Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Event-Add.jpg)

* `Context Menu of an existing event` - allows to Delete and Edit the selected event, but also to add a new event.

![Add Event - Border Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Event-Menu.jpg)

In all cases, `Add Event` opens a popup to define your new event:

![Add Event - Details] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Event_Details.jpg)

* `Name` - your event name
* `Date` - the date of the event


## Filters

Filtering via the 'Side Bar' is one of multiple ways, how you can select the rides, which are then analysed in the 'Trends View'. The special feature of filtering in the 'Side Bar', compared to other filtering options is, the 'Auto Filter' provided here:

![Filters - Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Filters_Settings.jpg)

* Section 'Filters' - shows the list of your predefined filter queries - you can select one or multiple filters (using Windows, the multi-select is done via "Shift" or "CRTL" and "mouse-click. Other OS might work differently, but offer the same feature). Multiple filters here are applied with an logical "AND", so that only the data of rides which fulfill ALL filter rules is considered in a chart.

* Sections 'Workout Code', 'Sport',... are the 'Autofilter's. The values shown for each 'Autofilter' is the list of values used in that particular 'Autofilter' field of your rides. You can select one or many of these values which then limit the rides to those where one of the selected values is assigned (logical "OR").

_Note: All fields which are of type "ShortText" or "Text" in the 'Preferences->Data Fields->Field' list and are assigned to a "Screen Tab", are available as 'Autofilters'._

### Filters - Menu

* `Autofilter` - the list shows all possible 'Autofilter' fields - which you can either activate or de-activate to be shown/used in the 'Side Bar'

* `Manage Filters` - open a dialog box which allows to create your own filter queries (the filter queries created here are available for all GoldenCheetah Filter functions)

![Filters - Manage] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Filters_Manage.jpg)

Further information on filtering can be found under: [Filtering/Searching] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Special-Topics_SearchFilter)


## Charts

The 'Charts' section is new with 3.1. It provides a different way to access the charts which are shown in the 'Main View' without having the need to add every single chart to the 'Charts Bar'.

![SideBar - Charts] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/SideBar-Charts.jpg)

The 'Side Bar - Charts' only take effect if you use a special chart (Default - "Library") on the main view. If you display any other chart on the 'Main View', selection of a chart in the 'Side Bar - Charts' has no effect.

Here the configuration of the 'Library' Chart:

![SideBar - Library] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Sidebar-Chart-Library.jpg)


## Summary

This pane is a simple display pane, providing a summary view of the rides selected. The data shown honors both filters and date ranges. The sections 'Totals', 'Averages' and 'Maximums' have fixed content. The section 'Metrics' is configurable and defined in the GoldenCheetah preferences. See also `Menu Bar -> Tools -> Options...` [Metrics->Summary] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Preferences_Metrics)

BACK: [Side Bar: General] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Side-Bar_General-handling)