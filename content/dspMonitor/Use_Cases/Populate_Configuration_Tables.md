+++
title = 'Populate Configuration Tables'
solution = 'Data Quality'
+++

# Populate Configuration Tables

The Configuration Tables define the meta-data for standard and
user-created reports.

This use case covers the following topics:

  - [Register Quality Dimensions](#Register_Quality_Dimensions)
  - [Register Data Quality Score
    Thresholds](#Register_Data_Quality_Score_Thresholds)
  - [Customize Group Metric
Graph](#Customize_Group_Metric_Graph)

## <span id="Register_Quality_Dimensions"></span>Register Quality Dimensions

A Quality Dimension is a recognized term used by data management
professionals to describe a feature of data that can be measured or
assessed against defined standards to determine data quality.

To register Quality Dimensions:

1.  Select **dspMonitor \> Configuration \> Administrative \> Quality
    Dimension** in *Navigation* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Quality Dimension
    page](../Page_Desc/Quality_Dimension.htm)

3.  Enter a dimension in **QUALITY DIMENSION** field.

4.  Enter a priority in the **PRIORITY** field.

5.  Enter a description in the **DESCRIPTION** field.

6.  Click the **Active** check box to make the Quality Dimension active.

7.  Click
**Save**.

## <span id="Register_Data_Quality_Score_Thresholds"></span>Register Data Quality Score Thresholds

Thresholds define the status assigned to an object being scored when the
percentage of defects falls below the threshold. Statuses are Red
(critical), Yellow (warning) and Green and are displayed on summary
pages, charts and dashboards in dspMonitor™.

dspMonitor™ is delivered with a default threshold setting based on the
sigma levels displayed on the *[Sigma
Levels](../Page_Desc/Sigma_Levels.htm)* page. Additional threshold
settings can be added to meet the project needs.

To register data quality score thresholds:

1.  Select **Configuration \> Data Quality Score Thresholds** in
    *Navigation* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Data Quality Score Thresholds
    page](DQS_Thresholds.htm)

3.  Enter a name in the **NAME** field.

4.  Enter or select a percentage for the critical threshold in the
    **CRITICAL THRESHOLD** field.

5.  Enter or select a percentage for the critical threshold in the
    **WARNING THRESHOLD** field.
    
    **NOTE:** If Enable Sigma Level is checked on the
    *[Parameters](../Page_Desc/Parameters.htm)* page, sigma levels are
    available for selection in the critical and warning threshold list
    boxes. Sigma levels can be viewed on the *[Sigma
    Levels](../Page_Desc/Sigma_Levels.htm)* page.

6.  Click
**Save**.

## <span id="Customize_Group_Metric_Graph"></span>Customize Group Metric Graph

dspMonitor™ is delivered with a sample group metric Excel spreadsheet
that can be customized by groups, connection strings and data length to
meet the project needs.

To customize the Initial Connection and Groups for the Group Metric
Graph:

1.  Select **Configuration \> Parameters** in *Navigation* pane.

2.  Click <span style="font-weight: bold;">Metric Parameters</span> tab.

3.  Verify the following parameters are configured:
    
      - Graph Directory Path
    
      - Metric Report Day
    
      - Metric Report Week
    
      - Metric Report Month
    
    **NOTE:** The views are created for the groups once a complete
    metric cycle has finished. Configure the metric parameters to set
    the number of days, weeks and months, respectively, which are stored
    in the metrics.

4.  Select **Configuration \>** **Group Metric Graph** in *Navigation*
    pane.

5.  Click **Download**.

6.  Save the file.

7.  Open the Excel file.

8.  Click **MonthlyData** worksheet.

9.  Right-click the A-1 cell.

10. Select **Edit Query**.

11. Update the Connection information to match that of the client site.

12. Repeat steps 7– 9 for the WeeklyData and DailyData worksheets within
    the Excel workbook.

13. Update the graph to match the local groups, if applicable.

14. Click **Upload** on the *[*Group Metric
    Graph*](../Page_Desc/Group_Metric_Graph.htm)* page to upload the
    modified Excel file.
