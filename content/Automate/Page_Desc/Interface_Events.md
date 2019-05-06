# <span id="InterfaceEventsH"></span> Interface Events H

[Interface Events V](#InterfaceEventsV)

<div class="use">

Use this page to:

  - [Register Interface
    Events](../Use_Cases/Register_Interface_Events.htm)
  - [Register Stored Procedure
    Events](../Use_Cases/Register_Stored_Procedure_Events.htm)
  - [Register WebApp Events](../Use_Cases/Register_WebApp_Events.htm)
  - [Register Workflow
    Events](../Use_Cases/Register_Workflow_Events.htm)
  - [Copy Files from One Folder to
    Another](../Use_Cases/Copy_Files_from_One_Folder_to_Another.htm)
  - [Set Up a Looping
    Process](../Use_Cases/Set_up_a_Looping_Process.htm)

</div>

To access this page:

1.  Select **Interfaces** in the *Navigation* pane.
2.  Click the **Events** icon for the desired interface.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>EVENT ID</p></td>
<td><p>Displays a system-generated ID to uniquely identify the event.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays a value that determines the order in which the event runs.</p></td>
</tr>
<tr class="even">
<td><p>EVENT TYPE</p></td>
<td><p>Displays the type of event. Options are:</p>
<ul>
<li>Stored Procedure</li>
<li>WebApp</li>
<li>Workflow</li>
</ul>
<p><strong>NOTE:</strong> The Event Type selected on the <em>Horizontal</em> View of the <em><a href="#">Interface Events</a></em> page determines the configuration options available on the <em><a href="#InterfaceEventsV">Vertical</a></em> View.</p></td>
</tr>
<tr class="odd">
<td><p>PAGE ID</p></td>
<td><p>Displays the page for which the event runs.</p>
<p><strong>NOTE:</strong> This field only applies to WebApp events. </p></td>
</tr>
<tr class="even">
<td><p>EVENT</p></td>
<td><p>Displays the event that executes, which is selected on the <em><a href="#InterfaceEventsV">Vertical</a></em> View. The events that are available are those registered to the page selected in the Page ID field.</p>
<p><strong>NOTE:</strong> This field only applies to WebApp events. </p></td>
</tr>
<tr class="odd">
<td><p>LOOP</p></td>
<td><p>If checked, the event is intended to be processed multiple times based on input, (e.g. an Automate IO process that downloads multiple files, each of which must be processed individually).</p>
<p>If unchecked, the event is not processed multiple times.</p>
<p>Refer to <a href="../Use_Cases/Set_up_a_Looping_Process.htm">Set Up a Looping Process</a> for more information.</p>
<p>It is unchecked by default.</p></td>
</tr>
<tr class="even">
<td><p>OBJECT</p></td>
<td><p>Displays the name of the workflow view (with the naming convention wf:[WorkflowView])or thestored procedure (with the naming convention sp:[StoredProcedureName])</p>
<p><strong>NOTE:</strong> This field is only populated for Workflow and Stored Procedure events.</p></td>
</tr>
<tr class="odd">
<td><p>COMMENT</p></td>
<td><p>Displays a description of the event.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If checked, the event has been tested and is ready to be run.</p>
<p>If unchecked, the event does not run when the interface is either manually run or set to run on a schedule.</p>
<p>It is checked by default.</p></td>
</tr>
<tr class="odd">
<td><p>Parameters</p></td>
<td><p>Click to open a parameters page unique to the Event Type:</p>
<ul>
<li>For Workflow events, the <em><a href="Workflow.htm">Workflow</a></em> page displays.</li>
<li>For WebApp events, the <em><a href="WebApp_Event.htm">WebApp Event</a></em> page displays.</li>
<li>For Stored Procedure events, the <em><a href="Stored_Procedure.htm">Stored Procedure</a></em> page displays.</li>
</ul>
<p>Use these pages to set parameters for the event. The parameters in the code are automatically registered to the parameters page for the event.</p></td>
</tr>
<tr class="even">
<td><p>Validations</p></td>
<td><p>Click to open the <em><a href="Interface_Event_Validations.htm">Interface Event (Validations)</a></em> page. Use this page to add validations at the event level, versus at the interface level.</p>
<p>The count on the icon is the total number of validations registered to the selected event.</p></td>
</tr>
</tbody>
</table>

# <span id="InterfaceEventsV"></span> Interface Events V

[Interface Events H](#InterfaceEventsH)

Field

Description

Event ID

Displays a system-generated ID to uniquely identify the event.

Stored Procedure

Displays the stored procedure assigned to the event.

**NOTE:** This field only displays for Stored Procedure events.

Stored Procedure Parameters

Click to open the *[Stored Procedure](Stored_Procedure.htm)* page to
view parameters passed to the event. The parameters in the stored
procedure event code are automatically registered to the *[Stored
Procedure](Stored_Procedure.htm)* page for the event.

**NOTE:** This field only displays for Stored Procedure events.

Event Type

Displays the type of event. Options are:

  - Stored Procedure
  - WebApp
  - Workflow

The Event Type selected on the *[Horizontal](#InterfaceEventsH)* View of
the *[Interface Events](#)* page determines the configuration options
available on the *[Vertical](#InterfaceEventsV)* View.

Page ID

Displays the page for which the event runs.

**NOTE:** This field only displays for WebApp events. 

Event

Displays the event that executes, which is selected on the *Vertical*
View. The events that are available are those registered to the page
selected in the Page ID field.

**NOTE:** This field only displays for WebApp events. 

WebApp Parameters

Click to open the *[WebApp Event](WebApp_Event.htm)* page to view
parameters (i.e., fields and values) passed to the event. The parameters
in the WebApp event code are automatically registered to the *[WebApp
Event](WebApp_Event.htm)* page for the event.

**NOTE:** This field only displays for WebApp events.

View

Displays the workflow view used by the workflow event. The view is
created in the Data Source assigned when the interface was created on
the *[Interfaces](Interfaces.htm)* page.

**NOTE:** This field only displays for Workflow events.

Fields

Click to open the *[Workflow (Email)](Workflow_Email.htm)* page to
configure the email settings for the workflow notification, such as
subject line and body text. These fields must be added to the view and
aliased correctly to be utilized by the workflow. Refer to *[Configure
Workflow
Fields](../../Sys_Admin/Use_Cases/Configure_Workflow_Fields.htm)* in the
System Administration help for more information.

**NOTE:** This field only displays for Workflow events.

Links

Click to open the *[Workflow Links](Workflow_Links.htm)* page to add
links that navigates a user to a specific page to then perform a
function. Refer to *[Configure Workflow
Links](../../Sys_Admin/Use_Cases/Configure_Workflow_Links.htm)* in the
System Administration help for more information.

**NOTE:** This field only displays for Workflow events.

Workflow Properties

Workflow Method

Displays the protocol for sending and receiving emails.

**NOTE:** This field only displays for Workflow events.

Workflow User ID

If populated, anonymous workflow is used and Workflow User ID displays
the user ID who receives the workflow email.

If blank, standard workflow is used. Refer to *[Workflow
Overview](../../Sys_Admin/Use_Cases/Workflow_Views.htm)* in System
Administration help for more information.

**NOTE:** This field only displays for Workflow events.

Workflow Expire Days

Displays the number of days in which a Workflow expires. After the
defined number of days, the workflow link no longer works for the user.

**NOTE:** This field only displays for Workflow events.

Workflow Reuse

If checked, the workflow is reusable for other interface events.

If unchecked, the workflow is not reusable for other interface events.

It is unchecked by default.

**NOTE:** This field only displays for Workflow events.

Link To Page ID

Displays the page that opens when the user clicks the workflow link in
the workflow email.

**NOTE:** This field only displays for Workflow events.

Link To Page Restricted

If checked, page access between two pages bound by key fields is
restricted.

If unchecked, page access between two pages bound by key fields is not
restricted, i.e., pages can be linked without restriction.

It is unchecked by default.

This field is used in conjunction with the Binding Fieldnames field. 
Normally when two pages contain shared key fields (such as Orders and
Order Details), restrict the link to page by binding key.

**NOTE:** This field only displays for Workflow events.

Binding Fieldnames

Displays the fields to bind the workflow event. Binding fields are
required when the primary keys are not available or if the primary keys
have different names. They are needed when the linking relationship
cannot be inferred because keys are either not defined or have different
names from parent to child. Specify the field names here as one or more
parent=child pairs, separated by commas. For example: CustomerID=CustID;
or EmployeeID=EmployeeID, Department=DepartNo. (=child portion may be
omitted if names are not different.)

**NOTE:** This field only displays for Workflow events.

Retry Parameters

Retry Interval

Displays the interval at which to retry running the event. If the Retry
Interval field is set 5, and the UOM is set to Hours, when the event
fails, the DSP tries to run it again in 5 hours.

Maximum Retry Interval

Displays the number of times the event runs until it stops. If the
Maximum Retry Interval is 10, and if the event fails, it will retry
according to the Retry Interval and Retry Interval UOM for 10 times and
then stop.

Retry Interval UOM

Displays the unit of measure used with the Retry Interval. Options are:

  - Day
  - Hour
  - Minute
  - Month
  - Second
