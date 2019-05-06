# Target Table Status

This chart displays the number of active tables by refresh status for
each target.

Targets are destination databases (registered as data sources in the
platform) where tables are refreshed with source data using Collect.
Source data can also be refreshed into a source database (.sdb), so an
sdb displays as a target in the x axis on this chart as
well.<span> </span>

Status includes:

  - Error tables: Tables that failed to refresh.
  - Success Tables: Tables that have been refreshed and downloaded to
    the target successfully.
  - Not downloaded tables: Tables that have not yet been refreshed.
  - Refreshing tables: Tables that are currently refreshing.

Click a bar to drill down to the *Targets* page to view details about
the selected target and Target Source and to access the *Tables* page
for the Target Source to refresh tables.

Refer to [View Dashboard in
Collect](../Use_Cases/View_Dashboard_in_Collect.htm) for general
information about how data displays on dashboards.

To access the chart in Collect, click
<span style="font-weight: bold;">Summary Dashboard</span> in the
<span style="font-style: italic;">Navigation</span> pane.
