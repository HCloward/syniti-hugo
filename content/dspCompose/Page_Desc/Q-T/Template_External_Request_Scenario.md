+++
title = 'Template (External Request Scenario) H'
solution = 'Data Quality'
+++

# Template (External Request Scenario) H

[Template (External Request Scenario)
 V](Template_External_Request_Scenario.htm#Template__External_Request_Scenario__V)

<div class="use">

Use this page to:

  - [Create an External Request
    Scenario](../Use_Cases/Create_an_External_Request_Scenario.htm)
  - [Create an External Request Scenario for an Excel-initiated
    Request](../Use_Cases/Create_an_External_Request_Scenario_for_an_Excel_Initiated_Requestel.htm)

</div>

<span style="color: #000000;">To access this page:</span>

1.  Click <span style="font-weight: bold;">dspCompose \>
    Team</span> on the *Navigation *pane.
2.  Click <span style="font-weight: bold;">Templates</span> for a team.
3.  Click the <span style="font-weight: bold;">Vertical View</span> icon
    for a template.
4.  Click the<span style="font-weight: bold;"> Configuration</span> tab.
5.  Click the <span style="font-weight: bold;">External Request
    Scenarios</span> icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>SUBJECT ALIAS</p></td>
<td><p>Displays subject line of the external email received by dspCompose™. dspCompose™ uses this external request scenario for the template to create a request. The alias is a unique name typically related to the name of the template.</p></td>
</tr>
<tr class="odd">
<td><p>SCENARIO DESCRIPTION</p></td>
<td><p>Displays name or brief description of the scenario.</p></td>
</tr>
<tr class="even">
<td><p>REQUEST DESCRIPTION FORMAT</p></td>
<td><p>Displays description used for a request created from this External Request Scenario. This format is used as the request’s description on the <em>Request</em> page. The field defaults to Request from #RequesterEmailAddress# - #Date#  where the RequesterEmailAddress is the address of the user who submitted the email to create the request, and the Date is the date that the email was received at the External Data Email Account.</p></td>
</tr>
<tr class="odd">
<td><p>EXCEL ALLOWED</p></td>
<td><p>If enabled, this external request scenario is configured to create a request and accept an Excel file attached to an email from a designated contact. The Excel file provides data for the first Data Entry role in the workflow. In this case, not only will the request be created, but the worksheet data from the Excel file will be inserted into the table used by the first Data Entry role (after certain conditions are met).</p>
<p><span style="font-weight: bold;">NOTE:</span> This check box cannot be disabled if:</p>
<ul>
<li><p>The template has been activated, even if the template is in Developer mode</p></li>
<li><p>The template has not yet been activated, but an Excel file has been added to the external request scenario.</p></li>
</ul>
<p>The check box can be disabled if the template has not yet been activated, and an Excel file has been added to the external request scenario, but the user clears data from all fields on the <span style="font-style: italic;">Template (External Request Scenario</span>) page's <span style="font-style: italic;">Vertical</span> View on the Advanced tab.</p></td>
</tr>
<tr class="even">
<td><p>Email Addresses</p></td>
<td><p>Click to open the <em>Template (External Request Scenario Email Address)</em> page to add, edit and delete email addresses that can send an email to create a request in dspCompose™ for the scenario.</p></td>
</tr>
<tr class="odd">
<td><p>External Roles</p></td>
<td><p>Click to open the <em><a href="Template_External_Request_Sceanario_External_Role.htm">Template (External Request Scenario External Role)</a></em> page to add and edit external roles assigned to the external scenario.</p>
<p>This icon only displays if:</p>
<ul>
<li>External Data roles are assigned to the template and</li>
<li>EXCEL ALLOWED is not enabled for the particular External Request Scenario.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Connections</p></td>
<td><p>Click to open the <em><a href="Template_External_Request_Scenarios_Connections.htm">Template (External Request Scenarios Connections)</a></em> page to set a connection to a target system for each process template used in the scenario.</p>
<p>Refer to <a href="../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm">Establish a Connection to a Target System</a> for more information.</p>
<p><strong>NOTE:</strong> If a user adds a request based on this template and does not select a connection ID, the default connection assigned to the Integrate Template is used for the request.</p></td>
</tr>
</tbody>
</table>

## <span id="Template__External_Request_Scenario__V"></span>Template (External Request Scenario) V

[Template (External Request Scenario)
H](Template_External_Request_Scenario.htm)

This page has the following tabs:

  - [General](#General_Tab)
  - [Advanced](#Advanced_tab)

## <span id="General_Tab"></span>General tab

<div class="use">

Use this tab to:

  - [Create an External Request
    Scenario](../Use_Cases/Create_an_External_Request_Scenario.htm)
  - [Create an External Request Scenario for an Excel-initiated
    Request](../Use_Cases/Create_an_External_Request_Scenario_for_an_Excel_Initiated_Requestel.htm)

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Subject Alias</p></td>
<td><p>Displays the subject line of the external email received by dspCompose™. When dspCompose™ receives an external email, if the subject line of the email contains this text, dspCompose™ uses this external request scenario for the template to create a request.</p>
<p><strong>NOTE:</strong> If dspCompose™ receives an email without a valid Subject Alias, the email fails a validation and processing stops. dspCompose™ sends the email back to the original sender for correction.</p></td>
</tr>
<tr class="odd">
<td><p>Scenario Description</p></td>
<td><p>Displays the name or brief description of the scenario. Use this field to identify the scenario, and, if the template has multiple scenarios, to distinguish it from others attached to the template.</p></td>
</tr>
<tr class="even">
<td><p>Request Description Format</p></td>
<td><p>Displays the description used for a request created from this external request scenario. This format is used as the request’s description on the <em>Request</em> page. The field defaults to Request from #RequesterEmailAddress# - #Date# where the RequesterEmailAddress is the address of the user who submitted the email to create the request, and the Date is the date that the email was received at the External Data Email Account.</p></td>
</tr>
<tr class="odd">
<td><p>Connections</p></td>
<td><p>Click to open the <em><a href="Template_External_Request_Scenarios_Connections.htm">Template (External Request Scenarios Connections)</a></em> page to set a connection to a target system for each process template used in the scenario.</p></td>
</tr>
<tr class="even">
<td><p>Email Addresses</p></td>
<td><p>Click to open the <em>Template (External Request Scenario Email Address)</em> page to add, edit and delete email addresses that can send an email to create a request in dspCompose™ for the scenario. Refer to <a href="../Use_Cases/Add_Email_Addresses_for_a_Scenario.htm">Add Email Addresses for a Scenario</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>External Roles</p></td>
<td><p>Click to open the <em><a href="Template_External_Request_Sceanario_External_Role.htm">Template (External Request Scenario External Role)</a></em> page to add and edit external roles assigned to the external scenario.</p>
<p>This icon only displays if:</p>
<ul>
<li>External Data roles are assigned to the template and</li>
<li>EXCEL ALLOWED is not enabled for the particular External Request Scenario.</li>
</ul>
<p>Refer to <a href="../Use_Cases/Use_External_Data_Roles_in_Request_Processing.htm">Use External Data Roles in Request Processing</a> for more information.</p></td>
</tr>
</tbody>
</table>

 

## <span id="Advanced_tab"></span>Advanced tab

<div class="use">

Use this tab to:[Create an External Request Scenario for an
Excel-initiated
Request](../Use_Cases/Create_an_External_Request_Scenario_for_an_Excel_Initiated_Requestel.htm).

</div>

Field

Description

Excel Definition

Excel Allowed

If enabled, this external request scenario is configured to create a
request and accept an Excel file attached to an email from a designated
contact. The Excel file provides data for the first Data Entry role in
the workflow. In this case, not only will the request be created, but
the worksheet data from the Excel file will be inserted into the table
used by the first Data Entry role (after certain conditions are met).

This check box cannot be disabled if:

  - The template has been activated, even if the template is in
    Developer mode
  - The template has not yet been activated, but an Excel file has been
    added to the external request scenario.

The check box can be disabled if the template has not yet been
activated, an Excel file has been added to the external request
scenario, but the user clears data from all fields on the
<span style="font-style: italic;">[Template (External Request
Scenario)](#)</span> page's
<span style="font-style: italic;">Vertical</span> View on the Advanced
tab.

Finish First Role

If enabled, the Data Entry role with the lowest priority is to be
finished once the data from the spreadsheet has passed validations and
been written to the Data Entry table.

In this case, the request moves to the next role in the workflow, either
the next Data role or a Review role, and a user assigned to this next
role receives a workflow message that the role is ready. The FINISHED BY
column on the *[Request (Roles)](Request_Roles_H.htm)* page displays the
email of the user who submitted the Excel file. The FINISHED ON column
displays the date the email was received.

If the Finish First Role check box is disabled, the Data Entry role with
the lowest priority receives a workflow message that the role is ready
after the data from the Excel file has passed validations and been
written to the Data Entry table.

Sheet Name

Displays the name of the worksheet in the sample Excel file. A version
of this worksheet with Request-ready data will be mailed to the external
data email account to create requests for this template.

**NOTE:** This name is case sensitive.

Staging Data Source ID

Displays the name of the data source where the staging table will be
created and stored.The dspCompose\_Data data source is the recommended
selection.

Staging Table Name

Displays the name of the table that will be used to import Excel
attachment spreadsheet data.

The name can be automatically generated by dspCompose™ in the format
st\[Template name\]\[Subject Alias\]ExcelStaging when the Sample Sheet
is uploaded.

Upload Sample Sheet

Click to upload the sample Excel file.

The file must be in a specified format.

  - The first row contains the column names of the table that will be
    created for the lowest priority Data Entry role for the request.
  - The second row is ignored, and could contain column descriptions to
    assist users when entering data.
  - The third row is the first data record imported into the staging
    table.

**NOTE:** The only files that can be uploaded are Excel files (with an
.xls or .xlsx extension).

Build Staging Area

Click to create the staging table in the data source identified in the
Staging Data Source ID field with the name in the Staging Table Name
field.

Map Sheet Columns

Click to open the [*Template (External Request Scenario
Column)*](Template_External_Request_Scenario_Column.htm) page to map
columns from the sample sheet to columns in the template.

**NOTE:** The Map Sheet Columns icon is only active once the following
two criteria are met:

  - An Excel file has been successfully processed for this scenario.
    Refer to [Create an External Request Scenario for an Excel-initiated
    Request](../Use_Cases/Create_an_External_Request_Scenario_for_an_Excel_Initiated_Requestel.htm)
    for more information.
  - The Template has been generated.  Generate a template on the
    *[Templates](Templates_H.htm)* page’s *Vertical* View on the General
    tab.

**NOTE:** The count on this icon represents the number of columns that
have been mapped from the Excel file to the staging table.

Refer to [Map Columns from the Template to Columns from the Excel
File](../../../Migration/Map/Use_Cases/Map_Columns_Template_to_Sprdsht.htm)for
more information.

External Request Create Rules

Click to open the [Template (Event Rule)](Template_Event_Rule.htm) page
to add, edit and delete rules. Refer to [Create Custom Rules for
Excel-initiated
Requests](../Use_Cases/Create_Custom_Rules_for_Excel_Initiated_Requests.htm)
for more information.

**NOTE:** The count on this icon represents the number of rules that
have been added to the external request scenario. These rules run on
data in the staging table before it is moved to the data entry table.

Clear Staging Area

Click to clear the staging area, allowing the staging table to be
rebuilt if the sample sheet must be uploaded after the initial upload.
