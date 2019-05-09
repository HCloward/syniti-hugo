+++
title = 'Add ZActive Fields'
solution = 'Migration'
+++

# Add ZActive Fields

ZActive fields can be added to the Source table to filter out rows to be
inserted into the Target table.

To add a zActive field to a Source table:

1.  Add a field to the Source table in the database.

2.  Click **ProcessArea** in the *Navigation* pane in Map.

3.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map)* page.

4.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.

5.  Click **Vertical View** for the Target Source where the field was
    added.

6.  Click **Edit**.
    
    [View the field descriptions for the Target Sources page's Vertical
    View](../Page_Desc/Target_Sources_H_Map)

7.  Enter a field name starting with “z” in the **Active Field** field,
    for example, zActive\_MARA.

8.  Click **Save**.
    
    **NOTE:** The insert rule checks for this field to equal 1 before
    loading data into the Target table. Manual rules must be written to
    set this flag to 1.

The field entered in the Active Field, for example ZActive, is stored as
a bit field in the database with a value of 0 by default. Before this
field (for example, ZActive) can be moved from the Source to the Target
table, the value must be set to 1 by a manual rule.

To create that rule create a new view in the dsw\[ProcessArea\] database
and select the Target table containing the zActive field and, if
required, the table containing the dependent field(s).

If the Target table contains the dependent field(s), create an update
rule selecting the zActive field in the first row, ‘1’ aliased as
zActiveNew in the second row, add the dependent field(s) in the
proceeding row(s) along with the active filter(s).

If the Update Row table contains the dependent field(s) make the joins
between the tables as needed and create an update rule selecting the
zActive field in the first row, ‘1’ aliased as zActiveNew in the second
row, add the dependent field(s) in the proceeding row(s) along with the
active filter(s).

<span style="font-weight: bold;">NOTE</span>: The dependent field
represents the field that determines whether the record is active or
not.
