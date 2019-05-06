# Import Sources

A Source is a copy of the original data (system, flat file, database,
etc.) from the legacy system that is being moved into
Transform.  Sources are imported into the Transform processing
database, which brings data into a Transform object and saves time and
resources from manually setting up Sources. 

The Sources that display in Transform depend on the context selected in
the Context bar and the Target selected on the Targets page. Sources are
assigned to Targets in Target Design.

**NOTE:** Multiple Sources can be assigned to a Target in Target Design.

If the user selects a different context in the Context bar, the
Source(s) assigned to Targets in that context is then the Source(s) used
in Transform. Transform provides the ability to import data from an
Excel file, a text file, or another Source table in another database on
the same server into a Source table.

All Sources are imported prior to processing the Targets.

<span style="font-weight: bold;">NOTE:</span> To import the data into
the Source table, the Source Database Object must follow the naming
conventions defined for Source table names. Refer to [Naming Conventions
f](Naming_Conventions.htm)or more information.

<span style="font-weight: bold;">NOTE:</span> Package files used for
import are stored in the path defined in the Source Path field on the
Transform tab of the <span style="font-style: italic;">Vertical</span>
View of the
<span style="font-style: italic;">[Parameters](../../../Data_Quality/dspMonitor/Page_Desc/Parameters.htm)</span>
page in Console. The default path is C:\\DSW\\Source.

To import Source data into a Source table in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.

2.  Click the **Sources** icon for a Target.

3.  Click the **Vertical View** icon for the Source.

4.  Click the **Process Information** tab on the *[Target
    Sources](../Page_Desc/Target_Sources_H.htm)* page.

5.  Click the **Create Import Table** check box to select it to
    automatically generate the Source table; the **View Import Table**
    icon becomes enabled.

6.  Click the **Process** icon in the Page toolbar.

7.  Click the **View Import Table** icon to view the Source table.
    
    <span style="font-weight: bold;">NOTE:</span> This icon is disabled
    if the user has enabled the Create Import Table check box but has
    not processed the Target Source after doing so. The View Import
    Table icon will be disabled until the user clicks the Process icon
    for the Target Source.
