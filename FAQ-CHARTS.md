## CHARTS



### I want to plot month -1,-2 and -3 how do I do that?

Assuming the chart allows you to specify a date range you can select 'This' 'month'
and select prior '3' to specify a month 3 years prior, similarly 'This' 'month' and
prior '2' is a month 2 months ago, whilst 'This' 'month' and prior '1' is last month.

'This' 'month' prior and 0 is just this month.



### How should I use Aerolab?

The following is a brief piece of advice from Robert Chung, from a discussion on the
Golden Cheetah Users mailing list:

Ideally, you'll want calm conditions (both in terms of wind and traffic) but here's a
quickie test you can do just to get a handle on what to do. Try to find a loop without
stop signs, or an out-and-back with maybe a little dip or something in the middle. Make
sure you won't get hit by a car and have good sight lines. I just go around my block a
few times. Do a loop in the drops, then another loop faster, then a loop slower; then
repeat with your hands on the hoods.

Weigh yourself and the bike and ballpark the air density.

See whether you can come close to modeling the "true" elevation profile by sliding the
CdA slider around. Even with this informal test, as long as the wind isn't blowing too
hard, you ought to be able to see a difference between the loops where you were in the
drops and the loops where you on the hoods, and to spot little bumps and dips in the road.

There is also an overview of Virtual Elevation to measure aerodynamics in this
YouTube video from the power seminar at Interbike 2011 given by Jim Meyer the founder
of Quarq:

<http://www.youtube.com/watch?v=b8tJnFE_BFg&feature=youtu.be&t=27m58s>

Finally, Robert Chung's original paper is included in the docs section of the GoldenCheetah
repository, you can it up here (click on 'View Raw' to download):

<https://github.com/GoldenCheetah/GoldenCheetah/blob/master/doc/contrib/ChungVE.pdf>



### My map doesn't show?

This is most likely because you have a proxy that requires authentication or session
details. We do not have sophisticated support for internet proxy servers. We will
re-use the operating system settings where they are configured.



### What is the treemap plot used for?

Typically it is used to visualise where you spend your time or where you get best
results.  It is not particularly useful if you do not maintain details for each ride
e.g. workout code, sport et al.



### Can I change the colors in plot x ?

With the exception of the Long Term Metric plots the colours on the charts are
configured in the GoldenCheetah preferences pane. It is possible to apply a theme
or change each individual color.

We want to use the same colours to plot each data series across the charts, so you
can change them globally.

The only colours you cannot change are the colours assigned to intervals when plotting
them on scatterplot or PfPv. These colours are assigned according to their sequence.



### How do you zoom in on a chart?

You can zoom in on the distribution, scatterplot and PfPv charts by selecting the zoom
area with the left click of the mouse.

On the performance (ride) plot you can zoom with the span slider at the bottom of the
chart (if you select the full plot in the chart settings).

There are no other zoom options for the other charts.



### I zoomed in but can't zoom out?

Right click will zoom back out to the previous zoom level (in the case of zooming
multiple times).  If you select another activity the chart will return to fully
zoomed out.



### GoldenCheetah is saying there is no data for a chart, but I'm sure there is?

You should check in the editor if the data series is present. if the activity is a
manual activity entry it will contain no data.
