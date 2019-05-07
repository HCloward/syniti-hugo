+++
title = 'Track Error Records on Reports'
solution = 'Data Quality'
+++

# Track Error Records on Reports

Detailed metric information can be configured and generated for a
specific report. These metric reports specifically track how long an
error record exists in a report and provides details on when the error
was fixed.

To track error records on reports:

1.  Select **Configuration \> Report Repositories** in *Navigation*
    pane.

2.  Click **Reports** icon for Repository.

3.  Click **Vertical View** for Report.

4.  Click **Metric Data Information** tab.

5.  Click **Report Metric Data Build** check box to enable metric
    reporting.
    
    **NOTE:** If Report Metric data is being configured for the first
    time and report columns do not currently exist, an informational
    message displays.

6.  Click **Yes**.

7.  Click **Report Columns** icon to indicate which columns will be
    tracked for Metric Data Tracking.
    
    [View the field descriptions for the Metric Data Column (Config)
    page](../Page_Desc/Metric_Data_Column_Config.htm)

8.  Enter a sort order in **ORDER** field to determine how the columns
    are arranged in the report.

9.  Select a report column from **COLUMN** list box.

10. Enter a heading in **HEADING** field as the column that displays in
    the report.

11. Click **KEY COLUMN** check box to enable it, if the column is a key
    on the table.
    
    **NOTE:** Add the key columns and any additional columns on the
    report to track.

12. Click **Save**.

13. Click **Back** button for the browser to return to the *Repository
    Reports* page’s *Vertical* View.

14. Click **Metric Data Information** tab.

15. Click **Process** icon to immediately run the report; a confirmation
    message displays.
    
    **NOTE:** A *Service* page runs these reports on a schedule. The
    report runs when the Report Metric Data Completed On date is less
    than the Process Completed On date and the date differs by more than
    one day. To stop dspMonitor™ from processing the report on a
    schedule, disable the Report Metric Data Build check box on the
    Metric Data Information tab.

16. Click **Ok**.

17. Click **Results** to view how long key data has been on the report.

18. Select **Dashboard \> Reports (Metrics)** to view reports of all
    metric data results.
