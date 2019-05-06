# Mapping Status and Rule Status

## <span id="How_Statuses_Change_During_the_Mapping_Approvals_Process"></span>How Statuses Change During the Mapping Approvals Process

As a mapping passes through the Mapping Approval process, the system
updates the Mapping Status and Rule Status.

1.  The Mapping Status and Rule Status are set to
    <span style="font-weight: bold;">Pending Review</span> by default
    when Target Design and Map are synced.
2.  After the Mapper sets the mapping’s action, configures the
    appropriate settings, and clicks Save, if the mapping passes all
    validations, the system sets the Mapping Status to
    <span style="font-weight: bold;">In Progress</span>. The Rule Status
    remains in <span style="font-weight: bold;">Pending Review</span>.
3.  After a Business User clicks the Submit or Submit All icon on the
    <span style="font-style: italic;">[Field
    Mappings](../Page_Desc/Field_Mappings_H.htm)</span> page, the system
    sets the Mapping Status to
    <span style="font-weight: bold;">Complete</span>. The Rule Status
    remains in <span style="font-weight: bold;">Pending Review</span>.
4.  After a Developer reviews and approves a mapping on the
    <span style="font-style: italic;">[Mapping
    Approval](../Page_Desc/Mapping_Approval_H.htm)</span> page the
    system updates the Rule Status field to
    <span style="font-weight: bold;">In Progress</span>. This indicates
    the Developer can begin development on the rule.
5.  After a mapping is created (when the user clicks Create and Complete
    on the <span style="font-style: italic;">[Automation SQL Field
    Mappings](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H.htm)</span>
    page or the Create All Rules icon on the
    <span style="font-style: italic;">[Automation](../../SQL_AutoGen/Page_Desc/Automation_page.htm)</span>
    page)  the system updates the Rule Status to Complete.

<span style="font-weight: bold;">NOTE</span>: For the Developer to
create the rule in SQL AutoGen, the Mapping Status must be set to
Complete.

Refer to [Approve or Reject Mappings](Approve_or_Reject_Mappings.htm)
for more information.

## Mapping Status Values

Mapping Status values are:

  - <span style="font-weight: bold;">Pending Review</span> – The default
    value indicates that a mapping has been either:
      - Synced with Target Design but work on the mapping has not begun.
      - Synced with Target Design, has been worked on, but the saved
        changes did not pass validations.
      - Reset by a mapper or a Developer. Mappings can be reset in
        AutoGen on the <span style="font-style: italic;">[Automation SQL
        Field
        Mappings](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H.htm)</span>
        page, on the <span style="font-style: italic;">[Field
        Mappings](../Page_Desc/Field_Mappings_H.htm)</span> page, or on
        the <span style="font-style: italic;">[Mapping
        Approval](../Page_Desc/Mapping_Approval_H.htm)</span> page.
  - <span style="font-weight: bold;">Design Required</span> – The
    mapping has been reviewed by a Developer and rejected on the
    <span style="font-style: italic;">[Mapping
    Approval](../Page_Desc/Mapping_Approval_H.htm)</span> page. The
    mapper must update the mapping and submit it again.
  - <span style="font-weight: bold;">Complete</span> – The mapping has
    been submitted when the mapper has finished creating the mapping and
    clicks the Submit or Submit All icons on the
    <span style="font-style: italic;">[Field
    Mappings](../Page_Desc/Field_Mappings_H.htm)</span> page.

## Rule Status Values

Rule Status displays the status of the rule to be built from the
mapping.

Rule Status values are:

  - <span style="font-weight: bold;">Pending Review</span> – The default
    value indicates that a mapping for the rule:
      - Has not yet been submitted.
      - Has been submitted and is waiting for Developer review.
      - Has been reset by a Mapper or a Developer. Mappings can be reset
        in AutoGen on the [Automation SQL Field
        Mappings](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H.htm)
        page and on the <span style="font-style: italic;">[Field
        Mappings](../Page_Desc/Field_Mappings_H.htm)</span> page or on
        the <span style="font-style: italic;">[Mapping
        Approval](../Page_Desc/Mapping_Approval_H.htm)</span> page.
  - <span style="font-weight: bold;">Revision Requested</span> – The
    mapping for this rule has been reviewed by a Developer and rejected
    on the <span style="font-style: italic;">[Mapping
    Approval](../Page_Desc/Mapping_Approval_H.htm)</span> page. The
    mapper must update the mapping and submit it again.
  - <span style="font-weight: bold;">In Progress</span> – The mapping
    has been approved on the <span style="font-style: italic;">[Mapping
    Approval](../Page_Desc/Mapping_Approval_H.htm)</span>page.
  - <span style="font-weight: bold;">Complete</span> – The mapping
    development has been completed. A user clicked the Create and
    Complete icon on the  <span style="font-style: italic;">[Automation
    SQL Field
    Mappings](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H.htm)</span>
    page or the Create All Rules icon on the
    <span style="font-style: italic;">[Automation](../../SQL_AutoGen/Page_Desc/Automation_page.htm)</span>
    page. A Developer clicked Complete on the [Mapping
    Approval](../Page_Desc/Mapping_Approval_H.htm)
page.

## <span id="Configure_Mapping_Status_and_Rule_Status"></span>Configure Mapping Status and Rule Status

There are two types of Mapping Status and Rule Status: Installed and
custom.

A user can change the Mapping Status on the
<span style="font-style: italic;">Vertical</span> View of the
<span style="font-style: italic;">[Field
Mappings](../Page_Desc/Field_Mappings_H.htm)</span> page to an installed
status or a custom status.

### Configure Installed Statuses

Installed statuses are applied during the Mapping Approval process and
indicate where a mapping or rule is in the process. Installed
<span id="Mapping Status" class="popUpLink">Mapping Statuses</span> and
<span id="Rule Status" class="popUpLink">Rule Statuses</span> cannot be
deleted. All attributes can be configured except for the name.

A user cannot update the Rule Status in Map. It is updated by the
system.

The user can update the Rule Status in SQL AutoGen. Refer to [Update a
Rule Status](../../SQL_AutoGen/Use_Cases/Update_a_Rule_Status.htm) for
more information.

### Add Custom Statuses

Custom statuses can be added to track work on mapping and rule creation.
These statuses are applied manually and are not set by the system.
Custom statuses, such as "Impeded," are used for documentation purposes
as an additional status beyond installed statuses for tracking mapping
progress.

A custom status is assigned to mappings between the status of Pending
Review and Complete. It cannot be used to define a mapping status beyond
Complete.

<span style="font-weight: bold;">NOTE</span>: Custom statuses display on
the [Target Source Rule Book](../Page_Desc/Target_Source_Rule_Book.htm),
but do not display on dashboards.

### Add a Custom Mapping Status

To add a custom Mapping Status in Map:

1.  Select <span style="font-weight: bold;">Configuration \> Mapping
    Status</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Mapping Status
    page](../Page_Desc/Mapping_Status_page.htm)

3.  Enter the name of the status in the
    <span style="font-weight: bold;">MAPPING STATUS</span> field.

4.  Enter a brief description of the status in the
    <span style="font-weight: bold;">DESCRIPTION</span> field.

5.  Select an image from the <span style="font-weight: bold;">IMAGE
    NAME</span> list box.
    
    **NOTE:** Images that were installed with the system display. These
    images can be viewed on the
    *[Images](../../../Platform/Sys_Admin/Page_Desc/Images%20H.htm)*
    page (Admin \> Configuration \> Style \> Images). A user can also
    add custom images on this page.

6.  Click the <span style="font-weight: bold;">DEFAULT</span> check box
    to enable it, if applicable.
    
    **NOTE:** The default status is set for a mapping when the mapping
    is saved. The system uses the In Progress status unless another
    status has this setting enabled.

7.  Click the <span style="font-weight: bold;">TRACK HISTORY</span>
    check box to enable it, if applicable.
    
    **NOTE:** If the check box is checked, when a mapping is set to this
    status, it is tracked on the
    <span style="font-style: italic;">[Field Mapping
    History](../Page_Desc/Field_Mapping_History.htm)</span> page.

8.  Click <span style="font-weight: bold;">Save</span>.

This custom Mapping Status displays as an option in the Mapping Status
list box on the <span style="font-style: italic;">[Field
Mappings](../Page_Desc/Field_Mappings_H.htm)</span> page’s
<span style="font-style: italic;">Vertical</span> View.

### Add a Custom Rule Status

To add a custom Rule Status:

1.  Select <span style="font-weight: bold;">Configuration \> Rule
    Status</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Add</span>.
    
    [*View the field descriptions for the Rule Status
    page.*](../Page_Desc/Rule_Status.htm)

3.  Enter the name of the status in the
    <span style="font-weight: bold;">RULE STATUS</span> field.

4.  Enter a brief description of the status in the
    <span style="font-weight: bold;">DESCRIPTION</span> field.

5.  Select an image from the <span style="font-weight: bold;">IMAGE
    NAME</span> list box.
    
    **NOTE:** Images that were installed with the system display. These
    images can be viewed on the
    <span style="font-style: italic;">Images</span> page (Admin \>
    Configuration \> Style \> Images). A user can also add custom images
    on this page.

6.  Click <span style="font-weight: bold;">Save</span>.

This custom Rule Status displays as an option in the RULE STATUS list
box on the [<span style="font-style: italic;">Automation SQL Field
Mappings</span>](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H.htm)
page.
