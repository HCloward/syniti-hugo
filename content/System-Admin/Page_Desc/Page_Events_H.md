+++
title = ''
solution = 'Platform'
+++

# <span id="Page_Events_H"></span>Page Events H

[Page Events V](#Page_Events_V)

<div class="use">

Use this page to:

  - [Register Workflow Views](../Use_Cases/Register_Workflow_Views.htm)
  - [Create an OnValidate Page Event for Bulk
    Execution](../Use_Cases/Create_an_OnValidate_Page_Event_for_Bulk_Execution.htm)
  - [Register a Validation Rule to a
    Page](../../WebApp_Dev/ValidationRules.htm)
  - [Create a Business Rule for a
    Field](../../WebApp_Dev/Create_a_Business_Rule_for_a_Field.htm)

</div>

Refer to [Event Design
Process](../../WebApp_Dev/Event_Design_Process.htm) for additional
information about this page.

To access this page:

1.  Select **Admin \> WebApps**in the *Navigation* pane.
2.  Click the **Pages** icon for a **WEB APP NAME**.
3.  Click the **Events** icon for a **DESCRIPTION**.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>EVENT</p></td>
<td><p>Displays the event that runs on the page, or the name of the field that triggers the event rule to run.</p>
<p>Event rules can be created to run:</p>
<ul>
<li><p><strong>OnLoad –</strong> Executes prior to the page displaying, allowing lazy data population.</p>
<p><strong>NOTE:</strong> This event rule is not available for Service pages.</p></li>
<li><p><strong>OnValidate –</strong> Executes when a record is saved or the user clicks the boaStatus icon.</p>
<p><strong>NOTE:</strong> This event rule is not available for Report pages.</p></li>
<li><p><strong>BeforeDelete –</strong> Executes before a record can be deleted.</p>
<p><strong>NOTE:</strong> BeforeDelete events can be run in the Background only.</p>
<p><strong>NOTE:</strong> This event rule is not available for Service pages.</p></li>
<li><strong>Columns –</strong> Executes at the record level when a user clicks a specific field.The options display as the names of the columns that can have record-level events added.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If checked, the workflow will be run.</p>
<p>If unchecked, the workflow will not be run.</p></td>
</tr>
<tr class="even">
<td><p>EVENT PROCESS TYPE ID</p></td>
<td><p>Displays the process type of the event – foreground or background. Any event running for more than several seconds must be run in the background and must be assigned to a queue. If the process takes fewer than several seconds to run, or if the process needs user-session level context, set it to run in the foreground. A Foreground event runs on the web server, which can give plugin code access to specific user and runtime information from the web session. A Foreground event can also provide immediate feedback to the user, such as reloading the page and displaying post event messages.</p></td>
</tr>
<tr class="odd">
<td><p>Validation Rules</p></td>
<td><p>Click to open the <em><a href="Page_Validation_Rules.htm">Page Validation Rules</a></em> page to add and edit a validation rule. Validation rules run before business rules and validate data based on certain conditions.</p></td>
</tr>
<tr class="even">
<td><p>Business Rules</p></td>
<td><p>Click to open the <em><a href="Page_Business_Rules_H.htm">Page Business Rules</a></em> page to add and edit a Business rule. Business rules run after validation rules complete. Business rules execute based on whether validations pass or fail.</p></td>
</tr>
</tbody>
</table>

## <span id="Page_Events_V"></span>Page Events V

[Page Events H](#Page_Events_H)

<div class="use">

Use this page to [Register Workflow
Views](../Use_Cases/Register_Workflow_Views.htm).

</div>

This page has the following tabs:

  - [General tab](#General_Tab)

  - [Advanced Properties tab](#Advanced_Properties)

  - [Bulk Execution tab](#Bulk_Execution)

## <span id="General_Tab"></span>General tab

**NOTE:** The Bulk Execution tab will only be seen if Bulk Execution is
enabled. Refer to [Enable Bulk Execution for a
Page](../Use_Cases/Enable_Bulk_Execution_for_a_Page.htm) for more
information.

Field

Description

Event Description

Page

Displays the name of the page. This value is populated from the
DESCRIPTION field on the Page's page and is not editable.

Event

Displays the event that runs on the page, or the name of the field that
triggers the event rule to run.

Event rules can be created to run:

  - **OnLoad –** Executes prior to the page displaying, allowing lazy
    data population.
    
    **NOTE:** This event rule is not available for Service pages.

  - **OnValidate –** Executes when a record is saved or the user clicks
    the boaStatus icon.
    
    **NOTE:** This event rule is not available for Report pages.

  - **BeforeDelete –** Executes before a record can be deleted.
    
    **NOTE:** BeforeDelete events can be run in the Background only.
    
    **NOTE:** This event rule is not available for Service pages.

  - **Columns –** Executes at the record level when a user clicks a
    specific field. The options display as the names of the columns that
    can have record-level events added.

Messages

Pre Message

Displays the message that appears before running this event and prompts
the user with a confirmation message to continue. Most irreversible or
not easily reversible actions should include a Pre Message to ensure the
user doesn’t accidentally disrupt a process. If the Pre Message is not
specified, then the user will not receive a message that the process is
about to occur.

Post Message

Displays the message that appears when this event finishes processing.

Post Messages display at different times depending on whether the event
runs in the foreground or background.

A Background event displays the message as a Minor Notification,
immediately after the job has been queued. In this case, use the Post
Message to indicate to the user that the work will be run at a certain
time (for example, “The package will be processed shortly.”).

Foreground events display their message after execution. Post Messages
for Foreground events are useful when executing plugin code that doesn’t
always write out a message, or when executing non-plugin Business rules.
This ensures that the user always receives a confirmation that their
action has completed.

If the Post Message is not specified, then the user will not receive a
message that the process has completed.

Comments

Comment

Displays comments entered by the user.

## <span id="Advanced_Properties"></span>Advanced Properties

**NOTE:** The Bulk Execution tab will only be seen if Bulk Execution is
enabled. Refer to [Enable Bulk Execution for a
Page](../Use_Cases/Enable_Bulk_Execution_for_a_Page.htm) for more
information.

Field

Description

Transaction Method

Displays the method in which the event is executed. There are three
options:

  - **Disabled –** This option provides the least likeliness of a
    deadlock as well as fastest execution time. However, when running a
    series of procedures, an error in one will not result in a rollback
    of the previous procedures. This could potentially leave the
    database in an unstable state, if these procedures are not
    idempotent.

  - **Enabled –** This option provides the functionality of rolling back
    in the event of an error. This rollback is applied per Execution
    Groups, which are formed by sequential sets of stored procedures.
    For example:
    
    1.  Three stored procedures run.
    2.  An External Page runs.
    3.  Three more procedures run.
    
    This results in two Execution Groups (first three, and last three).
    In the event a procedure within one of the Execution Groups fails,
    any other procedure that has been run within that group is undone.
    This setting carries the highest potential of deadlock. A failure
    within an Execution Group does not cause any other execution groups
    to roll back.

  - **Serialized –** This option is similar to Enabled, with the added
    locking at the Page Event level. When this option is chosen, each
    event invocation will ensure exclusive execution of the underling
    Page Events rules. This option reduces the number of procedure
    related deadlocks occurring, but can lead to event lock related
    timeouts if several users are attempting to execute the same event
    simultaneously.
    
    **NOTE:** This option must **not** be used if the column property
    supports multi-row actioning.

Function

Displays whether the user is navigated back to the previous page or to
the page’s *Vertical* View after the Event rule(s) finishes processing.

For example, the Page Designer sets this option to Back in cases where
the user may be expected to navigate to a second page, click a
particular button, and then be sent back to the previous page where that
event has affected the previous record.

The Page Designer sets this option to Vertical in cases where an action
on the *Horizontal* View results in information that must display to the
user on the *Vertical* View.

Event Level

Displays the level at which the event is run, either at the page level
or against a specific record on the page. The default and most commonly
used Event Level is Row, which passes the row information to the event.

Page level execution is only supported for toolbar buttons defined from
the Toolbar view for the page. It does not pass row-level information to
the event. If a toolbar button is set to page-level event, the button
can be clicked when there are no records on the page.

**NOTE:** When the event is OnLoad, the only option in this list box is
Page.

Support Bulk Execution

If checked, the Bulk Execution feature is enabled on the page and the
Bulk Execution tab is visible.

Bulk Execution is the ability to run an event on a DSP page for all
records or a subset of those records via a simple, guided user
experience.

**NOTE:** Bulk Execution is only available for On Validate events that
run in the background.

Refer to *[Use Bulk Execution](../../Bulk_Exec/Use_Bulk_Execution.htm)*
and *[Configure Bulk
Execution](../Use_Cases/Configure_Bulk_Execution_Overview.htm)* for more
information.

Queue ID

Displays the queue where the job associated with the background event
runs.

**NOTE:** This field displays for background events only and must be set
for the event to run.

Web App Event Properties

Public

If checked, this Event can be called via a business rule from a page in
any WebApp. The page’s keys are inserted into the Page Event Parameters
as the initial parameters.

**NOTE:** If unchecked, the Parameters icon is not active.

Page View Type

Displays whether the Event runs on the *Horizontal* or *Vertical* View.

Parameters

Click to open the *[Page Event Parameters](Page_Event_Param_H.htm)*
page, where a user can view, add and edit parameters required to call
this public WebApp Event. At a minimum, these include the primary keys
for this table.

**NOTE:** Parameters can be set for Public events only. The Public check
box must be checked for this icon to be active.

## <span id="Bulk_Execution"></span>Bulk Execution

<div class="use">

Use this tab to [Configure Business Rule
Settings.](../Use_Cases/Configure_Business_Rule_Settings.htm)

</div>

<span style="font-weight: bold;">NOTE:</span> This tab displays if the
Support Bulk Execution check box is checked on the Advanced Properties
tab. Refer to [Enable Bulk Execution for a
Page](../Use_Cases/Enable_Bulk_Execution_for_a_Page.htm) for more
information.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Exclude Business Rule Default</p></td>
<td><p>If checked, any business rules registered to the OnValidate event are not run. The Exclude Business Rules check box on the Bulk Execution panel is checked.</p>
<p>If unchecked, business rules registered to the OnValidate event run by default, and the Exclude Business Rules check box on the Bulk Execution panel is unchecked.</p></td>
</tr>
<tr class="odd">
<td><p>Exclude Business Rule Option</p></td>
<td><p>If checked, the Exclude Business Rules check box on the Bulk Execution panel is checked, and the user cannot update it.</p>
<p>If unchecked, the user can update the Exclude Business Rules check box on the Bulk Execution panel.</p></td>
</tr>
</tbody>
</table>
