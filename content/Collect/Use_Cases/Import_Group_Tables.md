+++
title = 'Import System Types Groups Tables'
solution = 'Platform'
+++

# Import System Types Groups Tables

The import group table(s) process imports System Type group tables from
Common into Collect to facilitate the process of adding sources. This
process also imports the table’s indices and rules. The Fetch process
builds this list or a user can download it from the dspCloud™.

To import group tables:

1.  Click <span style="font-weight: bold;">Collect \> Targets</span> on
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Sources</span> icon for a
    target.

3.  Select a source.

4.  Click <span style="font-weight: bold;">Import Group Tables</span> on
    the Page toolbar.
    
    **NOTE:** The page automatically displays in
    <span style="font-weight: bold;">Edit</span> mode.
    
    [View the field descriptions for the Group Import
    page](../Page_Desc/Group_Import)

5.  Select a System Type group to import from Common as a source from
    <span style="font-weight: bold;">System Type Group ID</span> list
    box. Refer to Common documentation on [System
    Types](../../Common/Use_Cases/Add_System_Types) for detailed
    information.

6.  Select a schedule for when the target is refreshed with source data
    from <span style="font-weight: bold;">Schedule ID</span> list box,
    if the target should be refreshed on a schedule. Otherwise, the
    target is refreshed on-demand via the **Build and Refresh** icon on
    the <span style="font-style: italic;">Targets</span> page. Refer to
    [Common documentation on Create
    Schedules](../../Common/Use_Cases/Create_Schedules) for detailed
    information on creating and modifying a schedule.

7.  Click <span style="font-weight: bold;">Publish Schema Owner</span>
    check box to enable it, which imports the table schema owner to the
    target and overrides the default Target Source schema owner.
    
    **NOTE:** Systems like Oracle EBS must have this option checked.
    Because SAP only has one schema owner for all tables, this options
    is not required for SAP.

8.  Click <span style="font-weight: bold;">Publish Rules</span> check
    box to enable it, which loads rules assigned to the tables in the
    group import to the rule configuration table to update the tables
    when processed.
    
    **NOTE:** If Publish Rules is unchecked, rules assigned to the
    tables do not load into the rule configuration table. In this case,
    there are no rules to process against the table. Once a rule is
    loaded into the table, there is no sync process between the Group
    Import and the current Target Source Table.

9.  Click <span style="font-weight: bold;">Save</span>.

10. Click <span style="font-weight: bold;">Import Table Groups</span> to
    import all group tables, indices and rules into the Target Source; a
    confirmation message displays.

11. Click <span style="font-weight: bold;">Ok</span>.
