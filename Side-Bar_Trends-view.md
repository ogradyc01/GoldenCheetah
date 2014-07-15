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

* Name - how you want to call the season
* Type - currently 3 types are possible (Season, Cycle, Ad-hoc) - as of now they are for information purpose only, there is no functionality associated yet
* From - the 'from date' of the season/date range
* To - the 'to date' of the season/date range
* Starting LTS - Sets both the Long Term Stress (LTS) and Short Term Stress (STS) starting value for the PMC charts (independent of the PMC metrics used). _Note: Please observe, that the value set in a season, is also considered when selecting a different 'Date Range' - so make sure that seasons, which should not have an influence on the PMC calculations, have a 'Starting LTS' set to '0' (which means the value is not considered)_
* Lowest SB -  currently for information purposes only, no functionality associated 

_Note: Please observe that some charts can have their own data range defined for the chart. If this is the case, the 'Date Range' in the 'Side Bar' does not have any effect on the chart._


## Events


## Filters


## Charts


## Summary

This pane is a simple display pane, providing a summary view of the data selected. The data shown considers both filters and date ranges. The sections 'Totals', 'Averages' and 'Maximums' have fixed content. The section 'Metrics' is configurable and defined in the the GoldenCheetah preferences. See also `Menu Bar -> Tools -> Options...` [Metrics->Summary] (https://github.com/GoldenCheetah/GoldenCheetah/wiki/Preferences_Metrics)



