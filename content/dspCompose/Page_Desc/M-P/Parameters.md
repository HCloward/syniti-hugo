+++
title = 'Parameters'
solution = 'Data Quality'
+++

# Parameters

<div class="use">

Use this page to [Configure dspCompose™
parameters](../Config/Configure_dspCompose_Parameters.htm).

</div>

This page has the following tabs:

  - [General tab](#General_Tab)
  - [Template tab](#Template_Tab)
  - [Posting And File tab](#Posting_And_File_Tab)
  - [Naming Conventions tab](#Naming_Conventions)

### <span id="General_Tab"></span>General tab

Use this tab to [Set up Workflow
Messages](../Config/Set_up_Workflow_Messages.htm)

To access this page, select **dspCompose \>Configuration \>
Parameters** in the *Navigation* pane.

Field

Description

Application Information

Version

Displays current version of dspCompose™.

Date

Displays date when this version of dspCompose™ was released.

Application Settings

Add Roles On Template Creation

If enabled, all roles and dependencies defined on the *Roles* page
(Configuration \> Roles) are automatically registered to a new template.
Default value is Enabled.

Integrate Category

Displays the category in Integrate where BDC and GUI scripts are stored.
 A category is automatically created in Integrate to serve as a
repository for templates created in dspCompose™.  Auto-created processes
are assigned to this category as well. The default value is dspCompose.

File Import Batch Size

Displays the batch size used when importing data from an Excel file into
a request. Default value is 10000.

Use UserID In Workflow

If enabled, user’s User ID is used in the From line in workflow emails,
making the workflow semi-anonymous. If disabled, the user’s email
address is used in the From line in workflow emails. Default value is
Disabled.

### <span id="Template_Tab"></span>Template tab

Use this tab to:

  - [Enable Role Validations](../Config/Enable_Role_Validations.htm)
  - [Update Validation
    Messages](../Config/Update_Validation_Messages.htm)
  - [Set Force Reject
    Severity](../Use_Cases/Set_Force_Reject_Severity.htm)
  - [Set Org Unit Assignment Security for a
    Request](../Use_Cases/Request_Org_Unit_Assignments.htm#Set_Org_Unit_Assignment_Security_for_a_Request)

Field

Description

New Template Defaults

Allow Partial Approval

If enabled, new templates are created with Allow Partial Approval
enabled. This setting allows the Review role to reject or approve
request data by row, allowing different users assigned to the Review
role to be responsible for reviewing specific data. A new request is
created for all rejected roles. This value can be overwritten at the
template level. Default value is Disabled.

Use Comparison Approval Page

If enabled, new templates are created with Use Comparison Approval Page
enabled. This setting allows Review roles to use an enhanced Approval
page to view original data along with any changes to the data entered on
the Data Entry page. The Review role can select to approve or reject
each change. This enhanced page is also used to display posting archives
for requests. This value can be overwritten at the template level.

Only advanced users, comfortable with modifying SQL and familiar with
table names and fields referenced in the request data, should configure
comparison approvals. Default value is Disabled.

Enable List Box Validation

If enabled, dspCompose™ validates the values entered on the data entry
pages of the request that have a list or combo box.  dspCompose™ ensures
that the values that have been entered or selected on the data entry
pages are contained in the list boxes assigned to the data entry pages.
Records that fail this validation fail with a severity of Error. This
setting is used as a default when creating new templates and can be
overwritten at the template level. Default value is Enabled.

Enable Required Validation

If enabled, dspCompose™ validates that all required fields of data type
nvarchar on data entry pages of the request contain values. Records with
blank required fields fail with a severity of Error. dspCompose™ runs
the validation when the user clicks the Validate button on the *[Request
(Roles)](Request_Roles_H.htm)* page. This setting is used as a default
when creating new templates and can be overwritten at the template
level. Default value is Enabled.

**NOTE:** Validations are not run on required fields with data types
other than nvarchar.

Enable Check Box Validation

If enabled, dspCompose™ validates that the values selected on data entry
pages of the request for a check box are the values in the table
corresponding to the proper check box format set on the column property.
Records that fail this validation fail with a severity of Error.
dspCompose™ runs the validation when the user clicks the Validate button
on the Request (Roles) page. This setting is used as a default when
creating new templates and can be overwritten at the template level.
Default value is Enabled.

Force Reject Severity

If enabled, dspCompose™ rejects data entry records that fail a
validation whose severity meets or is more severe than the Force Reject
Severity. These records cannot be approved by the Review role and are
automatically rejected and sent back to the Data role for correction. If
no Force Reject Severity is set, all data entry records can be rejected
or approved by Review role users. This setting is used as a default when
creating new templates and can be overwritten at the template level. The
default value is Blank.

Org Unit Security Level

Displays a value that represents actions that may be performed on Org
Unit Values when a request is created. Values are:

  - **OrgUnit Values Available For Assignment** – All of the individual
    Org Unit values possible for the request are available for
    assignment to the request, but no assignments are assigned by
    default.
  - **User Assignments Defaulted, Change Allowed** – All of the
    individual Org Unit assignments available are assigned to the
    request by default, but may be unassigned.
  - **User Assignments Defaulted, No Change Allowed** – All of the
    individual Org Unit assignments available are assigned to the
    request and cannot be unassigned. If this option is selected, the
    Select All, Unselect All, and Reset Defaults button do not display
    on the *Request (Org Unit Assignments)* page.

This value may be overwritten at the template level. The default value
is User Assignments Defaulted, Change Allowed.

Only Show Org Unit Values Assigned to Requester

If enabled, Org Unit values presented at the request level are based on
the requestor’s Org Unit assignments. If disabled, Org Unit values
presented at the request level are based on all users’ Org Unit
assignments from users assigned to the template. The value set at the
Parameter level becomes the default value for new templates.

System Validation Messages

List Box Validation Message

Displays message that displays on the Request (Role Validations) page
when an invalid value in a list box is selected, the user attempts to
save the record and the list box validation fails. The field accepts
\#Column\# as dynamic substitution for replacement at run time. Default
value is \#Column\# was not in the list of valid values.

List Box Where Clause Validation Message

Displays message that displays on the Request (Role Validations)pagewhen
an invalid value in a list box based on Where clause criteria is
selected, the user attempts to save the record and the list box
validation fails. The field accepts \#Column\# as dynamic substitution
for replacement at run time. Default value is
**\[\#Column\#\] was not in the list of valid values based on dependent criteria**.

Required Validation Message

Displays message that displays on the Request (Role Validations)page
when a user attempts to save data and has left a required field blank.
The field accepts \#Column\# as dynamic substitution for replacement at
run time. Default value is**\#Column\# cannot be empty.**

Check Box Validation Message

Displays message that displays on the Request (Role Validations)page
when a user attempts to save data and a check box, either enabled or
disabled, causes an error. Default value is
**\#Column\# has an invalid CheckBox value.**

### <span id="Posting_And_File_Tab"></span>Posting And File tab

Use this tab to [Display Posting Options on
Requests](../Config/Display_Posting_Options_on_Requests.htm).

Field

Description

Post Page Display

Foreground Post

If enabled, the Post role is allowed to select this option on the
<span style="font-style: italic;">[Request
(Post)](Request_Post.htm)</span> page to immediately post request data
to a target ERP system in the foreground.

If disabled, this option does not display and is not available to the
Post role when submitting a request.

The default value is enabled.

**NOTE:** This option is not available if a request is based on a GUI
Script template.

The user credentials used to post data can be acquired using the methods
outlined in [Establish a Connection to a Target
System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm).

A post that runs in the foreground is used for requests that do not time
out the system based on the number of records to process.

Background Post

If enabled, the Post role is allowed to select this option on
the<span style="font-style: italic;">[Request
(Post)](Request_Post.htm)</span><span> page</span> to post request data
to a target ERP system in the background.

If disabled, this option does not display and is not available to the
Post role when posting a request. The default value is enabled.

The user credentials used to post data can be acquired using the methods
outlined in [Establish a Connection to a Target
System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm).

A request is posted in the background if there is a large amount of data
to process that may affect system performance or may time out a session.
Monitor posts that run in the background on the
[<span style="font-style: italic;">Request Role Finish
Monito</span>r](Request_Role_Finish_Monitor.htm) page.

Schedule Post

If enabled, the Post role is allowed to select this option on the
<span style="font-style: italic;">[Request
(Post)](Request_Post.htm)</span><span> page </span>to post a request at
a configurable later date and time.

If disabled, this option does not display and is not available to the
Post role when posting a request. The default value is enabled.

The user credentials used to post data can be acquired using the methods
outlined in [Establish a Connection to a Target
System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm).

Refer to [Setting the Post Start
Time](../Use_Cases/Setting_the_Post_Start_Time.htm) for more
information.

Posting Settings

Background Posting Queue ID

Displays the queue used by the background posting functionality in
dspCompose™. The default value is Blank.

Chunk Size

Displays the number of records that are processed at once when posting
data to a target ERP system. The default value is **1000**.

Posting Archive Retention Interval

Displays the number of days posting archives are retained until purged.
With the ability to purge posting archives, space in the database can be
saved and unnecessary clutter is removed from the data. If the value is
set to 0, the posting archives are never purged. The default value is
**5**.

File Settings

File Location

Displays the location of Excel spreadsheets created by dspCompose™ and
used by External Data roles to submit request data. The default location
is /Files/.

File Retention Interval

Displays the number of days the generated Excel spreadsheets containing
request data are retained on the server until purged. With the ability
to purge files, the web server does not contain unnecessary clutter.
Also, the cleanup minimizes the impact dspCompose™ has on the server.
Default value is **5**.

Protect Excel Sheets

If enabled, the Excel file that is sent to users for review via workflow
is protected.

Required Field Background

Displays the background color for required fields in the data entry
Excel file. A user generates this file at the Request role level. If a
field is required, the column’s cells display in this color.

**NOTE:** This setting can be overridden on the
<span style="font-style: italic;">Template (Role Excel Column
Control)</span> page (Team \> Templates \> Roles \> Excel Column Control
\> Required Columns Format).

Required Field

Displays the text color for required fields in the data entry Excel
file. A user generates this file at the Request role level. If a field
is required, the text in the column’s cells display in this color.

**NOTE:** This setting can be overridden on the
<span style="font-style: italic;">Template (Role</span>

**NOTE:** <span style="font-style: italic;"> Excel Column
Control)</span> page (Team \> Templates \> Roles \> Excel Column Control
\> Required Columns Format).

### <span id="Naming_Conventions"></span>Naming Conventions

Use this page to [Add a Data Source that Stores Views for
Import](../Use_Cases/Add_a_Data_Source_that_Stores_Views_for_Import.htm).

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Import View Filter</p></td>
<td><p>Displays the format of the view name that must be used when creating a view to import into dspCompose™. If the view name does not follow this format, the view name does not display in the View list box on the <span style="font-style: italic;">Vertical</span> View of the <span style="font-style: italic;">Request (Roles)</span> page (Requests &gt; Roles), and the view cannot be imported.  </p>
<p>Refer to <a href="../Use_Cases/Import_a_View_at_the_Request%20Role_Level.htm">Import a View at the Request-Role Level</a> for more information.  </p></td>
</tr>
</tbody>
</table>
