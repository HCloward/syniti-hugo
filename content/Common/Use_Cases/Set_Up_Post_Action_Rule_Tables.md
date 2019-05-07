+++
title = 'Set up Post Action Rule Tables'
solution = 'Platform'
+++

# Set up Post Action Rule Tables

Use this generic method to register rules that are used by Collect after
a table download. The benefit of this feature is that the stored
procedure is already written. It only needs to be configured using this
page.

To set up post action rule tables:

  - [Register Procedure as a Rule](#Register_Procedure_as_a_Rule)
  - [Add Post Action Rules Table](#Add_Post_Action_Rules)
  - [Configure Rule
Columns](#Configure_Rule_Columns)

## <span id="Register_Procedure_as_a_Rule"></span>Register Procedure as a Rule

Before the Post Action Rule Table can be used, the
dspCommon.dbo.apiPostActionRuleUpd stored procedure must be registered
as a rule to the table it runs. Refer to the Collect documentation for
detailed information on [registering a rule to a
table](../../Collect/Use_Cases/Add_Rules_and_Indices_to_Tables.htm#Register_Rules_to_Tables).

## <span id="Add_Post_Action_Rules"></span>Add Post Action Rules Table

To add a post action rule table:

1.  Select **Configuration \> Modules \> Post Action Rule Table** in
    *Navigation* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Post Action Rule Table
    page](../Page_Desc/Post_Action_Rule_Table_H.htm)

3.  Enter a table name that is impacted by the table rule in **TABLE**
    field.

4.  Enter a brief description of the table in **DESCRIPTION** field.

5.  Click **Save.**

## <span id="Configure_Rule_Columns"></span>Configure Rule Columns

To configure rule columns:

1.  Select **Configuration \> Modules \> Post Action Rule Table** in the
    *Navigation* pane.

2.  Click the **Rule Columns** icon for the table.

3.  Click **Add**.
    
    [View the field descriptions for the Post Action Rule Table Column
    page](../Page_Desc/Post_Action_Rule_Table_Column.htm).

4.  Enter a column name that is impacted by the table rule in the
    **COLUMN** field .

5.  Select a database rule from the **DATA BASE RULE ID** list box if a
    database rule must be run after the table is downloaded. Refer to
    [Set up Database Functions](Set_up_Database_Functions.htm) to
    register a new database function.

6.  Click the **ACTIVE** check box to activate the rule. If disabled,
    the rule does not run after the table is downloaded.

7.  Enter a brief description of the rule in the **DESCRIPTION** field.
    
    <span style="font-weight: bold;">NOTE:</span> If no description is
    entered, COLUMN RULE is saved in this field by default.

8.  Click **Save.**
