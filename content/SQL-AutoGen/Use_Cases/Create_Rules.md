+++
title = 'Create Rules'
solution = 'Migration'
+++

# Create Rules

A Target Source Rule (also referred to as a Source Rule) cleans and
massages the data before it is loaded in to the target table. SQL
AutoGen generates all source rules to run against the source tables
based on mappings created in Map.

A target rule cleans and manipulates data before it is loaded in to the
target. In Map, these mappings use a source of {Target Rules}. The
{Target Rules} source is where target rules are registered, and SQL
AutoGen uses this source to generate rules that are then run against the
target table.

<span style="font-weight: bold;">NOTE:</span> A source table and target
table must have been built for the object before rules can be generated.

<span style="font-weight: bold;">NOTE:</span> The target’s Design Status
must be In Design or Design Finished to perform this task.

<span style="font-weight: bold;">NOTE:</span> The Mapping Status must be
Complete for a mapping before a rule can be created based on that
mapping. A Rule Status can be updated in SQL AutoGen. Refer to [Update a
Rule Status](Update_a_Rule_Status.htm) for more information.

Each rule consists of a view and a stored procedure that can be created
using SQL AutoGen and stored in the target table.

**NOTE:** If a rule was built in SQL AutoGen, the Created On and Created
By field on the *Vertical* View of the *Field Mappings* page in Map will
be populated. If the Approved On and Approved By fields are empty for
the mapping, the mapping was created in AutoGen and was not approved on
the *Mapping Approval* page.

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

Rules can be created for an individual mapping on the *Automation SQL
Field Mappings* page or for the entire target on the *Automation* page.

To create rules at the target level in AutoGen:

1.  Click the **Automation** tab on the Quick Panel.

2.  Either click the **Create All Rules** icon in the Page toolbar for
    the selected object
    
    Or
    
    Click the **Create And Approve Rules** icon in the Page toolbar for
    the selected object.  

<span style="font-weight: bold;">NOTE:</span> For a rule to be built,  a
mapping’s Mapping Status must be Complete,

To create an individual rule in AutoGen:

1.  Click the **Automation** tab on the Quick Panel.

2.  Click the **Mappings** icon for an Object.

3.  Select a rule.

4.  Click the **Create and Complete** icon in the Page toolbar; a
    confirmation message displays.
    
    **NOTE:** This icon is disabled if the mapping’s Mapping Status is
    not Complete.

5.  Click **OK**.
