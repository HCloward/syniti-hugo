# Add Target Exports

Transform does not load data into an ERP system; it stages data for
export. Target exports are the last sets of rules to move the Target
data to a location so that it can be staged for export to an ERP system
using a loading tool, such as a direct load program or CTS.

This load program is set on the [*Target
Exports*](../Page_Desc/Target_Exports_H.htm) page’s
<span style="font-style: italic;">Horizontal</span> View in the **Load
Type** field.

The Target export view must be manually created in SQL server along with
the Target export tables. The view and table must exist before
registering the Target export in Transform.

**NOTE:** BackOffice follows a strict naming convention for creating
names that each member of the object can understand. Any manually
created objects must also follow these conventions. Refer to [Naming
Conventions](Naming_Conventions.htm) for more information.

**NOTE:** Transform writes export files to the path defined in the
Export Path field on the Transform tab of the
<span style="font-style: italic;">Vertical</span> View of the
<span style="font-style: italic;">[Parameters](../../Console/Page_Desc/Parameters.htm)</span>
page in Console. All export files are written to the path:
C:\\DSW\\Export\\\<Wave Name\>-\<Process Area\>\\\<Target Name\>.  

To register a Target export to a Target in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.

2.  Click the
    <span class="StyleListNumberBold" style="font-weight: bold;">Exports</span>
    icon for a Target.

3.  Click **Add**.
    
    *[View the field descriptions for the Target Exports
    page.](../Page_Desc/Target_Exports_H.htm)*

4.  Enter a sort value in the
    <span class="StyleListNumberBold" style="font-size: 12.0pt;line-height: 115%;font-weight: bold;">PRIORITY</span>
    field.
    
    **NOTE:** If multiple exports exist for the Target, the Priority
    determines the order the export will be processed.

5.  Select a value from the
    <span class="StyleListNumberBold" style="font-weight: bold;"><span id="Status" class="popUpLink">STATUS</span></span>
    list box.

6.  Select a Target from the
    <span class="StyleListNumberBold" style="font-weight: bold;">TARGET
    EXPORT</span> list box.
    
    **NOTE:** This is the manually created view in SQL server.

7.  Select a type from the
    <span class="StyleListNumberBold" style="font-weight: bold;">EXPORT
    TYPE</span> list box.
    
    **NOTE:** The Export Type displays how data is exported from
    Transform. Options include Database, Integrate, Local File and
    Protected Package.
    
    <span style="font-weight: bold;">NOTE:</span> If a user saves a
    Target export with an export type of Local File, an Assemble
    tab-delimited package is created and registered to the export.
    
    **NOTE:** If the export type is Integrate, refer to [Use an
    Integrate Process as an Export
    Type](Use_an_Integrate_Process_as_an_Export_Type.htm) for more
    information.

8.  Select a type from the
    <span class="StyleListNumberBold" style="font-weight: bold;">LOAD
    TYPE</span> list box, if applicable.
    
    **NOTE**: This is the tool or method that will be used for the
    Target export.

9.  Click
    <span class="StyleListNumberBold" style="font-weight: bold;">Save</span>;
    the *Vertical* View displays.
    
    *[View the field descriptions for the Target Exports
    page.](../Page_Desc/Target_Exports_H.htm)*

10. Select a package from the **Export Name** list box.
    
    **NOTE:** Once the Target export is saved, click the package name
    next to Export Name to access the
    *[Packages](../../../Platform/Assemble/Packages_H.htm)* page in
    Assemble (formerly known as "CranPort") to view details about the
    package.

11. Enter the name of the load program used to load the date in the
    <span class="StyleListNumberBold" style="font-weight: bold;">Load
    Program</span> field.

12. Select a name from the
    <span class="StyleListNumberBold" style="font-weight: bold;">Load
    Person</span> list box to indicate the resource who will load the
    data.

13. Enter text in the
    <span class="StyleListNumberBold" style="font-weight: bold;">Load
    Requirements</span> field to tack requirements for the data load.

14. Enter a brief Target export description in the
    <span class="StyleListNumberBold" style="font-weight: bold;">Comment</span>
    field.

15. Click
    <span class="StyleListNumberBold" style="font-weight: bold;">Save</span>.

16. Close the *Vertical* View.

17. Click the <span style="font-weight: bold;">Execute</span> icon for
    the Target export to process the Target export in the background; a
    confirmation message displays.

18. Click **OK**.

<span style="font-weight: bold;">NOTE:</span> If a process takes less
than 0.5 seconds to run, the duration in the DURATION field is 0.
