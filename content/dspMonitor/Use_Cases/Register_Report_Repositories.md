+++
title = 'Register Report Repositories'
solution = 'Data Quality'
+++

# Register Report Repositories

Reports are organized by report repository. Once created in the database
and registered in Common, report repositories must then be registered in
dspMonitor.

To register a report repository (referred to as a data source in
Common), refer to [Register a Data Source in
Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm).

To register a report repository in dspMonitor:

1.  Select **Configuration \> Report Repositories** in *Navigation*
    pane.

2.  Click **Add**.
    
    [View the field descriptions for the Report Repositories
    page](../Page_Desc/Report_Repositories_H.htm)

3.  Select a report repository from the **REPOSITORY** list box.
    
    **NOTE:** The **REPOSITORY** list box displays all report
    repositories (referred to as a data source in Common) registered to
    the DSP® instance.

4.  Click **Save**.

5.  Click **Vertical View** to enter a cache database, change the report
    filter, or the opportunity view filter, if applicable.

6.  Click **Edit**.
    
    [View the field descriptions for the Report Repositories page's
    Vertical View](../Page_Desc/Report_Repositories_H.htm)

7.  Update **Report Filter** if default value is not applicable.
    
    **NOTE:** The default Report Filter value is maintained under
    Configuration \> Parameters.

8.  Enter an **Opportunity View Filter**.
    
    **NOTE:** The recommended value is tv\*OptSel. If this value is
    entered, when configuring reports on the *Repository Reports* page,
    only views that follow the naming convention of tv\*OptSel are
    available to choose as an Opportunity View from the list box. If not
    value is entered, the Default Opportunity View Filter from the
    *Parameters* page is used.

9.  Enter a database in **Cache Database Name** if a separate database
    is used for all cache tables.
    
    **NOTE:** The Cache Database Name allows a cache database to exist
    for a repository instead of defining multiple cache databases.
    Reducing the number of cache databases on the SQL Server instance
    increases performance and alleviates clutter. If a cache database is
    used, it must be configured *before* reports are registered to the
    repository.

10. Select a threshold ID from the **Threshold ID** list box.
    
    **NOTE:** If no threshold is selected, the threshold ID set on the
    *Parameters* page is used in the data quality score status
    calculation. Refer to [Register Data Quality Score
    Thresholds](Populate_Configuration_Tables.htm#Register_Data_Quality_Score_Thresholds)
    for more information.

11. Click **Save**.
