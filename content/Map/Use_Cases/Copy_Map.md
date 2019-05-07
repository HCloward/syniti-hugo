+++
title = 'Copy'
solution = 'Migration'
+++

# Copy

The Copy action is used when mapping a field that is an exact copy from
the Source to the Target.

<span style="font-weight: bold;">NOTE:</span> If the user clicked the
Auto Map icon on the <span style="font-style: italic;">[Target
Sources](../Page_Desc/Target_Sources_H_Map.htm)</span> page for the
Source, any auto mapped fields are set to the Copy action with a Mapping
Status of In Progress.

To create a field mapping using the Copy action on the
<span style="font-style: italic;">Field Mappings</span> page:

1.  Select the field to be mapped.

2.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Field Mappings
    page](../Page_Desc/Field_Mappings_H.htm)

3.  Select **Copy** from the **ACTION** list box.

4.  Select the table that stores the field to be copied from the
    **SOURCE TABLE** list box.
    
    **NOTE:** When mapping a Source, this field displays the Add Row and
    Update Row Sources for the Add Row Source only. When mapping a
    Target, the field displays any Target in the Wave and Process Area.

5.  Select the field in the <span style="font-weight: bold;">SOURCE
    TABLE</span> to be copied from the **SOURCE FIELD** list box.

6.  Click <span style="font-weight: bold;">Submit</span> on the Page
    toolbar.

**NOTE:** If the <span>Auto Gen Level on the
</span><span style="font-style: italic;">[Automation](../../SQL_AutoGen/Page_Desc/Automation_page.htm)</span><span>
page’s </span><span style="font-style: italic;">Vertical</span><span>
View is set to Off for the Target</span>, this rule is not built in SQL.
If the Auto Gen Level is set to ON but the Auto Generate Rule check box
on the <span style="font-style: italic;">[Automation SQL Field
Mappings](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H.htm)</span>
page’s <span style="font-style: italic;">Vertical</span> View is
unchecked, then the rule is  not built.

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

  - The Developer clicks the **Reject** icon on the *Mapping Approval*
    page.
  - The Mapper clicks the **Reset** icon on the *Field Mappings* page.

**NOTE**: When a user clicks Reset, Mapping By, Submitted By, Created By
and Approved By field will be reset to NULL values.  The Rejected By
field does not update and contains the user ID of the Developer who
rejected the mapping on the <span style="font-style: italic;">Mapping
Approval</span> page. The Mapper can contact the Developer with any
questions.

Once the fields allow update, edit them, click **Save**, and click the
**Submit** icon on the Page toolbar. This updated mapping is sent to the
Developer for review on the *Mapping Approval* page.
