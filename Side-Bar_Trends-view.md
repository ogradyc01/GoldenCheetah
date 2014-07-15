Side Bar: Trends view (Version 3.1)
***

![SideBar General] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/SideBar_Trends.jpg)

The 'Side Bar' for the 'Trends' view offers five different panes - als illustrated above.

## Date Ranges

Date ranges define for which period in time data is shown in the main view of the 'Trends'. GoldenCheetah comes with a number of pre-defined 'Date Ranges' - which start with 'All Dates' and end with 'Last 12 months'. The predefined data ranges cannot be deleted or changed.

You can add you own data ranges - also called 'Seasons' in multiple ways.

* Pane Header Menu (all options)

![Add Season - Border Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Date_Range-Add_Season1.jpg)

* Context Menu - predefined seasons (only Add is possible)

![Add Season - Border Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Date_Range-Add_Season2.jpg)

* Context Menu - user defined seasons (all options)

![Add Season - Border Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Date_Range-Add_Season3.jpg)

In all cases, 'Add Season' opens a popup to define your new season:

![Add Season - Details] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Date_Range-Add_Season_Details.jpg)

* Name - your season name
* Type - currently 3 types are possible (Season, Cycle, Ad-hoc) - as of now they are for information purpose only, there is no functionality associated yet
* From - the 'from date' of the season/date range
* To - the 'to date' of the season/date range
* Starting LTS - Sets both the Long Term Stress (LTS) and Short Term Stress (STS) starting value for the PMC charts (independent of the PMC metrics used). 

_Note: Please observe, that the 'Starting LTS' value set in a season, is also considered when selecting a different 'Date Range' - so make sure that seasons, which shall not influence the overall PMC calculations, have the 'Starting LTS' set to '0' (which is is not considered in PMC calculation)_
* Lowest SB -  currently for information purposes only, no functionality associated 

_Note: Please observe that some charts can have their own data range defined for the chart. If this is the case, the 'Date Range' in the 'Side Bar' does not have any effect on the chart._

### Other Functions on 'Date Ranges'

* Edit Season - allows to change season settings (same fields to 'Add Season')
* Delete Season - deletes the selected season (please observe - no additional popup - season is immediately deleted)
* Add Event - create an Event for the selected season (see section 'Events' for more details)

## Events

Events are single dates which can be races,etc. Events are created and maintained for a user defined 'Date Range/Season', but are shown in the PMC charts independent of the selected 'Date Range'.

* Pane Header Menu - allows only to create events - the 'Season' for such an event is the actual selected season in the 'Date Range' pane. The popup does not appear, if the currently selected 'Date Range' is a system pre-defined range. (Events can only be created for user-defined seasons.)

![Add Event - Border Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Event_Add.jpg)

* Context Menu of an existing event - allows to Delete and Edit the selected event, but also to add a new event.

![Add Event - Border Menu] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Event_Menu.jpg)

In all cases, 'Add Event' opens a popup to define your new event:

![Add Event - Details] (https://raw.githubusercontent.com/Joern-R/GoldenCheetah/master/doc/wiki/Event_Details.jpg)

* Name - your event name
* Date - the date of the event


## Filters


## Charts


## Summary

This pane is a simple display pane, providing a summary view of the data selected. The data shown considers both filters and date ranges. The sections 'Totals', 'Averages' and 'Maximums' have fixed content. The section 'Metrics' is configurable and defined in the the GoldenCheetah preferences. See also `Menu Bar -> Tools -> Options...` [Metrics->Summary] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Preferences_Metrics)



