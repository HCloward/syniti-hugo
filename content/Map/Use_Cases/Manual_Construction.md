# Manual Construction

The Manual Construction action is used when a rule is too complex to be
automatically generated and will be written manually in Construct.

<span style="font-weight: bold;">NOTE</span>: When a field mapping’s
action is set to Manual Construction, the Source associated with the
field is automatically added to the zSource page in Construct, and the
user does not need to manually enter the zSource. Refer to [Set up
 zSources](../../Construct/Config/Set_up_ZSources.htm) for more
information.

<span style="font-weight: bold;">NOTE</span>: When a mapping with an
action of Manual Construction is saved, the Instruction field on the
<span style="font-style: italic;">Vertical</span> View of the
<span style="font-style: italic;">Field Mappings</span> page for the
mapping indicates that the rule requires development. The Rule Name
field displays “Developer must create the rule.”

<span style="font-weight: bold;">NOTE</span>: A mapping with a Manual
Construction action cannot be saved unless the fields SOURCE TABLE,
SOURCE FIELD, DEFAULT VALUE, and RULE SQL on the
<span style="font-style: italic;">Horizontal</span> View are blank and
the Target Relationship ID field on the
<span style="font-style: italic;">Vertical</span> View is empty on the
<span style="font-style: italic;">Field Mappings</span> page.

To create a field mapping using the Manual Construction action on the
*[Field Mappings](../Page_Desc/Field_Mappings_H.htm)* page:

1.  Select <span style="font-weight: bold;">ProcessArea</span> in the
    *Navigation* pane.  

2.  Click the **Targets**icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map.htm)* page.

3.  Click the **Mappings** icon for a Target.

4.  Select the field to be mapped.

5.  Click **Edit**.
    
      <span style="color: #0000ff;">[View the field descriptions for the
    Field Mappings page](../Page_Desc/Field_Mappings_H.htm)</span>

6.  Select **Manual Construction** from the **ACTION** list box.

7.  Enter Mapper's notes in the **RULES COMMENT** field.

8.  Enter as much technical information available for the developer to
    build the rule.

9.  Click **Save**.

10. Click the **Submit** icon on the Page toolbar.

The mapping must be approved by a Developer on the *[Mapping
Approval](../Page_Desc/Mapping_Approval_H.htm)* page for documentation
purposes and to help track progress of the data migration project. Refer
to <span style="color: #0000ff;">[Approve or Reject
Mappings](Approve_or_Reject_Mappings.htm)</span> and
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
