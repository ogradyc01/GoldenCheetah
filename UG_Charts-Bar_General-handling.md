Charts Bar: General handling (Version 3.2)
***

![Charts Bar](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/ChartsBar_Activities.jpg)

The 'Charts Bar' is a quick access to the different data charts / metrics charts / CP charts / maps / etc. of GoldenCheetah. With the initial installation of GoldenCheetah the 'Charts Bar' is pre-configured with a number of different charts.

_Note: For each different view of GoldenCheetah (Trends/Diary/Activities/Train) the 'Charts Bar' is different and also any change in configuration of the 'Charts Bar' only takes effect for the respective view._

_Note2: GoldenCheetah comes with a set of pre-defined Charts for the different views. At the first time you add/change/delete a chart the default charts are copied and are now your personal / athlete specific set of charts. Any further change is done on your personal version. If you want to go back to the default settings - you can do this via `Reset Layout` for each view (Trends/Diary/Activities/Train) separately._

### Add Chart

Adding a new chart to the 'Charts Bar' of a view can be done in 2 ways:

* `Mouse-click the icon` on the right hand side of each 'Charts Bar' - which then opens open an 'Add Chart' selection which contains the possible chart types for the the currently active 'Scope Bar' view (Trends/Diary/Activities/Train).

* `Menu Bar->View->Add Chart` brings up exactly the same list like the variant before.

The different 'Chart Types', their availability for the different 'Scope Bar' views, and their configuration settings are explained here: 
[Chart Types](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_General)

### Configure Chart / Close Chart

Configuration and closing (= removing from 'Chart Bar') of a chart is done using the `More...` function reached through mouse-over in the left/top corner of the 'Main View'.

![ChartBar More 1](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/ChartsBar_Activities_More.GIF)

Depending on the type of chart, one or many options available on 'More...". In our example you have:

* `Close` - this is available for ANY chart: 'Close' removes the chart from the 'Charts Bar' after asking if you really want to do this. You can remove any of the charts - whether they are origi
* `Export Chart Image...` - for charts which have graphics/plots: 'Export Chart Image...' opens a dialog to export the graphic/plot as a graphics file (in .png) format. The export basically creates an internal screenshot of the VISIBLE area of the 'Main View'. If your chart is bigger than the visible area, only the visible part will be exported.
* `All Chart Settings` - for charts having specific settings, 'All Chart Settings' opens the chart type specific 'Chart Settings' dialog box. These dialog boxes have the same parameter like those when adding a chart. (See [Chart Types](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_ChartTypes_General)  )

![Chart Bar More 2](https://raw.githubusercontent.com/GoldenCheetah/GoldenCheetah/master/doc/wiki/ChartsBar_Activities_More.jpg)

_Note: For some of the chart types, an accelerated access of their most common configuration settings is also revealed by a 'mouse-over' to 'More...' as part of a semi-transparent overlap to the upper border of the 'Main View'. You can change the available settings, without to go to 'All Chart Settings'. The overlay is available as long as the mouse cursor stays in the semi-transparent area._

### Reset Layout

Last function associated to charts is the `Reset Layout` option. This function is accessed through the 'Menu Bar' only. So please check [Menu Bar: View](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Menu-Bar_View)

### Change Chart Order 

Changing the order of the charts in the 'Charts Bar' is possible. The re-sorting has to take place in the "Tiled" view of the charts. This view can be switched on (as one option) through the [Tool Bar](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_Tool%20Bar_Functions)

When being in the 'Tiled' view it's possible to "drag&drop" the charts into a new order. The section to "drag" is the header line / chart name. The section to "drop" is the separator section between the two chart where you want to 'dragged' chart to be moved to.

Changes in the 'Tiled' view are also considered in the 'Charts Bar' view.

BACK: [General UI](https://github.com/GoldenCheetah/GoldenCheetah/wiki/UG_General_UI-Layout-and-terminology)
