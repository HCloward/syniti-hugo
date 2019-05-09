+++
title = 'Refresh'
solution = 'Platform'
+++

# Refresh

Refresh processes can run on a schedule or can be manually initiated
(targets can only be manually refreshed). Only active sources and tables
are downloaded.

<span style="font-weight: normal;">Sources are the original databases
that the table data is read from. They can be manually refreshed or set
to refresh on a schedule. </span>

This section contains the following topics:

  - [Refresh Targets](#Refresh_Targets)
  - [Manually Refresh Sources](#Manually_Refresh_Source)
  - [Schedule Source Refresh](#Schedule_Source_Refresh)
  - [Refresh Tables](#Refresh_Tables)
  - [Manually Refresh Tables](#Manually_Refresh_Table)
  - [Schedule Table Refresh](#Schedule_Table_Refresh)

The **Refresh** icon is disabled for **DBMoto®** package types because
the refresh process is run by DBMoto® instead of Collect. The
**DBMoto®** option is only available if DBMoto® for Collect is
installed.

## <span id="Refresh_Targets"></span>Refresh Targets

Targets are destination SQL Server databases where the source data is
refreshed. The target must be manually refreshed or have all the sources
scheduled to refresh the data.

To manually refresh a target:

1.  Click **Targets** in
    *<span style="font-size: 11.0pt;">Navigation</span>* pane.
2.  Select the Target.
3.  Click **Refresh** on Page toolbar; a confirmation message displays.
4.  Click **Ok**.

## <span id="Manually_Refresh_Source"></span>Manually Refresh Source

To manually refresh a source:

1.  Verify the source and the applicable tables are active.

2.  Click **Targets** in
    *<span style="font-size: 11.0pt;">Navigation</span>* pane.

3.  Click **Sources** for Target.

4.  Select the Source.

5.  Click **Build And Refresh** on Page toolbar.
    
    **NOTE**: If the source is IG Universal Connect, the table data is
    refreshed, but no packages are built.

6.  Click **Ok**.

**NOTE:**If packages for the tables already exist, they are only
refreshed (i.e., data is pulled from the Source database). If packages
for the tables do not exist, the packages are built and the tables are
refreshed.

**NOTE**: When a Target Source of IG Universal Connect is refreshed, a
Boomi Process is executed.

## <span id="Schedule_Source_Refresh"></span>Schedule Source Refresh

To refresh a source on a schedule:

1.  Verify the source and the applicable tables are active.

2.  Click **Targets** in
    *<span style="font-size: 11.0pt;">Navigation</span>* pane.

3.  Click **Sources** for Target.

4.  Click **Vertical View** for Source.

5.  Click **Advanced Settings** tab.

6.  Click **Edit**.
    
    [View the field descriptions for the Target Sources page's Vertical
    View](../Page_Desc/Target_Sources_H_Collect)

7.  Update **Schedule ID** list box if default value is not applicable.
    
    **NOTE:** The <span style="font-weight: bold;">Schedule ID</span>
    field determines when the refresh process is run. Schedules are
    created and maintained in Common. Refer to [Create
    Schedules](../../Common/Use_Cases/Create_Schedules) for detailed
    information.

8.  Click **Save**. 

## <span id="Refresh_Tables"></span>Refresh Tables

If a table has schedule set to a value other than NULL, that schedule is
used in calculating the next run date time. Tables can be manually
refreshed or set to refresh on a schedule.

**NOTE**: To receive a workflow email that a table download has failed
in Collect, a user must be assigned to a security role that has the
Collect WebApp group WorkFlowFailureAll or WorkFlowFaiureByTargetAccess
assigned. Refer to [Set
Security](../../Sys_Admin/Use_Cases/Setting_security) in System
Administration for more information.

## <span id="Manually_Refresh_Table"></span>Manually Refresh Table

To manually refresh a table:

1.  Verify the table is active.
2.  Click **Tables** in *Navigation* pane to view a list of all tables
    for all sources.
3.  Select the Table.
4.  Click **Build And Refresh** on Page Toolbar to build package and
    download table from source; a confirmation message displays.
5.  Click **Ok**.

**NOTE:** If the package for the table already exists, it is only
refreshed (i.e., data is pulled from the Source database). If the
package for the table does not exist, the package is built and the table
is refreshed. 

## <span id="Schedule_Table_Refresh"></span>Schedule Table Refresh

To refresh a table on a schedule:

1.  Verify the table is active.

2.  Click **Tables** in *Navigation* pane to view a list of all tables
    for all sources.

3.  Click **Vertical View** for the Table.

4.  Click **Advanced Settings** tab.

5.  Click **Edit**.
    
    [View the field descriptions for the Tables page's Vertical
    View](../Page_Desc/Tables_H)

<!-- end list -->

1.  Update **Schedule ID** list box if default value is not applicable.
    
    **NOTE:** The <span style="font-weight: bold;">Schedule ID</span>
    field determines when the tables are scheduled to be refreshed. The
    source schedule option applies to all tables where the **Schedule**
    field at the table level is set to NULL. Any schedule at the table
    level
    **<span class="underline"><span style="color: #ff0000;">overrides</span></span>**
    the schedule set for the source.. Schedules are created and
    maintained in Common. Refer to [Create
    Schedules](../../Common/Use_Cases/Create_Schedules) for detailed
    information.

<!-- end list -->

1.  Click **Save**.
