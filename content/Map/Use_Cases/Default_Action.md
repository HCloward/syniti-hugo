+++
title = 'Default'
solution = 'Migration'
+++

# Default

The Default action is used when mapping a field that should write a
default value to the Target field. For example, if the Target field
should always contain the value “1,” create a rule that populates the
field with this default value for every record that is mapped.

To create a field mapping using the Default action on the
<span style="font-style: italic;">[Field
Mappings](../Page_Desc/Field_Mappings_H)</span> page:

1.  Select the field to be mapped.
    
    [View the field descriptions for the Field Mappings
    page](../Page_Desc/Field_Mappings_H)

2.  Click <span style="font-weight: bold;">Edit</span>.

3.  Select **Default** from the **ACTION** list box.

4.  Enter the default value to write to the Target field in the
    **DEFAULT** field.
    
    **NOTE:** While mapping a field with the Default action, a user can
    create a placeholder to create output values for blank, empty, and
    null values. The rule created by the mapping uses these output
    values. If the user enters \<blank\> in the Default field on the
    Field Mappings page, the output used in the rule is single quotes
    with one space between them (' ').  If the user enters \<empty\>,
    the rule uses single quotes with no space between them (''). If the
    user enters \<null\>, the rules uses NULL, representing no data.

5.  Click **Save**.

6.  Click the <span style="font-weight: bold;">Submit</span> icon on the
    Page toolbar.

**NOTE:** If the Auto Gen Level on the
<span style="font-style: italic;">[Automation](../../SQL_AutoGen/Page_Desc/Automation_page)</span>
page’s <span style="font-style: italic;">Vertical</span> View is set to
Off for the Target, this rule is not built in SQL. If the Auto Gen Level
is set to ON but the Auto Generate Rule check box on the
<span style="font-style: italic;">[Automation SQL Field
Mappings](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H)</span>
page’s <span style="font-style: italic;">Vertical</span> View is
unchecked, then the rule is  not built.

The mapping must be approved by a Developer on the *[Mapping
Approval](../Page_Desc/Mapping_Approval_H)* page for documentation
purposes and to help track progress of the data migration project. Refer
to <span style="color: #0000ff;">[Approve or Reject
Mappings](Approve_or_Reject_Mappings)</span> and
<span style="color: #0000ff;">[Assign Developers to a Target or
Source](../../Design/Use_Cases/Add_Developers_and%20Business%20Contacts)</span>
for more information.

Once the mapping has been submitted, the **Action, Source Table, Source
Field** and **Default Value** fields do not allow updates until one of
the following events occurs:

  - The Developer clicks **Reject** on the *Mapping Approval* page.
  - The Mapper clicks **Reset** on the *Field Mappings* page.

**NOTE**: When a user clicks Reset, Mapping By, Submitted By, Created By
and Approved By field will be reset to NULL values. The Rejected By
field does not update and contains the user ID of the Developer who
rejected the mapping on the <span style="font-style: italic;">Mapping
Approval</span> page. The Mapper can contact the Developer with any
questions.

Once the fields allow update, edit them, click **Save**, and click the
**Submit**icon on the Page toolbar. This updated mapping is sent to the
Developer for review on the *Mapping Approval* page.
