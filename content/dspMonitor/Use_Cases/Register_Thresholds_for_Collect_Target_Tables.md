+++
title = 'Register Thresholds for Collect Target Tables'
solution = 'Data Quality'
+++

# Register Thresholds for Collect Target Tables

A Data Quality Steward can register data quality score thresholds for
Collect target tables. This allows the Data Quality Steward to register
the tables to a report in the report repository.

**NOTE:** The threshold levels set at the target table level are applied
globally across all report repositories for all reports that use the
table.

To register data quality score thresholds for a Collect target:

1.  Select **dspMonitor \> Configuration \> Report Repositories** in the
    *Navigation* pane.

2.  Click the **Collect Targets** icon.

3.  Click the **Configure Thresholds** icon.

4.  Click **Add**.
    
    [View the field descriptions for the Target Table Threshold
    page](../Page_Desc/Target_Table_Threshold.htm)

5.  Select the table name from the **TABLE NAME** list box.

6.  Select the threshold ID from the **THRESHOLD ID** list box.
    
    **NOTE:** If a new threshold is set on the *[Report Target
    Tables](../Page_Desc/Report_Target_Tables%20H.htm)* page this value
    is automatically updated. The table is automatically added here if
    it did not already exist. Refer to [Register Collect Target Tables
    to a Report](Register_Collect_Target_Tables_to_a_Report.htm).
    
    **NOTE:** If no threshold is selected here or on the *[Report Target
    Tables](../Page_Desc/Report_Target_Tables%20H.htm)* page, the
    threshold set on the *[Parameters](../Page_Desc/Parameters.htm)*
    page is used. Refer to [Register Data Quality Score
    Thresholds](Populate_Configuration_Tables.htm#Register_Data_Quality_Score_Thresholds)
    for more information about thresholds.

7.  Click **Save**.
