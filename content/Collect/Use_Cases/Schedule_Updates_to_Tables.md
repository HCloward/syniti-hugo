# Schedule Updates to Tables

The Schedule Updates functionality clears or updates all manually set
source and table schedules to provide mass updates to schedules for
targets and sources.

**NOTE:** Collect schedule table updates can be done quickly for
**<span class="underline"><span style="color: #ff0000;">all</span></span>**
tables in a Source. Use this method rather than directly updating the
schedules via the [<span style="font-style: italic;">Target Source
Tables</span>](../Page_Desc/Target_Source_Tables.htm) page so the new
Next Schedule Run Times are calculated correctly.

This feature covers the following topics:

  - [Clear All Schedules](#Clear_All_Schedules)

  - [Update All Schedules](#Update_All_Schedules)

## <span id="Clear_All_Schedules"></span>Clear All Schedules

If the target does not need to be refreshed anymore, clear all
schedules.

To clear all schedules for targets and sources:

1.  Select **Tools \> Bulk Table Schedule Update** in *Navigation* pane.

2.  Click **Edit**.
    
    [View the field descriptions for the Bulk Table Schedule Update
    page.](../Page_Desc/Bulk_Table_Schedule_Update.htm)

3.  Select a target database from **Schedule Target** list box.

4.  Select a source database from **Schedule Source** list box. This
    field maybe left blank for a Clear Schedule process, but must be
    populated for an Update Schedule process
    
    OR
    
    Leave **Schedule Sources** blank to update all sources.

5.  Click **Save**.

6.  Click **Clear Schedule**; a confirmation message displays. If
    Schedule Source is blank, all sources for the selected target are
    cleared.

7.  Click **Ok**.

## <span id="Update_All_Schedules"></span>Update All Schedules

If all targets need to be refreshed at a time other than on the schedule
defined for the targets, use this feature to update all the schedules at
once.

To update all schedules for a target and a source:

1.  Select **Tools \> Bulk Table Schedule Update** in *Navigation* pane.

2.  Click **Edit**.
    
    [View the field descriptions for the Bulk Table Schedule Update
    page.](../Page_Desc/Bulk_Table_Schedule_Update.htm)

3.  Select a target database from **Schedule Target** list box.

4.  Select a source database from **Schedule Source** list box.
    
    OR
    
    Leave **Schedule Sources** blank to update NULL or empty sources.

5.  Select a schedule to **Schedule To** list box.

6.  Click **Save**.

7.  Click **Update Schedule**; a confirmation message displays.

8.  Click **Ok**.
