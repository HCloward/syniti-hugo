+++
title = 'Add Add Row Sources'
solution = 'Migration'
+++

# Add Add Row Sources

An Add Row Source is the Source table where records are migrated from
and inserted into the target table. Records in an Add Row Source table
are used for reconciliation.

An Add Row Source is added in Target Design. Refer to [Assign a Source
to a Target](../../Design/Use_Cases/Assign_a_Source_to_a_Target) for
more information.

An additional Add Row Source can also be added in Map.

Add an Add Row Source if another Source database object is needed from
the same system for the same target table. For example, the same Source
system has two tables for customers, one table contains SoldTos and
another contains ShipTos. Both these tables are in the same system and
need to be migrated to the target table ttKNA1.

A Target Source can have multiple Add Row Sources. Each Add Row Source
can have multiple Update Row Sources.

<span style="font-weight: bold;">NOTE</span>: An Add Row Source is not
added to another Add Row Source, but is added as a separate Add Row
Source.

<span style="font-weight: bold;">NOTE</span>: After Add Row Sources are
added, their fields are mapped on the
<span style="font-style: italic;">[Field
Mappings](../Page_Desc/Field_Mappings_H)</span> page. To map all Add
Row Sources, the <span style="font-style: italic;">Field Mappings</span>
page must be accessed by clicking the Mappings icon on the [Target
Sources (Add Row)](../Page_Desc/Target_Sources_Add_Row) page. Refer
to [Access the Field Mappings
Page](Perform_Field_Mapping#Access_the_Field_Mappings_Page) for more
information.

To add an Add Row Source in Map:

1.  Click <span style="font-weight: bold;">ProcessArea</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map)* page.

3.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    target.

4.  Click <span style="font-weight: bold;">Add</span>
    
    [View the field descriptions for the Target Sources
    page](../Page_Desc/Target_Sources_H_Map)

5.  Select the Source name from the
    <span style="font-weight: bold;">Source ID</span> list box.

6.  Select the object from the <span style="font-weight: bold;">Source
    DATABASE OBJECT</span> list box.
    
    **NOTE:** This database is registered in Common. Refer to [Register
    a Data Source in
    Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common)
    for more information

7.  Click <span style="font-weight: bold;">Save</span>; the
    <span style="font-style: italic;">Vertical</span> View displays.

8.  Enter the name of the Source that overrides the zSource for the
    target configured in Target Design in the
    <span style="font-weight: bold;">z Source Override</span> field.
    
    **NOTE**: The z Source Override field must be completed for Add Row
    Sources so that delete rules do not delete target data from the
    wrong table.

9.  Click <span style="font-weight: bold;">Save</span>.
