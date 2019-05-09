+++
title = 'Xref'
solution = 'Migration'
+++

# Xref

The Xref action is used when mapping a field that must use value
mapping.

<span style="font-weight: bold;">NOTE:</span> The Xref action requires a
check table to be defined for the field. If a check table is not already
defined for the field, update the System Type for this field to add a
check table. Refer to [Add Check
Tables](../../../Platform/Common/Use_Cases/Add_a%20Lookup%20Table%20Manually.)
in the Common documentation.

<span style="font-weight: bold;">NOTE:</span> The RuleXref action must
be used with a lookup table that has multiple key fields. This will
allow missing values in the Target table to be inserted into the Value
Mapping table. The Xref action can only be used with a lookup table that
has a single key field. If the Target Lookup table is a multiple key
table, the Value Mapping process will concatenate Target values from the
multiple key fields into a single field. To map fields on a multiple key
lookup table, use the RuleXref action for the field to be mapped on the
<span style="font-style: italic;">Field Mappings</span> page. RuleXref
concatenates Source values and is the recommended Migration Solution
process to load the values correctly into the Value Mapping process.

<span style="font-weight: bold;">NOTE:</span> When mapping fields on a
multiple key lookup table, concatenate the fields with a ":" separator,
for example, field1:field 2.

<span style="font-weight: bold;">NOTE:</span> A lookup table is
registered as a Source table with a status of Documentation and a rule
priority offset of 50000 so that it is sorted last. Documentation
Sources are not processed but are a reference item to see all the
sources of data.

In value mapping, the individual value in a Source field is changed to a
value that the Target system will accept in the Target field. For
example, if two large companies merge, they may want to convert the
Legacy Org Numbers first and then value map to the new Org numbers (in
an Org check table) in the Target ERP system.

On the <span style="font-style: italic;">Field Mappings</span> page, set
the field in the Source that must be mapped to the field in the Target.
Configure value mapping using the Value Mappings pages.

Value mapping uses check tables, which are created as part of a System
Type in Common. Refer to [Add Check
Tables](../../../Platform/Common/Use_Cases/Add_a%20Lookup%20Table%20Manually.)
for more information.

When fields with a check table display on the
<span style="font-style: italic;">Field Mappings</span> page, the check
table name displays in the <span style="font-weight: bold;">CHECK
TABLE</span> field. Click the check table name link to configure the
check table.

To create a field mapping using the Xref action on the
<span style="font-style: italic;">Field Mappings</span> page:

1.  Select the field to be mapped.

2.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Field Mappings
    page](../Page_Desc/Field_Mappings_H)

3.  Select **Xref** from the **ACTION** list box.

4.  Select the table that stores the field to be value mapped from the
    **SOURCE TABLE** list box.
    
    **NOTE:** This table may or may not be a check table, but is the
    table that stores the values to be mapped.
    
    **NOTE:** When mapping a Source, this field displays the Add Row and
    Update Row Sources for the Add Row Source only. When mapping a
    Target, the field displays any Target in the Wave and Process Area.

5.  Select the field to be value mapped from the **SOURCE FIELD** list
    box.

6.  Click **Save**.

7.  Click the <span style="font-weight: bold;">Submit</span> icon on the
    Page toolbar.

**NOTE:** If the Auto Gen Level on the
<span style="font-style: italic;">[Automation](../../SQL_AutoGen/Page_Desc/Automation_page)</span>
page’s <span style="font-style: italic;">Vertical</span> View is set to
Off for the Target, this rule is not built in SQL. If the Auto Gen Level
is set to ON but the Auto Generate Rule check box on the
<span style="font-style: italic;">[Automation SQL Field
Mappings](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H)</span>
page’s <span style="font-style: italic;">Vertical</span> View is
unchecked, then the rule is not built.

The mapping must be approved by a Developer on the *[Mapping
Approval](../Page_Desc/Mapping_Approval_H)* page for documentation
purposes and to help track progress of the data migration project. Refer
to <span style="color: #0000ff;">[Approve or Reject
Mappings](Approve_or_Reject_Mappings)</span> and
<span style="color: #0000ff;">[Assign Developers to a Target or
Source](../../Design/Use_Cases/Add_Developers_and%20Business%20Contacts)</span>
for more information.

Once the mapping has been created, the **Action, Source Table, Source
Field** and **Default Value** fields do not allow updates until one of
the following events occurs:

  - The Developer clicks **Reject** on the *Mapping Approval* page.
  - The Mapper clicks **Reset** on the *Field Mappings* page.

**NOTE:** When a user clicks Reset, Mapping By, Submitted By, Created By
and Approved By field will be reset to NULL values. The Rejected By
field does not update and contains the user ID of the Developer who
rejected the mapping on the <span style="font-style: italic;">Mapping
Approval</span> page. The Mapper can contact the Developer with any
questions.

Once the fields allow update, edit them, click **Save**, and click the
**Submit** icon on the Page toolbar. This updated mapping is sent to the
Developer for review on the *Mapping Approval* page.

Refer to [Perform Value Mapping](Perform_Value_Mapping_Overview) for
more information on mapping using an Xref action.
