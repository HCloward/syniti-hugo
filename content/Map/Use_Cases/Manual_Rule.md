+++
title = 'Manual Rule'
solution = 'Migration'
+++

# Manual Rule

The Manual Rule action is used when a rule is too complex to be
automatically generated and must be written.

<span style="font-weight: bold;">NOTE</span>: Basic and Complex rules
are managed in Target Design. They are not edited or submitted in Map.
The mapping for a field with either a complex rule or both a complex and
a basic rule displays in Map with an Action of Manual Rule.  Refer to
[Add a Basic Rule](../../Design/Use_Cases/Basic_Rules.htm) and [Add a
Complex Rule](../../Design/Use_Cases/Complex_Rules.htm) for more
information.

<span style="font-weight: bold;">NOTE</span>: A mapping with a Manual
Rule action cannot be saved unless the fields SOURCE TABLE, SOURCE
FIELD, DEFAULT VALUE, and RULE SQL on the
<span style="font-style: italic;">Horizontal</span> View are blank and
the Target Relationship ID field on the
<span style="font-style: italic;">Vertical</span> View is empty on the
<span style="font-style: italic;">Field Mappings</span> page.

To create a field mapping using the Manual Rule action on the
<span style="font-style: italic;">[Field
Mappings](../Page_Desc/Field_Mappings_H.htm)</span> page:

1.  Select the field to be mapped.

2.  Click <span style="font-weight: bold;">Edit</span>.
    
        [View the field descriptions for the Field Mappings
    page](../Page_Desc/Field_Mappings_H.htm)

3.  Select **Manual Rule** from the **ACTION** list box.

4.  Enter Mapper's notes in the <span style="font-weight: bold;">RULES
    COMMENT</span> field.
    
    **NOTE:** Enter as much technical information available for the
    developer to build the rule.

5.  Click **Save**.

6.  Click the <span style="font-weight: bold;">Submit</span> icon on the
    Page toolbar.

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

  - The Developer clicks **Reject** on the *Mapping Approval* page.
  - The Mapper clicks **Reset** on the *Field Mappings* page.

**NOTE**: When a user clicks Reset, Mapping By, Submitted By, Created By
and Approved By field will be reset to NULL values. The Rejected By
field does not update and contains the user ID of the Developer who
rejected the mapping on the <span style="font-style: italic;">Mapping
Approval</span> page. The Mapper can contact the Developer with any
questions.

Once the fields allow update, edit them, click **Save**, and click the
**Submit**icon on the Page toolbar. This updated mapping is sent to the
Developer for review on the *Mapping Approval* page.
