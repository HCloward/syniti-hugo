+++
title = 'Update System Types for a Source'
solution = 'Migration'
+++

# Update System Types for a Source

A Migration Developer can update the System Type used by a Source.

A Source’s System Types is selected when the data source is registered.

The Source type must be updated if the wrong System Type was selected
when the Source was added to the Target.

Updating the System Type ensures that all Target Sources are assigned
the correct System Type when they are added. It does not affect the
System Type for Sources that have already been mapped.

If the mapping has been completed for the wrong System Type, the fields
for the correct System Type may differ from the wrong one, requiring
that fields must be added, updated or removed. To update a System Type
in this case, use the [Source Where
Used](../Page_Desc/Source_Where_Used.htm) page. Refer to [Sync Source
Data Source-System Types Across all
Targets](Sync_Data_Source_System_Types_Across_Targets.htm) for more
information.

To update a Source’s System Type in Target Design:

1.  Select <span style="font-weight: bold;">Configuration \>
     Source</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Edit</span> for a Source.
    
    [View the field descriptions for the Source
    page](../Page_Desc/Source_Target_Design.htm)

3.  Select the System Type from the
    <span style="font-weight: bold;">SYSTEM TYPE ID</span> list box.
    
    **NOTE:** These System Types are registered in Common.

4.  Enter a brief description of the System Type in the
    <span style="font-weight: bold;">DESCRIPTION</span>  field if
    needed.

5.  Click <span style="font-weight: bold;">Save</span>.
