+++
title = 'Page Business Rules H'
solution = 'Platform'
+++

# Page Business Rules H

[Page Business Rules V](#PageBusinessRulesV)

<div class="use">

Use this page to

  - [Register Workflow
    Views](../../../Migration/Console/Use_Cases/Create_Custom_Workflow_Messages#Register).
  - [Create a Stored Procedure Business
    Rule](../../WebApp_Dev/Create_a_Business_Rule_for_a_Field)
  - [Create an External Page Business
    Rule](../../WebApp_Dev/CreateExternalPageBusinessRule)
  - [Create a WebApp Event Business
    Rule](../../WebApp_Dev/CreateWebAppEventBusinessRule)
  - [Create a WebApp Event (Private) Business
    Rule](../../WebApp_Dev/CreateWebAppEventPrivateBusinessRule)

</div>

To access this page:

1.  Select  **Admin \>WebApps** in the *Navigation* pane.

2.  Click the **Pages** icon for a **WEB APP NAME**.

3.  Click the **Events** icon for a page.

4.  Click the **Business Rules** icon for an event.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the number indicating the order in which the workflows will run. Business Rules that have Force Foreground Execution enabled will run first if the event is set to background.  </p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If checked, the workflow will be run.</p>
<p>If unchecked, the workflow will not be run.</p></td>
</tr>
<tr class="even">
<td><p>PROCEDURE TYPE</p></td>
<td><p>Displays the type of Business rule.</p>
<p>Options are:</p>
<ul>
<li>External Page</li>
<li>Stored Procedure</li>
<li>WebApp Event</li>
<li>WebApp Event (Private)</li>
<li>Workflow</li>
</ul>
<p><strong>NOTE:</strong> Refer to <a href="../../../Migration/Console/Use_Cases/Create_Custom_Workflow_Messages#Register">Register Workflow Views</a> for information about adding Business Rules to a workflow.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays the name of the workflow view.</p></td>
</tr>
<tr class="even">
<td><p>COMMENT</p></td>
<td><p>Displays comments entered by the user.</p></td>
</tr>
<tr class="odd">
<td><p>RUN ON VALIDATE</p></td>
<td><p>If checked and the corresponding Validation rule returns zero records or if it returns records with a severity level less than Error, the Business rule executes.</p></td>
</tr>
<tr class="even">
<td><p>RUN ON VALIDATE FAIL</p></td>
<td><p>If checked and the corresponding Validation rule returns any record that fails with a severity level of Error, the Business rule executes.</p></td>
</tr>
<tr class="odd">
<td><p>FORCE FOREGROUND EXECUTION</p></td>
<td><p>If checked and the workflow is on an event that is set to run in the background, it will execute twice, once in the foreground and later in the background.</p>
<p>The intent of the feature is to ensure that the Business rule runs against the Web Server, even if the event is set to the background. For example, Force Foreground Execution may be required for plugin access to the Http Context.</p></td>
</tr>
</tbody>
</table>

## <span id="PageBusinessRulesV"></span>Page Business Rules V

[Page Business Rules H](#Page_Business_Rules_H_)

<div class="use">

Use this page to [Register Workflow
Views](../../../Migration/Console/Use_Cases/Create_Custom_Workflow_Messages#Register).

</div>

**NOTE:** The fields that display on this page depend on the Procedure
Type selected on the Horizontal View. Procedure types are:

  - [Stored Procedure](#Procedure_Type_of_Stored_Procedure)
  - [Workflow](#Procedure_Type_of_Workflow)
  - [External Page](#Procedure_Type_of_External_Page)
  - [WebApp Event](#Procedure_Type_of_WebApp_Event)
  - [WebApp Event
    (Private)](#_Procedure_Type_of_WebApp_Event_\(Private\))

### <span id="Procedure_Type_of_Stored_Procedure"></span>Procedure Type of Stored Procedure

<div class="use">

Use this page to [Create a Stored Procedure Business
Rule](../../WebApp_Dev/CreateExternalPageBusinessRule).

</div>

**NOTE:** CranSoft attempts to wrap all procedures within a single SQL
transaction. To avoid deadlocks, all pending transactions are committed
before executing an external process. As a result, mixing external
processes and SQL stored procedures can result in errors which cannot be
completely rolled back. To minimize the effect, consider placing all
external processes after SQL stored procedures by giving them a higher
priority.

Field

Description

Business Rule Properties

Procedure

Displays the name of the SQL stored procedure. Click the link on the
name to open the *Definition* page to view the SQL code.

Comment

Displays a user-entered comment, usually a description of what the
stored procedure does.

Advanced Properties

Run On Validate

If checked and the corresponding Validation rule returns zero records or
if it returns records with a severity level less than Error, the
Business rule executes.

Run On Validate Fail

If checked and the corresponding Validation rule returns any record that
fails with a severity level of Error, the Business rule executes.

Force Foreground Execution

If checked and the workflow is on an event that is set to run in the
background, it will execute twice, once in the foreground and later in
the background.

The intent of the feature is to ensure that the Business rule runs
against the Web Server, even if the event is set to the background. For
example, Force Foreground Execution may be required for plugin access to
the Http Context.

Timeout

Displays the amount of time in seconds that the stored procedure can run
before a timeout error
displays.

### <span id="Procedure_Type_of_Workflow"></span>Procedure Type of Workflow

<div class="use">

Use this page to [Register Workflow
Views](../../../Migration/Console/Use_Cases/Create_Custom_Workflow_Messages#Register).

</div>

Field

Description

Business Rule Properties

Alternate View

Displays the name of the Alternative View. Using an alternate view will
allow for a different set of data when the workflow is created at
runtime. The view will still be restricted by the current record's
primary keys. If multiple records are returned, then multiple workflows
will be sent out.

Workflow Fields

Click to open the *Advanced Workflow* page to configure workflow fields
that determine what displays in the subject line, body text, and other
fields of the workflow. These fields must be added to the view and
aliased correctly to be used in the workflow. Refer to [Configure
Workflow Fields](../Use_Cases/Configure_Workflow_Fields) for more
information about configuring the workflow email sent with this
workflow.

**NOTE:** The Workflow Fields button is not accessible until Save is
clicked.

Message Type ID

Displays the Message Type box that appears when the workflow is
executed. Message Types are configured in System Admin \> Configuration
\> Message Types. This configuration controls how the pop- up message
displays for the user, including the color of the message box and the
image that appears in it. For example, if the message contains as
serious error, select a message type with red coloring and an error X as
the icon.

Comment

Displays a user-entered comment about the workflow.

Link Properties

Workflow Links

Click to open the Workflow Links page to create custom workflow links.
Refer to [Configure Workflow
Links](../Use_Cases/Configure_Workflow_Links) for more information.

**NOTE:** The Workflow Links button is not accessible until Save is
clicked.

Link User ID

The Link User ID used for anonymous users. This list box displays all
Anonymous user accounts. Refer to the [Workflow Views
Overview](../Use_Cases/Workflow_Views) for more information on
creating an anonymous user account

Link Expire Days

Displays the number of days the workflow link is active and therefore
accessible.

Link Reuse

If checked, the workflow link can be used multiple times until it
expires. Otherwise, the user is denied access to the workflow link after
one use.

Link to Page ID

Displays the page the page that opens when the user clicks the link.
Options in this list box display as \[Component Name : Page Name\], for
example, Collect : Copy Targets.

Link to Page Restricted

Restricts page access between two pages bound by key fields. Uncheck the
check box to deactivate the option and allow a link from one page to
another without restrictions. This property is used in conjunction with
the Binding Field Names option. Normally when two pages contain shared
key fields (such as Orders and Order Details), users will want to
restrict the link to page by binding key. Turning this option off allows
the user to link from one page to another without restriction.

Binding Field Names

Displays the binding fields that are required when the primary keys are
not available or if the primary keys have different names. Binding field
names are needed when the linking relationship cannot be inferred,
because keys are either not defined or have different names from parent
to child. Specify them here as one or more parent=child pairs, separated
by commas. For example: *CustomerID=CustID*; or *EmployeeID=EmployeeID*,
*Department=DepartNo.* In cases where the primary keys are not defined,
but the names are identical between parent and child, the =child portion
may be omitted.

Advanced Properties

Run On Validate

If checked and the corresponding Validation rule returns zero records or
if it returns records with a severity level less than Error, the
Business rule executes.

Run On Validate Fail

If checked and the corresponding Validation rule returns any record that
fails with a severity level of Error, the Business rule executes.

Force Foreground Execution

If checked and the workflow is on an event that is set to run in the
background, it will execute twice, once in the foreground and later in
the background.

The intent of the feature is to ensure that the Business rule runs
against the Web Server, even if the event is set to the background. For
example, Force Foreground Execution may be required for plugin access to
the Http Context.

Timeout

Displays the amount of time in seconds that the stored procedure can run
before a timeout error
displays.

### <span id="Procedure_Type_of_External_Page"></span>Procedure Type of External Page

<div class="use">

Use this page to [Create an External Page Business
Rule](../../WebApp_Dev/CreateExternalPageBusinessRule).

</div>

**NOTE:** CranSoft attempts to wrap all procedures within a single SQL
transaction. To avoid deadlocks, all pending transactions are committed
before executing an external process. As a result, mixing external
processes and SQL stored procedures can result in errors which cannot be
completely rolled back. To minimize the effect, consider placing all
external processes after SQL stored procedures by giving them a higher
priority.

Field

Description

Business Rule Properties

Web App Plugin Type Code

Displays the name of the plugin that executes when the event fires.

Comment

Displays a user entered comment about what the code does.

Advanced Properties

Run On Validate

If checked and the corresponding Validation rule returns zero records or
if it returns records with a severity level less than Error, the
Business rule executes.

Run On Validate Fail

If checked and the corresponding Validation rule returns any record that
fails with a severity level of Error, the Business rule executes.

Force Foreground Execution

If checked and the workflow is on an event that is set to run in the
background, it will execute twice, once in the foreground and later in
the background.

The intent of the feature is to ensure that the Business rule runs
against the Web Server, even if the event is set to the background. For
example, Force Foreground Execution may be required for plugin access to
the Http
Context.

### <span id="Procedure_Type_of_WebApp_Event"></span>Procedure Type of WebApp Event

<div class="use">

Use this page to [Create a WebApp Event Business
Rule](../../WebApp_Dev/CreateWebAppEventBusinessRule).

</div>

Field

Description

Business Rule Properties

Event Page ID

Displays the name of the component and page name where the event
associated with this Business rule runs.

Event Name

Displays the name of the event on the page associated with this Business
rule.

Parameter View

Displays the name of an optional parameter view that can provide
secondary data to pass to a shared event.

This view contains columns that are available as extra columns to map to
parameters to send to a shared event. This view will be executed as part
of the shared event, pulling in an associated record to the executing
record, and assigning the other column data to mapped parameters. This
parameter view allows another view to provide more data to an event
without putting all the columns in the horizontal or vertical view on
the page.

This view is not required. If the field is blank, and the public WebApp
event requires parameters be passed in to execute the event, the
parameters set on the *[Page Event Parameters](Page_Event_Param_H)*
page are used.

Parameters

Click to open the *Page Event Rule Parameters* page to add, edit and
delete parameters that can be passed to this Business rule from a Public
WebApp Event.

Comment

Displays a user-entered comment.

Advanced Properties

Run On Validate

If checked and the corresponding Validation rule returns zero records or
if it returns records with a severity level less than Error, the
Business rule executes.

Run On Validate Fail

If checked and the corresponding Validation rule returns any record that
fails with a severity level of Error, the Business rule executes.

Force Foreground Execution

If checked and the workflow is on an event that is set to run in the
background, it will execute twice, once in the foreground and later in
the background.

The intent of the feature is to ensure that the Business rule runs
against the Web Server, even if the event is set to the background. For
example, Force Foreground Execution may be required for plugin access to
the Http
Context.

### <span id="_Procedure_Type_of_WebApp_Event_(Private)"></span> Procedure Type of WebApp Event (Private)

<div class="use">

Use this page to [Create a WebApp Event (Private) Business
Rule](../../WebApp_Dev/CreateWebAppEventPrivateBusinessRule).

</div>

Field

Description

Business Rule Properties

Event Name

Displays the name of the WebApp event.

Comments

Comment

Displays a user-entered comment about the WebApp event.

Advanced Properties

Run On Validate

If checked and the corresponding Validation rule returns zero records or
if it returns records with a severity level less than Error, the
Business rule executes.

Run On Validate Fail

If checked and the corresponding Validation rule returns any record that
fails with a severity level of Error, the Business rule executes.

Force Foreground Execution

If checked and the workflow is on an event that is set to run in the
background, it will execute twice, once in the foreground and later in
the background.

The intent of the feature is to ensure that the Business rule runs
against the Web Server, even if the event is set to the background. For
example, Force Foreground Execution may be required for plugin access to
the Http Context.
