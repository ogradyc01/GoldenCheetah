The R chart is introduced with v4.0 of GoldenCheetah.

The chart can be added to the activity view and the trend view.

In trend view the chart is refreshed when a date range or season is selected, or if the compare pane is updated. Whilst in the activity view the chart is refreshed when an activity is selected or, again, if the compare pane for intervals is updated.

When the chart is refreshed the user supplied R script is executed, and it should collect data and prepare a plot.

A simple example to plot HR might be:
> ride <- GC.activity()
> plot(ride$heart.rate)

This basically calls a GC function to fetch the data for the current ride and then uses the base R plot function to plot heart rate as a time series.

Similarly, in trend view, to plot a simple time series of average power for the current season:
> metrics <- GC.metrics()
> plot(metrics$Average_Power)
