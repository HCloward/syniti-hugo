# Create Rules for an Update Row Source

A Target Source Rule (also referred to as a Source Rule) cleans and
massages the data before it is loaded in to the target table. SQL
AutoGen generates all source rules to run against the source tables
based on mappings created in Map.

**NOTE:** A [source table](Build_Source_Tables.htm) and [target
table](Build_Target_Tables.htm) must have been built for the object
before rules can be generated.

**NOTE:** The target’s Design Status must be In Design or Design
Finished to perform this task.

Each rule consists of a view and a stored procedure that can be created
using SQL AutoGen and stored in the target table.

**NOTE:** If a rule was built in SQL AutoGen, the Created On and Created
By field on the *Vertical* View of the *[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)* page in Map will be
populated. If the Approved On and Approved By fields are empty for the
mapping, the mapping was created in AutoGen and was not approved on the
*[Mapping Approval](../../Map/Page_Desc/Mapping_Approval_H.htm)* page.

Once the rules are created for the field using SQL AutoGen, the
view(s)/procedure(s) (one for each rule assigned) will be available and
registered in Transform.

Update and insert rules used in Transform are automatically generated
and saved to the target database.

<span style="font-weight: bold;">NOTE:</span> A user can create all
target tables, source tables, Update Row source tables, and rules at one
time by clicking the Create All Objects icon on the
<span style="font-style: italic;">[Automation](../Page_Desc/Automation_page.htm)</span>
page.

All objects created using SQL AutoGen are written to the data source
defined for the object in Console (Process Area \> Objects \> Vertical
View \> Data Source ID).

Rules can be created for an individual mapping on the *[Automation SQL
Field Mappings](../Page_Desc/Automation_SQL_Field_Mappings_H.htm)* page
or for the entire target on the
*[Automation](../Page_Desc/Automation_page.htm)* page.

To create rules for an Update Row Source in AutoGen:

1.  Click the **Automation** tab in the Quick Panel.

2.  Click the **Sources** icon for a Target.
    
    **NOTE:** The a page displays behind the
    *[Automation](../Page_Desc/Automation_page.htm)* page and, depending
    on how the user’s view is configured, may be obstructed by the
    *Automation* page itself.  In this case, to view the *[Automation
    SQL Target Source](../Page_Desc/Automation_SQL_Target_Source.htm)*
    page either close the *Automation* page or reduce the size of the
    *Automation* page.

3.  Select the source on the
    <span style="font-style: italic;">[Automation SQL Target
    Source](../Page_Desc/Automation_SQL_Target_Source.htm)</span> page
    in the Parent pane.

4.  Select the Update Row source on the
    <span style="font-style: italic;">[Automation SQL Target Source
    (Update
    Row)](../Page_Desc/Automation_SQL_Target_Source_Update_Row.htm)</span>
    page in the Child pane.

5.  Click the **Create All Rules** icon in the Page toolbar; a
    confirmation message displays.

6.  Click **OK**.
