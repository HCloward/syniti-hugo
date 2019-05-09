+++
title = 'Build and Refresh Tables for a Schedule Group'
solution = 'Platform'
+++

# Build and Refresh Tables for a Schedule Group

Create a schedule group for a group of Target Source tables to build
and/or refresh an isolated group of tables. A schedule group could be a
group of tables for a specific business unit, or for a list of material,
customer or configuration tables.

To create a schedule group for a Target Source, refer to [Set up
Schedule Groups](../Config/Set_Up_Schedule_Groups). <span>When a
schedule group is assigned to a table, this table displays on the
</span><span style="font-style: italic;">[Target Source
Tables](../Page_Desc/Target_Source_Tables)</span><span> page.</span>

A user can add or remove tables from the schedule group to limit build
and refresh to a specific set of tables on that page.

To build and refresh tables for a schedule group:

1.  Click <span style="font-weight: bold;">Targets</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Sources</span> for a target.

3.  Click <span style="font-weight: bold;">Schedule Groups</span> for a
    Target Source.

4.  Select a schedule group.
    
    **NOTE:** Only schedule groups that are selected for tables within
    the source display.

5.  Click the <span style="font-weight: bold;">Tables</span> icon to
    view the tables that are built and refreshed for the selected
    schedule group.
    
    **NOTE:** Tables for the schedule group can be added or deleted on
    the <span style="font-style: italic;">[Target Source
    Tables](../Page_Desc/Target_Source_Tables)</span><span> page..
    </span>To add tables if needed. refer to [Manually Register Tables
    to Source](Manually_Register_Tables_to_Source) for more
    information.

6.  Click <span style="font-weight: bold;">Build Package</span> to build
    a package to download all active tables in the schedule group from
    the source database.
