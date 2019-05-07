+++
title = 'Not Used'
solution = 'Migration'
+++

# Not Used

The Not Used action is used when a field that is available in the Source
system will not be loaded into the Target system. The field is not used
for the selected Source, but may be used for other Source systems. A
field that is Not Used is mapped for reporting and metrics purposes.

<span style="font-weight: bold;">NOTE</span>: Unmapped Target or Target
Source fields can be automatically set to NotUsed. Refer to [Update
Unmapped Fields to NotUsed](Update_Unmapped_Fields_to_NotUsed.htm) for
more information.

<span style="font-weight: bold;">NOTE</span>: A mapping with a Not Used
action cannot be saved unless the fields SOURCE TABLE, SOURCE FIELD,
DEFAULT VALUE, and RULE SQL on the
<span style="font-style: italic;">Horizontal</span> View are blank and
the Target Relationship ID field on the
<span style="font-style: italic;">Vertical</span> View is empty on the
<span style="font-style: italic;">Field Mappings</span> page.

To create a field mapping using the Not Used action on the
<span style="font-style: italic;">[Field
Mappings](../Page_Desc/Field_Mappings_H.htm)</span> page:

1.  Select the field to be mapped.

2.  Click <span style="font-weight: bold;">Edit</span>.
    
    <span>[View the field descriptions for the Field Mappings
    page](../Page_Desc/Field_Mappings_H.htm)</span> 

3.  Select **Not Used** from the **ACTION** list box.

4.  Click **Save**.

5.  Click the <span style="font-weight: bold;">Submit</span> icon on the
    Page toolbar.

The mapping must be approved by a Developer on the *[Mapping
Approval](../Page_Desc/Mapping_Approval_H.htm)* page for documentation
purposes and to help track progress of the data migration project. Refer
to <span style="color: #0000ff;">[Mapping
Approval](Approve_or_Reject_Mappings.htm)</span> and
<span style="color: #0000ff;">[Assign Developers to a Target or
Source](../../Design/Use_Cases/Add_Developers_and%20Business%20Contacts.htm)</span>
for more information.

Once the mapping has been submitted, the **Action, Source Table, Source
Field** and **Default Value** fields do not allow updates until one of
the following events occurs:

  - The Developer clicks **Reject** on the *Mapping Approval* page.
  - The Mapper clicks **Reset** on the *Field Mappings* page.

**NOTE**: When a user clicks Reset, Mapping By, Submitted By, Created By
and Approved By field will be reset to NULL values.  The Rejected By
field does not update and contains the user ID of the Developer who
rejected the mapping on the <span style="font-style: italic;">Mapping
Approval</span> page. The Mapper can contact the Developer with any
questions.

Once the fields allow update, edit them, click **Save**, and click the
**Submit** icon on the Page toolbar. This updated mapping is sent to the
Developer for review on the *Mapping Approval* page.
