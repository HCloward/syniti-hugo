+++
title = 'Create Dashboards and Charts'
solution = 'Platform'
+++

# Create Dashboards and Charts

BackOffice Associates® Solutions supports the ability to create charts
and dashboards to display data. Individual charts of data are created by
using the Chart page type. Dashboards are created using the Dashboard
page type to create a collection of charts. For example, a dashboard can
be configured to display tables as a bar chart and the package types
used for downloads as a pie chart. A Combination Chart can be created to
combine multiple chart types (pie, column, line, and dotted line) on a
single chart page. 3D charts can be created for column and pie charts.

**NOTE:** The many chart options available for 3D, combination, and
regular charts can result in charts that are difficult for a user to
interpret. As a best practice when creating chart pages, make sure to
review how the data displays with the various options. To make a chart
clear and represent the data accurately, adjustments may be required
such as splitting a combination chart apart or using a dashboard.

Charts can display numeric data against categorical data, dividing the
data into two separate categories. The categories are value columns and
category columns. Column properties and category column properties can
be added to customize the charts. Pages can be linked to charts, charts
to pages and charts can be linked to charts. 

There are several steps required to create a chart page:

  - Create a view in SQL.
  - Register the view as a Chart page Type in DSP®.
  - Customize the chart page by applying column properties.

All charts in DSP® are based on a view in the associated database. Views
and charting typically follow the pattern of using a category of data
and a numeric value. A chart view contains the data to be displayed via
the chart page and can reference multiple views and tables.

At least one column in the view must contain a Value field (for X-axis
data) and a Category (for Y-axis data) field. There can be more than one
Value column and one to two Category columns. If there are two Category
columns, there can only be one Value column. 

An extra column can be included in the view, which must be manually
added to the *Page Columns* page where the Control = Category. The
Platform only supports two column properties where Control = Category.
Mark each category control as Primary and Secondary via the **Grouping
Category** field on the *Vertical* View.

3D charts can be created for column and pie charts.

Use the naming convention **webXXXChart**, where **XXX** is a logical
name for the chart page.

**NOTE**: BackOffice Associates® Solutions is delivered with a series of
charts and dashboards. Custom charts are maintained during upgrades to a
new version of BackOffice Associates® Solutions. Modifications made to
delivered charts are not supported; any changes made to delivered charts
will be lost on upgrade.

This section contains the following topics:

  - [Create a Chart](Create_a_Chart)
  - [Create a Dashboard](Create_a_Dashboard)
  - [Add Layouts](Add%20Layouts)
  - [Copy a Layout](Copy%20a%20Layout)
