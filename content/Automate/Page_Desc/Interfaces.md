+++
title = 'Interfaces H'
solution = 'Platform'
+++

# Interfaces H

[Interfaces V](#InterfacesV)

<div class="use">

Use this page to:

  - [Create an Interface](../Use_Cases/Create_an_Interface)
  - [Schedule Interfaces](../Use_Cases/Schedule_Interfaces)
  - [Activate Interfaces, Events and
    Validations](../Use_Cases/Activate_Interfaces_Events)
  - [Test Interfaces](../Use_Cases/Test_Interfaces)
  - [Schedule Interfaces](../Use_Cases/Schedule_Interfaces)
  - [View History of an
    Interface](../Use_Cases/View_History_of_an_Interface)

</div>

To access this page, select **Interfaces** in the *Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>GROUP</p></td>
<td><p>Displays the name of the interface group. Interface groups are used to categorize interfaces.</p></td>
</tr>
<tr class="odd">
<td><p>ORDER</p></td>
<td><p>Displays a number to order the interfaces within a group.</p></td>
</tr>
<tr class="even">
<td><p>INTERFACE ID</p></td>
<td><p>Displays a system-generated ID to uniquely identify the interface.</p></td>
</tr>
<tr class="odd">
<td><p>INTERFACE</p></td>
<td><p>Displays the name of the interface.</p></td>
</tr>
<tr class="even">
<td><p>DATA SOURCE ID</p></td>
<td><p>Displays the name of the data source registered to Automate that stores the stored procedures, validation views, and workflow views used by the interfaces.</p></td>
</tr>
<tr class="odd">
<td><p>QUEUE ID</p></td>
<td><p>Displays the service queue used when the interface runs. Queue ID is used to serialize certain operations or for load balance.</p>
<p>Options are:</p>
<ul>
<li><strong>Background Event –</strong> The background service controls job queue.</li>
<li><strong>General –</strong> The job is on General queue.</li>
<li><strong>Index –</strong> The job is on Index queue.</li>
<li><strong>Service Pages –</strong> The associated Service page controls the job queue.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>SCHEDULE TYPE</p></td>
<td><p>Displays the scheduling options for running an interface. Options are:</p>
<ul>
<li><strong>Frequency—</strong>A numeric value describing how often the schedule runs.</li>
<li><strong>RunTime—</strong> The specific time when the interface runs.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>SCHEDULE</p></td>
<td><p>Displays how often the interface runs based on the Frequency and UOM fields.</p>
<p><strong>NOTE:</strong> This field is auto-populated by Automate and only displays if the Schedule Type is Frequency.</p></td>
</tr>
<tr class="even">
<td><p>RUN TIME</p></td>
<td><p>Displays the time the schedule runs.</p>
<p><strong>NOTE:</strong> This field is only populated if the Schedule Type is RunTime.</p></td>
</tr>
<tr class="odd">
<td><p>DAYS</p></td>
<td><p>Displays when the interface runs based on the days selected on the Schedule Info tab on the <em><a href="#InterfacesV">Vertical</a></em> View.</p></td>
</tr>
<tr class="even">
<td><p>COMMENT</p></td>
<td><p>Displays a comment about the interface’s functionality that is entered in the General tab on the <em><a href="#InterfacesV">Vertical</a></em> View.</p></td>
</tr>
<tr class="odd">
<td><p>THREAD SAFE</p></td>
<td><p>This field is not used.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If checked, the interface has been tested and is ready to be run.</p>
<p>If unchecked, the interface has not been tested and is not ready to be run.</p>
<p>It is checked by default.</p>
<p><strong>NOTE:</strong> When checked, the Execute and Submit icons are enabled on the <em><a href="#InterfacesV">Vertical</a></em> View. </p></td>
</tr>
<tr class="odd">
<td><p>Events</p></td>
<td><p>Click to open the <em><a href="Interface_Events">Interface Events</a></em> page. Use this page to register interface events.</p>
<p>The count on the icon is the total number of events registered to the selected interface.</p></td>
</tr>
<tr class="even">
<td><p>Validations</p></td>
<td><p>Click to open the <a href="Interface_Validations"><em>Interface Validations</em></a> page. Use this page to register interface event validations.</p>
<p>The count on the icon is the total number of validations registered to the selected interface.</p></td>
</tr>
<tr class="odd">
<td><p>History</p></td>
<td><p>Click to open the <em><a href="Interface_History">Interface History</a></em>page to view historical details of the interface: when it ran,  how long it took to run, tasks associated with the interface, etc.</p></td>
</tr>
</tbody>
</table>

# <span id="InterfacesV"></span> Interfaces V

[Interfaces H](#InterfacesH)

This page contains the following tabs:

  - [General](#_General) tab
  - [Contact Info](#_Contact_Info) tab
  - [Schedule Info](#_Schedule_Info) tab
  - [Logging](#_Logging) tab

## <span id="_General"></span> General tab

<div class="use">

Use this tab to [Create an
Interface](../Use_Cases/Create_an_Interface).

</div>

Field

Description

Interface ID

Displays a system-generated ID to uniquely identify the interface.

Interface

Displays the name of the interface.

Comment

Displays a comment about the interface’s functionality.

Actions

Debug

Click to test the interface in Debug mode with full logging information.
The interface is immediately run in the foreground. Debug Mode (on the
[Logging](#_Logging) tab) must be enabled in order for this feature to
work.

**NOTE:** This icon is active when the ACTIVE check box is checked on
the *[Horizontal](#InterfacesH)* View.

Execute

Click to test the interface. The interface is immediately run in the
foreground.

**NOTE:** This icon is active when the ACTIVE check box is checked on
the *[Horizontal](#InterfacesH)* View.

Submit

Click to submit the interface to the job queue (i.e., to run in the
background).

**NOTE:** This icon is active when the ACTIVE check box is checked on
the *[Horizontal](#InterfacesH)* View.

Monitor

Click to open the *[Monitor](Monitor_H)* page to view and interact
with interfaces that are currently running or that have failed.

Reset

Click to reset the last run information and status of the current
interface. The Status of the interface is set to Validation Passed and
all jobs reference fields are NULLed out. The interfaces looks like it
has never been run, but all history is maintained.

History Info

History

Click to open the *[Interface History](Interface_History)* page to
view historical data of the interface: when it ran, how long it took to
run, tasks associated with the interface, etc.

Last Run Date

Displays the date and time at which the interface last ran.

Last Run Completed

Displays the date and time at which the interface last completed.

 

## <span id="_Contact_Info"></span> Contact Info tab

<div class="use">

Use this tab to:

  - [Set Up Notifications for an
    Interface](../Use_Cases/Set_Up_Notifications_for_an_Interface)
  - [Schedule Interfaces](../Use_Cases/Schedule_Interfaces)

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Message Success</p></td>
<td><p>Displays the message to be displayed upon a successful completion of running an interface.</p></td>
</tr>
<tr class="odd">
<td><p>Message Failure</p></td>
<td><p>Displays the message to be displayed upon an unsuccessful completion of running an interface.</p></td>
</tr>
<tr class="even">
<td><p>Business Role</p></td>
<td><p>Displays the role that receives the notification workflow email, depending on how workflow notification options are set.</p>
<p>A user is assigned to a role. Refer to <a href="../Use_Cases/Assign_Users_to_Roles">Assign Users to Roles</a> for more information. </p></td>
</tr>
<tr class="odd">
<td><p>Business Notification Option</p></td>
<td><p>Displays when a notification workflow is sent to the Business Role. Options are:</p>
<ul>
<li><strong>Always –</strong> Sends an email notification when an interface completes, regardless of the interface status.</li>
<li><strong>Failure Only –</strong> Sends an email notification only if the interface fails.</li>
<li><strong>Success Only –</strong> Sends an email notification only if the interface completes successfully.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Development Role</p></td>
<td><p>Displays the recipient of an automated interface email.</p></td>
</tr>
<tr class="odd">
<td><p>Development Notification Option</p></td>
<td><p>Determines when to send an automated interface email to the specified Development Role. Options are:</p>
<ul>
<li><strong>Always –</strong> Sends an email notification when an interface completes, regardless of the interface status.</li>
<li><strong>Failure Only –</strong> Sends an email notification only if the interface fails.</li>
<li><strong>Success Only –</strong> Sends an email notification only if the interface completes successfully.</li>
</ul></td>
</tr>
</tbody>
</table>

 

## <span id="_Schedule_Info"></span> Schedule Info tab

<div class="use">

Use this tab to [Schedule
Interfaces](../Use_Cases/Schedule_Interfaces).

</div>

Field

Description

Frequency

Displays the frequency at which the interface runs.

**NOTE:** This field only displays if the Schedule Type is Frequency.

UOM

Displays the UOM (Units of Measure) that dictate the frequency of the
interface runs. Options are:

  - Day
  - Hour
  - Minute
  - Month
  - Second

**NOTE:** This field only displays if the Schedule Type is Frequency.

Schedule

Displays how often the interface runs based on the Frequency and UOM
fields.

**NOTE:** This field is auto-populated by Automate and only displays if
the Schedule Type is Frequency.

Run Time

Displays the specific time when the interface runs.

**NOTE:** This field only displays if the Schedule Type is RunTime.

Days

Displays when the interface runs based on the days selected.

Days Info

Monday

If checked, the interface runs on Mondays.

If unchecked, the interface does not run on Mondays.

It is checked by default.

Tuesday

If checked, the interface runs on Tuesdays.

If unchecked, the interface does not run on Tuesdays.

It is checked by default.

Wednesday

If checked, the interface runs on Wednesdays.

If unchecked, the interface does not run on Wednesdays.

It is checked by default.

Thursday

If checked, the interface runs on Thursdays.

If unchecked, the interface does not run on Thursdays.

It is checked by default.

Friday

If checked, the interface runs on Fridays.

If unchecked, the interface does not run on Fridays.

It is checked by default.

Saturday

If checked, the interface runs on Saturdays.

If unchecked, the interface does not run on Saturdays.

It is checked by default.

Sunday

If checked, the interface runs on Sundays.

If unchecked, the interface does not run on Sundays.

It is checked by default.

 

## <span id="_Logging"></span> Logging tab

<div class="use">

Use this tab to:

  - [Schedule Interfaces](../Use_Cases/Schedule_Interfaces)
  - [Test Interfaces](../Use_Cases/Test_Interfaces)

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Debug Mode</p></td>
<td><p>If checked, Storage Level is ignored and only tasks with severities of Debug and higher are written to the <em><a href="Log">Log</a></em> page.</p>
<p>If unchecked, all tasks are written to the interface’s log.</p>
<p>It is unchecked by default.</p></td>
</tr>
</tbody>
</table>
