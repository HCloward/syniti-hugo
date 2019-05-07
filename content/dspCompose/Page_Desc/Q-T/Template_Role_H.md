+++
title = 'Template (Role) H'
solution = 'Data Quality'
+++

# Template (Role) H

[Template (Role) V](#Template_Role_V_All_Tabs)

<div class="use">

Use this page to

  - [Create Template Roles](../Use_Cases/Create_Template_Roles.htm)
  - [Assign Default Data Source and
    Views](../Use_Cases/Assign_Default_Data_Source_and_Views.htm)
  - [Add an External Data Role Type to a
    Template](../Use_Cases/Add_an_External_Data_Role_to_Template.htm)

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspCompose \>
    Team</span> on *Navigation *pane.
2.  Click <span style="font-weight: bold;">Templates</span> for a team.
3.  Click <span style="font-weight: bold;">Roles</span> for a template.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays order in which the role is processed in a request that uses the template.</p></td>
</tr>
<tr class="odd">
<td><p>ROLE ID</p></td>
<td><p>Displays name of the role assigned to the template.</p></td>
</tr>
<tr class="even">
<td><p>Validations</p></td>
<td><p>Click to open the <em><a href="Template_Role_Validations_H.htm">Template (Role Validations)</a></em> page to activate, deactivate, add, edit and delete validations for the role.</p></td>
</tr>
<tr class="odd">
<td><p>Columns</p></td>
<td><p>Click to open the <em><a href="Template_Role_Column.htm">Template (Role Column)</a></em> page to enable, disable or hide columns for the template. This icon is only available for the Data and Review role once the recording has been generated.</p></td>
</tr>
<tr class="even">
<td><p>Excel Column Control</p></td>
<td><p>Click to open the <em><a href="Template_Role_Excel_Column_Control_H.htm">Template (Role Excel Column Control)</a></em> page to add, edit or delete columns on the Excel spreadsheet generated for data entry, to determine whether a column is read only, and to determine what type of control is used to enter data, such as a text box. This icon is only available for Data and Review roles once the recording has been generated.</p></td>
</tr>
<tr class="odd">
<td><p>Events</p></td>
<td><p>Click to open the <em><a href="Template_Role_Event.htm">Template (Role Event)</a></em> page to configure events that will trigger rules to run for the template role.</p></td>
</tr>
<tr class="even">
<td><p>Dependencies</p></td>
<td><p>Click to open the <a href="Template_Role_Dependency_Select.htm">Template (Role Dependency Select)</a> page to select dependent roles for the template. Dependencies determine what role can not be processed until the current rule has been finished.</p></td>
</tr>
<tr class="odd">
<td><p>Contacts</p></td>
<td><p>Click to open the <em><a href="Template_Role_Validation_Threshold_Contact.htm">Template (Role Validation Threshold Contact)</a></em> page to add, edit and delete users who are notified when the validation threshold is exceeded.</p>
<p>A Template Administrator can set a validation threshold to monitor when a user, including an External Data role user, is unable to pass a role.</p>
<p>When a user clicks the Validate button on the Request (Roles) page for a role, and at least one record in a validation fails, dspCompose™ logs the failure and keeps a count of failed records. When this count exceeds the validation threshold, dspCompose™ sends the validation contacts an email.</p>
<p>If the role finishes successfully, dspCompose™ resets the validation count.</p>
<p>The validation threshold is set on the <em><a href="#">Template (Role)</a></em> page’s Vertical View on the Approve and Finish Settings tab.</p></td>
</tr>
<tr class="even">
<td><p>Finish Tables</p></td>
<td><p>Click to open the <a href="Template_Role_Finish.htm">Template Role (Finish)</a> page to add, edit or delete Collect rules to run on table data after the download is finished, and to specify filter columns for both source and target data. This icon is only available for Post roles.</p></td>
</tr>
</tbody>
</table>

## <span id="Template_Role_V_All_Tabs"></span>Template (Role) V (All Tabs)

[Template (Role) H](Template_Role_H.htm)

This page contains the following tabs:

  - [General tab](#General_Tab3)
  - [Import Settings tab](#Import_Settings_Tab)
  - [Approve And Finish Settings tab](#Approve_And_Finish)
  - [Page Settings tab](#Page_Settings_Tab)
  - [Advanced Settings tab](#Advanced_Settings_Tab)

## <span id="General_Tab3"></span>General tab

<div class="use">

Use this tab to [Link a Template to a
Page](../Use_Cases/Link_a_Template_to_a_Page.htm).

</div>

Field

Description

Settings

Role ID

Displays name of the role.

Basic

Priority

Displays order in which the role is processed on the request that uses
this template.

Description

Displays brief description about the role.

Role Type

Displays type assigned to role, which defines how the role data within
the request is manipulated.

Values are:

  - **Data** – Enter request data by manually entering or editing data,
    performing a mass change, or importing data.
  - **Review** – Review the data entered by the Data role, and approve
    or reject the data.
  - **Post** – Post the approved data to SAP.
  - **External Data** – Receive a spreadsheet generated by dspCompse™,
    enter request data, and email the spreadsheet to dspCompose™. This
    data, once it passes validations, becomes the basis for a request. 

Configuration

Validations

Click to open the *[Template (Role
Validations)](Template_Role_Validations_H.htm)* page to add, edit and
delete validation rules for the role.

Columns

Click to open the *[Template (Role Column)](Template_Role_Column.htm)*
page to enable, disable or hide columns for the template. This icon is
only available once the recording has been generated.

Events

Click to open the *[Template (Role Event)](Template_Role_Event.htm)*
page to configure events that will trigger rules to run for the template
role.

Dependencies

Click to open the *[Template (Role Dependency
Select)](Template_Role_Dependency_Select.htm)* page to select dependent
roles for the template. Dependencies determine what role can not be
processed until the current rule has been finished.

## <span id="Import_Settings_Tab"></span>Import Settings tab

<div class="use">

Use this tab to [Assign Default Data Source and Views for a
Template](../Use_Cases/Assign_Default_Data_Source_and_Views.htm)

</div>

Field

Description

Excel

Excel Import Allowed

If enabled, Excel files are able to be imported into the request in
order to upload data into dspCompose™.

Excel Column Control

Click to open the *[Template (Role Excel Column
Control)](Template_Role_Excel_Column_Control_H.htm)* page to add, edit
or delete columns on the Excel spreadsheetgenerated for data entry, to
set whether a column is read only, and to set what type of control is
used to enter data, such as a text box. This icon is only available once
the recording has been generated for Data and Review roles.

View

View Import Allowed

If enabled, a request’s data entry page can be created by importing a
view for any request based on the template.

This field only displays for the Data role.

**NOTE:** At least one data source that stores a view must be set on the
View Import Data Sources page.

The view name must follow naming conventions.

Refer to [Import a View at the Request-Role
Level](../Use_Cases/Import_a_View_at_the_Request%20Role_Level.htm) for
more information.

View Import Data Sources

Click to open the *[View Import Data
Sources](../Use_Cases/View_Import_Data_Sources.htm)* page to add or
remove data sources that store views that can be imported to create a
request based on the template.

**NOTE:** The count on this icon represents the number of data sources
assigned to the role.

**NOTE:** This field only displays for the Data role.

Refer to [Import a View at the Request-Role
Level](../Use_Cases/Import_a_View_at_the_Request%20Role_Level.htm) for
more information.

View Import Data Source ID Default

Displays data source used as the default value when using a view to
import data for requests using this template. This field only displays
for Data roles.

View Import View Name Default

Displays view used as the default value to import data for requests
using this template. This field only displays for Data roles.

## <span id="Approve_And_Finish"></span>Approve And Finish Settings tab

<div class="use">

Use this tab to:

  - [Set Target Role for Request Rejections from a Review
    Role](../Use_Cases/Set_Target_Role_for_Request_Rejections.htm)
  - [Set Validation
    Threshold](../Use_Cases/Set_Validation_Threshold.htm)
  - [Configure the Comparison Approval
    Setting](../Use_Cases/Configure_the_Comparison_Approval_Setting.htm)

</div>

Field

Description

Approve

Use Comparison Approval Page

If enabled, the users assigned to the Review role can use an enhanced
Approval page to view original data along with any changes to the data
entered on the Data Entry page. The Review role can select to approve or
reject each change. Only advanced users, comfortable with modifying SQL
and familiar with table names and fields referenced in the request data,
should configure comparison approvals. This field only displays for
Review roles.

Allow Partial Approval

If enabled, the Review role is able to reject or approve request data by
row, allowing different users assigned to the Review role to be
responsible for reviewing specific data. A new request is created for
all rejected roles. The default value is configured on the Parameters
page. This field only displays for Review roles.

Finish

Force Validate Before Finish

If enabled, validation rules are required to be completed without any
errors before a role can be finished. This field only displays for Data
Entry and Review roles.

Prevent Finish Severity

Displays severity level for validation failure. Role is unable to be
finished if the failed validation matches or is more severe than the
severity level.

Values are:

  - **Error** – Marks the status as invalid until the error is corrected
    and the Validation Rule passes.
  - **Message** – Marks the status as valid but a message displays.
  - **Warning** – Displays a message but the user can proceed with the
    task even if the validation  fails.

This field only displays for Data Entry and Review roles.

Reject

Reject Role Target

Displays the role on the request that becomes available when the Reject
button is clicked for the Review role. If blank, the request is sent
back to the lowest priority role. This setting allows for greater
workflow customization. dspCompose™ assigns the rejected request records
to the target role. This field only displays for Review roles.

Partial Approval Reject Request Role Target

Displays the role that will be assigned to a new request if:

  - dspCompose™ has been configured to allow partial approvals of
    requests
  - A Review role rejects some of the records in a request

If the field is blank, dspCompose™ assigns the request to the lowest
priority role in the request. This field only displays for Review roles.

Validation Failure Notification

Validation Threshold

Displays threshold value used to monitor when a user, including an
external role user, is unable to finish a role. When the Validate button
is clicked on theRequest (Roles)page for a role, and at least one record
in a validation fails, dspCompose™ logs the failure and keeps a count of
the failed records. When this count exceeds the validation threshold,
dspCompose™ sends the validation contacts an email. If the role finishes
successfully, dspCompose™ resets the validation count. If the validation
threshold is blank or is set to 0, dspCompose™ never sends an email to
the validation contacts. This field only displays for External, Data and
Review roles.

Contacts

Click to open the *[Template (Role Validation Threshold
Contact)](Template_Role_Validation_Threshold_Contact.htm)* page to add
and delete users who are notified when the validation threshold is
exceeded.

Download

Finish Tables

Click to open the [Template Role (Finish)](Template_Role_Finish.htm)
page to set Collect rules to run on table data after the download is
finished, and to specify filter columns for both source and target data.
This icon is only available for Post roles.

Finish Download In Background

If enabled, data downloads in the background after the user assigned to
the Post role clicks the Finish button on theRequest (Roles)page. This
field is only available for Post roles.

## <span id="Page_Settings_Tab"></span>Page Settings tab

<div class="use">

Use this tab to:

  - [Link a Template to a
    Page](../Use_Cases/Link_a_Template_to_a_Page.htm)
  - [Assign a Custom Page to a Template
    Role](../Use_Cases/Assign_a_Custom_Page_to_Template_Role.htm)
  - [Add Custom Roles for the Looped
    Template](../Use_Cases/Add_Custom_Roles_for_the_Looped_Template.htm)

</div>

Field

Description

Custom

Custom Page

If enabled, the Page label set displays with additional fields to
populate, allowing any page within the DSP® to be assigned to a template
role. A user assigned to the role navigates to this custom page by
clicking the Data Entry button on the Request (Roles) page.

Page

Web App ID

Displays name of WebApp that contains the custom page. This field only
displays if Custom Page is enabled.

Page ID

Displays name of the custom page. This field only displays if Custom
Page is enabled.

## <span id="Advanced_Settings_Tab"></span>Advanced Settings tab

This tab only displays for Data and Review roles.

Field

Description

Advanced

Excel Export Where Clause Override

Displays the WHERE clause used to override the system-generated WHERE
clause that is used to determine which records for the request are
selected when exporting data into Excel files.
<span style="font-family: Arial, sans-serif;font-style: normal;">This
field only displays for Data and Review roles.</span>
