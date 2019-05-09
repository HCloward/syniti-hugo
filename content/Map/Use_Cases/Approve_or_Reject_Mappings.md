+++
title = 'Approve or Reject Mappings'
solution = 'Migration'
+++

# Approve or Reject Mappings

In the Mapping Approval process:

1.  A Mapper configures a mapping in Map,
    <span style="text-indent: -.25in;">saves the mapping, and then
    clicks Submit on the Page toolbar of the *[Field
    Mappings](../Page_Desc/Field_Mappings_H)* page.</span>
2.  The Developer clicks the green tab on the Quick Panel to open the
    *[*Mapping Approval*](../Page_Desc/Mapping_Approval_H)* page to
    view mappings waiting for approval.
3.  The Developer reviews the mapping and either approves or rejects it.

When a mapping is approved or rejected, Mapping Status and Rule Status
are updated. Refer to [Mapping Status and Rule
Status](Mapping_Status_and_Rule_Status) for more information.

**NOTE**: A mapping can also be rejected in SQL AutoGen. Refer to
[Reject a Mapping](../../SQL_AutoGen/Use_Cases/Reject_a_Mapping) for
more information.

Every field mapping must be approved by a Developer on the *Mapping
Approval* page. Once approved,  the mapping is considered complete and
is tracked as “Complete” on Wave gate metrics reports. The rule for the
mapping can then be generated in AutoGen.

**NOTE**: A Developer can click the Complete icon to approve the
mapping, and set the Mapping Status and Rule Status for the selected
mapping to Complete. When a mapping is approved, the Rule Status is set
to In Progress by default. Clicking the Complete icon bypasses the In
Process status. The rule can then be created in SQL AutoGen.

Once the Developer has approved or rejected a mapping, the mapping no
longer displays on the *Mapping Approval* page.

## Security Configuration for Developers

To view the *Mapping Approval* page on the Quick Panel, a Developer must
be assigned to a role that has the MappingApproval WebApp Group assigned
to it. An Administrator assigns WebApp Groups to a security role. If a
Developer is not assigned to a role with the MappingApproval WebApp
Group assigned to it, the Mapping Approval tab does not display on the
Quick Panel.

A Developer should also be assigned Transform access (PowerUser Group)
and Target Design access (PowerUser Group)

To view mappings on the *Mapping Approval* page, a Developer must be
assigned to the Target or Source in Target Design. Refer to [Assign
Developers to a Target or
Source](../../Design/Use_Cases/Add_Developers_and%20Business%20Contacts)
for more information.

This section contains the following topics:

  - [Download Mappings for Review](#Download_Mappings_for_Review)
  - [Approve the Mapping](#Approve_the_Mapping)
  - [Reject the Mapping](#Reject_the_Mapping)
  - [Approve or Reject Multiple
    Mappings](#Approve_or_Reject_Multiple_Mappings)

## <span id="Download_Mappings_for_Review"></span>Download Mappings for Review

To facilitate review of mappings, a Developer can download all mappings
to a Word or Excel file.

A Developer can select how to receive notifications when mappings are
ready for review. Refer to [Set Message Types for Mapping
Review](../../Console/Use_Cases/Set_Message_Types_for_Mapping_Review)
for more information.

To download mappings:

1.  Click the **Mapping Approval** tab in the Quick Panel,

2.  Click the **Download List** icon in the Page toolbar.
    
    **NOTE**: The *[Mapping Approval Download
    List](../Page_Desc/Mapping_Approvals_Download_List)* page
    displays behind the *[Mapping
    Approval](../Page_Desc/Mapping_Approval_H)* page and, depending
    on how the user’s view is configured, may be obstructed by
    the  *Mapping Approval* page itself.  In this case, to view the
    *Mapping Approval Download List* page, either close the *Mapping
    Approval* page or reduce the size of the *Mapping Approval* pane.

3.  Click the gear icon to the right of the help icon.

4.  Select **Download**.

5.  Select the format to use when downloading the file on the **Format**
    tab.

6.  Click the **Fields** tab.

7.  Check the check box for each field that should be downloaded.

8.  Click the **Options** tab.

9.  Set options as needed.

10. Click the **Download** icon.

## <span id="Approve_the_Mapping"></span>Approve the Mapping

To approve the mapping, the Developer selects the mapping and clicks
Approve.

**NOTE:** A Developer can select multiple mappings and click **Approve**
for the group.  Refer to [Approve or Reject Multiple
Mappings](#Approve_or_Reject_Multiple_Mappings) for more information.

**NOTE:** If the *[Field Mappings](../Page_Desc/Field_Mappings_H)*
page is open in Map when a mapping is approved, refresh the *Field
Mappings* page manually to see the update.

The RULE STATUS for the mapping is set to “In Progress” on the *Field
Mappings* page in Map. The mapping is then counted as “complete” on Wave
gate metrics reports.

## <span id="Reject_the_Mapping"></span>Reject the Mapping

To reject the mapping, the Developer:

1.  Clicks **Edit** for the mapping on the
    <span style="font-style: italic;">[Mapping
    Approval](../Page_Desc/Mapping_Approval_H)</span> page.

2.  Enters a comment with the rejection reason for the mapping in the
    **Comment** field.
    
    **NOTE:** If the action for the mapping is Manual, Rule or RuleXref,
    the Developer can update the SQL code for the rule in the Rule SQL
    field. The Rule SQL field only displays when the action for the
    selected mapping is Manual, Rule or RuleXref.

3.  Clicks **Save**.

4.  Clicks **Reject**.

<span style="font-weight: bold;">NOTE:</span> When the developer rejects
the mapping, the Mapped By and Mapped On fields in Map are set to NULL.

**NOTE:** A Developer can select multiple mappings and click **Reject**
for the group. Refer to [Approve or Reject Multiple
Mappings](#Approve_or_Reject_Multiple_Mappings) for more information.

**NOTE:** Back in Map, the RULE STATUS for the mapping on the *[Field
Mappings](../Page_Desc/Field_Mappings_H)* page is changed to
Revision Requested and the MAPPING STATUS is changed from Complete to
Design Required. The comment added by the Developer on the *Mapping
Approval* page displays in Map on the *Field Mappings* page’s *Vertical*
View in the Comment field.

**NOTE:** If the *Field Mappings* page is open in Map when a mapping is
rejected, refresh the *Field Mappings* page manually to see the update.

## Correct the Rejected Mapping

To continue the Mapping Approval process in the case of a rejection the
following steps are completed in Map:

1.  The Mapper selects the mapping and clicks **Reset** on the Page
    toolbar.
    
    <span style="font-weight: bold;">NOTE:</span> When a user clicks
    Reset, the **Created By** and Created On fields, on the
    <span style="font-style: italic;">Vertical</span> View of the *Field
    Mappings* page, are cleared.
    
    **NOTE:** If the original mapping action created a rule in
    Transform, what happens to that rule when it is reset in Map is
    determined by a parameter set in Console on the Map tab of the
    *[Parameters](../../Console/Page_Desc/Parameters)* page. In the
    Reset Transform Rule list box, the following options are available:
    
      - **Deactivate Transform Rule** – The status of the rule Map
        created during the mapping process and registered in Transform
        is changed to Inactive in Transform when the mapping is reset in
        Map.
      - **Delete Transform Rule** – The rule Map created during the
        mapping process and registered in Transform is deleted when the
        mapping is reset in Map. The rule is deleted from the database
        and its registrations are removed from Transform.
      - **Ignore Transform Rule** – The rule Map created during the
        mapping process and registered in Transform is not affected by
        the reset.

2.  The Mapper makes the corrections to the mapping as requested by the
    Developer, and sets the MAPPING STATUS to Complete.

3.  The Mapper saves the rule and clicks **Submit** icon on the Page
    toolbar.

4.  Map drops the SQL Objects associated with the incorrect mapping and
    builds new Objects. The names of these Objects do not change in the
    database.

**NOTE:** If the mapping had an Action of Construction, the page created
in Construct is not deleted. It must be manually deleted from the
database.

Map creates a record on the *Mapping Approval* page and the review
process begins
again.

## <span id="Approve_or_Reject_Multiple_Mappings"></span>Approve or Reject Multiple Mappings

A Developer can select multiple mappings and approve or reject them as a
group on the *[Mapping Approval](../Page_Desc/Mapping_Approval_H)*
page.

To approve multiple mappings in Map:

1.  Click the **Mapping Approval** tab on the Quick Panel.

2.  Select multiple mappings.
    
    **NOTE:** To select a contiguous range of items, hold down the
    **Shift** key and select the first and last items in the range. To
    select a non-contiguous range of items, hold down the **Ctrl** key
    and select each item.

3.  Click **Approve**.
    
    **NOTE:** If the *[Field
    Mappings](../Page_Desc/Field_Mappings_H)* page is open in Map
    when multiple mappings are approved, refresh the *Field Mappings*
    page manually to see the update.

To reject multiple mappings in Map:

1.  Click the **Mapping Approval** tab on the Quick Panel.

2.  Click **Edit** for a mapping that should be rejected.

3.  Enter the reason for the rejection in the **Comment** field.
    
    **NOTE:** If the action for the mapping is Rule or RuleXref, the
    Developer must also enter the SQL code for the rule in the Rule SQL
    field. The Rule SQL field only displays when the action for the
    selected mapping is Rule or RuleXref.

4.  Click **Save**.

5.  Select multiple mappings to reject once comments have been added to
    each mapping.
    
    **NOTE:** To select a contiguous range of items, hold down the
    **Shift** key and select the first and last items in the range. To
    select a non-contiguous range of items, hold down the **Ctrl** key
    and select each item.

6.  Click **Reject**.
    
    **NOTE**: If the *Field Mappings* page is open in Map when multiple
    mappings are rejected, refresh the *Field Mappings* page manually to
    see the update.

Refer to [Reject the Mapping](#Reject_the_Mapping) for more information
about the mapping process when mappings are rejected.
