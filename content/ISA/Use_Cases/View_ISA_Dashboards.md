# View ISA Dashboards

The charts on the ISA dashboard provide summary data about the number of
records that fail IS rules. These rules are assigned to Project
Distributions, which are groups of users. The charts display data by
project distributions or by users.

The Total Records Chart drills down through failed record counts for
rules per Project Distributions.

The Records by User Chart drills down through failed record counts for
rules per users.

Each bar chart has a corresponding line chart to track trends (i.e., how
the number of records that have failed changes over time). For example,
the Records by Project Chart displays a count for each project for the
current day, while its corresponding Record Trend by Project chart
displays how the number of failed records changed for each project over
a period.

ISA charts also display:

  - Total Opportunities vs Failures Summary
  - Failure Percentage Summary
  - Dimensions Summary
  - Users can drill down through the charts on these dashboards to view
    data at the project, project distribution, or rule level.
  - Bar charts allow a user to drill down, trend charts display data
    only.

**NOTE**: ISA charts only include historical data. Real-time data is not
included on these charts.

Charts display:

  - Metrics for up to 10 days, depending on the Days to Retain Metrics
    field
  - The 10 rules that have the highest number of failed records

**NOTE**: Data on charts displays based on the Days to Retain Metrics
setting, which can be set at the Parameter level (Configuration \>
Parameters \> Basic Settings). Metrics can be retained for up to 10
days. Additionally, each project has its own Days to Retain Metrics
setting (set on the *Vertical View* of the *[Project
Summary](../Page_Desc/Project_Summary_H.htm)* page), which, if set, will
override the setting in Parameters.

When the user drills down through the charts to the Report Data Viewer,
the count of records on the Report Data Viewer may be lower than the
counts on the charts. User filters are applied to reports, but not to
the metrics in charts. To restrict access based on a user’s security
settings, a user only views reports to which that user has access
through project distribution assignments.

The View Data icon to the right of a chart name opens a pane that
displays the alternate text descriptions of chart data in a table. If a
chart has a legend, click a label in the legend to hide or show that
label’s section in the chart.

Hover a cursor over each section of a bar to view the field count.

If a chart is 3D, a 3D Controls icon is available to adjust the chart
angles.

ISA dashboards include the following charts:

  - [Total Records Charts](Total_Records_Charts.htm)
  - [Records by User Charts](Records_by_User_Charts.htm)
  - [Records by Project Chart](Records_by_Project_Chart.htm)
  - [Records by Distribution Chart](Records_by_Distribution_chart.htm)
  - [Records by Rule Chart](Records_by_Rule_chart.htm)
  - [Record Trend by Project Distribution
    Chart](Record_Trend_by_Project_Distribution_Chart.htm)
  - [Record Trend by Project Chart](Record_Trend_by_Project_Chart.htm)
  - [Record Trend by Project Distribution Rule
    Chart](Record_Trend_Prjt_Distrib_Rule_Chart.htm)
  - [Records by Distribution User
    Chart](Records_by_Distribution_User_Chart.htm)
  - [Record Trend by Project Distribution User
    Chart](Record_Trend_Prjt_Distrib_User.htm)
  - [Records by Distribution User Rules
    Chart](Records_Distribution_User_Rules.htm)
  - [Record Trend by Project Distribution User Rule
    Chart](Record_Trend_Prjt_Distrib_User_Rule.htm)
  - [Total Opportunities vs. Failures
    Summary](Total_Opportunities_vs._Failures_Summary.htm)
  - [Total Opportunities vs Failures By
    Project](Total_Opportunities_vs_Failures_By_Project.htm)
  - [Total Opportunities vs. Failures by
    Distribution](Total_Opportunities_vs._Failures_by_Distribution.htm)
  - [Total Opportunities vs. Failures by
    Rule](Total_Opportunities_vs._Failures_by_Rule.htm)
  - [Failure Percentage Summary](Failure_Percentage_Summary.htm)
  - [Failure Percentage by Project](Failure_Percentage_by_Project.htm)
  - [Failure Percentage by
    Distribution](Failure_Percentage_by_Distribution.htm)
  - [Failure Percentage by Rule](Failure_Percentage_by_Rule.htm)
  - [Dimension Summary](Dimension_Summary.htm)
  - [Selected Dimension by Project](Selected_Dimension_by_Project.htm)
  - [Selected Dimension by
    Distribution](Selected_Dimension_by_Distribution.htm)
  - [Selected Dimension by Rule](Selected_Dimension_by_Rule.htm)
