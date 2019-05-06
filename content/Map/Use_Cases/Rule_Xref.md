# Rule Xref

The RuleXref action is used when mapping a field that contains values
that must be converted before being value mapped.  For example, if two
large companies merge, they may want to convert the Legacy Org Numbers
first and then value map to the new Org numbers (in an Org check table)
in the Target ERP system.

<span style="font-weight: bold;">NOTE:</span> The Rule XRef action
requires a check table to be defined for the field. If a check table is
not already defined for the field, update the System Type for this field
to add a check table. Refer to [Add Check
Tables](../../../Platform/Common/Use_Cases/Add_a%20Lookup%20Table%20Manually..htm)
in the Common documentation.

<span style="font-weight: bold;">NOTE:</span> The RuleXref action must
be used with a lookup table that has multiple key fields. This will
allow missing values in the Target table to be inserted into the Value
Mapping table. The Xref action can only be used with a lookup table that
has a single key field. If the Target Lookup table is a multiple key
table, the Value Mapping process will concatenate Target values from the
multiple key fields into a single field. To map fields on a multiple key
lookup table, use the RuleXref action for the field to be mapped on the
Field Mappings page. RuleXref concatenates Source values and is the
recommended Migration Solution process to load the values correctly into
the Value Mapping process.

<span style="font-weight: bold;">NOTE:</span> When mapping fields on a
multiple key lookup table, concatenate the fields with a ":" separator,
for example, field1:field 2.

<span style="font-weight: bold;">NOTE:</span> The Source table and
Source field for the check table for the Rule Xref action are not
automatically set. They must be entered on the
<span style="font-style: italic;">Vertical</span> View of the [Legacy
Value (Source Table
Fields)](../Page_Desc/Legacy_Value_Source_Table_Fields_H.htm) page.

<span style="font-weight: bold;">NOTE:</span> A lookup table is
registered as a Source table with a status of Documentation and a rule
priority offset of 50000 so that it is sorted last. Documentation
Sources are not processed but are a reference item to see all the
sources of data.

To create a field mapping using the RuleXref action on the
<span style="font-style: italic;">Field Mappings</span> page:

1.  Select the field to be mapped.

2.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Field Mappings
    page](../Page_Desc/Field_Mappings_H.htm)

3.  Select **RuleXref** from the **ACTION** list box.

4.  Select the table that stores the field to be converted and then
    value mapped from the **SOURCE TABLE** list box.
    
    **NOTE:** This table may or may not be a check table.
    
    **NOTE:** When mapping a Source, this field displays the Add Row and
    Update Row Sources for the Add Row Source only. When mapping a
    Target, the field displays any Target in the Wave and Process Area.

5.  Select the field to be converted and then value mapped from the
    **SOURCE FIELD** list box.

6.  Click **Save**; a confirmation message displays.

7.  Click **Yes.**
    
    **NOTE:** A user must create the SQL to convert the value and store
    it in the <span style="font-weight: bold;">Rule SQL</span> field on
    the <span style="font-style: italic;">Vertical</span> View for the
    selected field mapping.

8.  Click the <span style="font-weight: bold;">Vertical View</span>
    icon.

9.  Click <span style="font-weight: bold;">Edit</span>.

10. Enter the SQL to convert the value in the
    <span style="font-weight: bold;">Rule SQL</span> field.

11. Click <span style="font-weight: bold;">Save</span>.

12. Close the <span style="font-style: italic;">Vertical</span> View.

13. Click <span style="font-weight: bold;">Submit</span> on the Page
    toolbar.

**NOTE:** If the Auto Gen Level on the
<span style="font-style: italic;">[Automation](../../SQL_AutoGen/Page_Desc/Automation_page.htm)</span>
page’s <span style="font-style: italic;">Vertical</span> View is set to
Off for the Target, this rule is not built in SQL. If the Auto Gen Level
is set to ON but the Auto Generate Rule check box on the
<span style="font-style: italic;">[Automation SQL Field
Mappings](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H.htm)</span>
page’s <span style="font-style: italic;">Vertical</span> View is
unchecked, then the rule is not built.

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
and Approved By field will be reset to NULL values. The Rejected By
field does not update and contains the user ID of the Developer who
rejected the mapping on the <span style="font-style: italic;">Mapping
Approval</span> page. The Mapper can contact the Developer with any
questions.

Once the fields allow update, edit them, click **Save**, and click the
**Submit** icon on the Page toolbar. This updated mapping is sent to the
Developer for review on the *Mapping Approval* page.

Refer to [Perform Value Mapping](Perform_Value_Mapping_Overview.htm) for
more information on mapping using a RuleXref Action.
