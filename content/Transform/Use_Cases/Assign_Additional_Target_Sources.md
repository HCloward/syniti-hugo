+++
title = 'Assign Additional Target Sources'
solution = 'Migration'
+++

# Assign Additional Target Sources

A Target Source is a record of the relationship between a Source table
and a Target table. Build rules against a Target Source to process
specific Source tables for specific Target tables. This allows multiple
Sources to be registered to a single Target and processed individually.

Transform contains the Target Sources created in Target Design. A Target
Source is a database containing the Source data. Its name begins with
sdb. Additional Source tables can be assigned to a Target.

Refer to [<span class="Body">Manage Target
Sources</span>](Manage_Target_Sources.htm) for more information about
working with Target Sources, including adding Target Source rules and
Target Source reports.

**NOTE:** BackOffice follows a strict naming convention for creating
names that each member of the object can understand. Any manually
created objects must also follow these conventions. Refer to [Naming
Conventions](Naming_Conventions.htm) for more information.

To add Target Sources to a Target in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.

2.  Click the **Sources** icon for a Target.

3.  Click **Add** on the *Target Sources* page in the child pane.
    
    *[View the field descriptions for the Target Sources
    page.](../Page_Desc/Target_Sources_H.htm)*

4.  Enter a value in the
    <span class="StyleListNumberBold" style="font-weight: bold;">PRIORITY</span>
    field.
    
    **NOTE:** If multiple Sources are registered to the Target, the
    priority is the order the Target Source is processed.

5.  Update the
    <span class="StyleListNumberBold" style="font-weight: bold;"><span id="Status" class="popUpLink">STATUS</span></span>
    list box if the default value of Inactive is not applicable.

6.  Select a Source from the
    <span class="StyleListNumberBold" style="font-weight: bold;">SOURCE
    ID</span> list box.
    
    **NOTE:** SOURCE ID is the user friendly name for the Source
    database. This database is assigned to the Source in Target Design,
    and always begins with sdb.

7.  Update the **SOURCE DATABASE OBJECT** list box if the default value
    is not applicable.
    
    **NOTE:** SOURCE CONNECTION TYPE is the Source table from the Source
    database.

8.  Select a type from **SOURCE CONNECTION TYPE** list box.
    
    **NOTE:** Refer to [Data Source Connection
    Types](Data_Source_Connection_Types.htm) for detailed information.

9.  Click
    <span class="StyleListNumberBold" style="font-weight: bold;">Save</span>;
    the *Vertical* View displays.
    
    **NOTE:** The CONNECTION TYPE selected on the *Horizontal* View
    determines which fields display on the General tab and the Process
    Information tab in *Vertical* View. Refer to the following table for
    more information.
    
     
    
    Field

10. Populate all applicable fields.

11. Click
    <span class="StyleListNumberBold" style="font-weight: bold;">Save</span>.
