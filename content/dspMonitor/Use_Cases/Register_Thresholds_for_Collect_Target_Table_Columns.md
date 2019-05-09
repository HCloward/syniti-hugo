+++
title = 'Register Thresholds for Collect Target Table Columns'
solution = 'Data Quality'
+++

# Register Thresholds for Collect Target Table Columns

A Data Quality Steward can register data quality score thresholds for
Collect target table columns. This allows the Data Quality Steward to
register the columns to a report in the report repository.

**NOTE:** The threshold levels set at the target table column level are
applied globally across all report repositories for all reports that use
the table column.

To register data quality score thresholds for a Collect target:

1.  Select **dspMonitor \> Configuration \> Report Repositories** in the
    *Navigation* pane.

2.  Click the **Collect Targets** icon.

3.  Click the **Configure Thresholds** icon.

4.  Click **Configure Columns** for a table.

5.  Click **Add**.
    
    [View the field descriptions for the Target Table Column Threshold
    page](../Page_Desc/Target_Table_Column_Threshold)

6.  Select the column name from the **COLUMN NAME** list box.

7.  Select the threshold ID from the **THRESHOLD ID** list box.
    
    **NOTE:** If a new threshold is set on the *[Report Target Table
    Columns](../Page_Desc/Report_Target_Table_Columns)* page, this
    value is automatically updated. The table and column are added if
    they did not already exist. Refer to [Register Collect Target Table
    Columns to a
    Report.](Register_Collect_Target_Table_Columns_to_a_Report)
    
    **NOTE:** If no threshold is selected here or on the *[Report Target
    Table Columns](../Page_Desc/Report_Target_Table_Columns)* page,
    the threshold set on the *[Parameters](../Page_Desc/Parameters)*
    page is used. Refer to [Register Data Quality Score
    Thresholds](Populate_Configuration_Tables#Register_Data_Quality_Score_Thresholds)
    for more information about thresholds.

8.  Click **Save**.
