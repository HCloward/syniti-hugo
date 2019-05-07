+++
title = 'Rule'
solution = 'Migration'
+++

# Rule

The Rule action is used when the field mapping for a field is performed
by a rule that is written by the user.

<span style="font-weight: bold;">NOTE</span>: Basic rules are managed in
Target Design. They are not edited or submitted in Map. The mapping for
a field with a basic rule displays in Map with an Action of Rule. Refer
to [Add a Basic Rule](../../Design/Use_Cases/Basic_Rules.htm) for more
information.

<span style="font-weight: bold;">NOTE</span>:  The SOURCE TABLE and
SOURCE FIELD fields should be empty when saving a mapping with a Rule
action. Include the Source table and field in the Rule SQL field on the
<span style="font-style: italic;">Vertical</span> View of the
<span style="font-style: italic;">Field Mappings</span> page.

To create a field mapping using the Rule action on the
<span style="font-style: italic;">[Field
Mappings](../Page_Desc/Field_Mappings_H.htm)</span> page:

1.  Select the field to be mapped.

2.  Click <span style="font-weight: bold;">Edit</span>.
    
     [View the field descriptions for the Field Mappings
    page](../Page_Desc/Field_Mappings_H.htm)

3.  Select the **Rule** icon from the **ACTION** list box.

4.  Click **Save**;a confirmation message displays.

5.  Click<span style="font-weight: bold;">Yes</span>.
    
    **NOTE:** A user must create the SQL and store it in the
    <span style="font-weight: bold;">Rule SQL</span> field on the
    <span style="font-style: italic;">Vertical</span> View for the
    selected field mapping.

6.  Click the **Vertical View** icon for the field mapping.

7.  Click **Edit.**
    
    [View the field descriptions for the Field Mappings page's Vertical
    View](../Page_Desc/Field_Mappings_H.htm#Field_Mappings_V)

8.  Enter the rule in the **Rule SQL** field.

9.  Click **Save**.

10. Close the *Vertical* View.

11. Click the <span style="font-weight: bold;">Submit</span> icon on the
    Page toolbar.

**NOTE:** If the Auto Gen Level on the
<span style="font-style: italic;">[Automation](../../SQL_AutoGen/Page_Desc/Automation_page.htm)</span>
page’s <span style="font-style: italic;">Vertical</span> View is set to
Off for the Target, this rule is not built in SQL. If the Auto Gen Level
is set to ON but the Auto Generate Rule check box on the
<span style="font-style: italic;">[Automation SQL Field
Mappings](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H.htm)</span>
page’s <span style="font-style: italic;">Vertical</span> View is
unchecked, then the rule is  not built.

The mapping must be approved by a Developer on the *[Mapping
Approval](../Page_Desc/Mapping_Approval_H.htm)* page for documentation
purposes and to help track progress of the data migration project. Refer
to <span style="color: #0000ff;">[Mapping
Approvals](Approve_or_Reject_Mappings.htm)</span> and
<span style="color: #0000ff;">[Assign Developers to a Target or
Source](../../Design/Use_Cases/Add_Developers_and%20Business%20Contacts.htm)</span>
for more information.

Once the mapping has been submitted, the **Action, Source Table, Source
Field** and **Default Value** fields do not allow updates until one of
the following events occurs:

  - The Developer clicks **Reject** on the *Mapping Approval* page
  - The Mapper clicks **Reset** on the *Field Mappings* page

**NOTE**: When a user clicks Reset, Mapping By, Submitted By, Created By
and Approved By field will be reset to NULL values.  The Rejected By
field does not update and contains the user ID of the Developer who
rejected the mapping on the <span style="font-style: italic;">Mapping
Approval</span> page. The Mapper can contact the Developer with any
questions.

Once the fields allow update, edit them, click **Save**, and click the
**Submit** icon on the Page toolbar. This updated mapping is sent to the
Developer for review on the *Mapping Approval* page.
