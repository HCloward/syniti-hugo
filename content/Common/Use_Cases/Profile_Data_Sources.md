# Profile Data Sources

Data can be profiled for an [entire Data
Source](#Profile_Entire_Data_Source) or for a [single
table](#Profile_Individual_Tables) within the Data Source.

There are many types of data that is collected when a Data Source is
profiled:

  - Record counts for each table
  - Unique values for each field
  - Unique value count for each field
  - Blanks for each field
  - Fields used and not used
  - Minimum/maximum values for each field
  - Maximum field length
  - Field datatype
  - Field data type
length

## <span id="Profile_Entire_Data_Source"></span>Profile Entire Data Source

To profile a Data Source:

1.  Click **Analyze** in the *Navigation* pane.

2.  Click **Profile** for Data Source ID.

3.  Click **Execute** to profile the entire data source; a confirmation
    message displays.
    
    OR
    
    Click <span style="font-weight: bold;">Profile TT Tables Only</span>
    icon to profile just the tables within the data source; a
    confirmation message displays.
    
    **NOTE:** The Profile TT Tables Only icon is enabled if tt tables
    exist in the data source; it is disabled if no tt tables exist in
    the data source.

4.  Click **Ok**.

**NOTE:** Profiling a Data Source may take several hours, depending on
the size of the data source. When the data source has been queued for
profiling, a confirmation message displays.

If an error occurs or if the profiling process needs to be restarted,
click **Reset** for the data source.

## <span id="Profile_Individual_Tables"></span>Profile Individual Tables

Profile an individual table if metrics for that single table (versus the
entire data source) are needed.

To profile a single table:

1.  Click **Analyze** in *Navigation* pane.

2.  Click **Profile** for Data Source ID.

3.  Click **Tables**.

4.  Verify the <span style="font-weight: bold;">ACTIVE</span> check box
    is enabled for the table.

5.  Click **Execute** for a table; a confirmation message displays.
    
    **NOTE:** Two conditions must be met before the Execute icon is
    enabled: 1) the table must be active in order for the Execute icon
    to be available for the table and 2) the data source must be
    profiled (i.e., click the Execute icon on the *[Data Sources
    Tables](../Page_Desc/Data_Sources_Tables.htm)* page).
    
    **NOTE:** Depending on the size of the table, profiling a table may
    take several minutes to complete.

6.  Click **Ok**.

If an error occurs or if the profiling process needs to be restarted,
click **Reset** for the table.
