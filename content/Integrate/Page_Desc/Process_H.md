+++
title = 'Process H'
solution = 'Platform'
+++

# Process H

[Process V All Tabs](#Process_V_All_Tabs)

<div class="use">

Use this page to [Create a Process](../Use_Cases/Create_a_Process)
and Activate a Process.

</div>

<span style="font-weight: bold;">NOTE</span>: Refer to the section on
each template type for information about activating a process.

To access this page:

1.  Select <span style="font-weight: bold;">Integrate \>
    </span>**Categories** from *Navigation pane*.
2.  Click the **Processes** icon for a category.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Category Templates</p></td>
<td><p>Click to open the <em><a href="Template_H">Template</a></em> page to view a list of all active and inactive templates assigned to the Category.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the process appears on the <em>Process</em> page’s <em>Horizontal View.</em></p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the unique name for the process entered on the <em>Process</em> page’s <em>Vertical</em> View.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the process entered on the <em>Process</em> page’s <em>Vertical</em> View.</p></td>
</tr>
<tr class="even">
<td><p>DATA SOURCE ID</p></td>
<td><p>Displays the name of the data source for the process. Integrate maps the data stored in this data source to a process template. This value was selected from a list of all data sources registered to the platform on the <em>Process</em> page’s <em>Vertical</em> View.</p></td>
</tr>
<tr class="odd">
<td><p>Templates</p></td>
<td><p>Click to open the <em><a href="Process_Templates_H">Process Templates</a></em> page to add, edit or delete the templates associated with the process. This action can only be performed when the process is inactive.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVATE/DEACTIVATE</p></td>
<td><p>Click to activate or deactivate the process. The button displays a green icon for active processes and a red icon for inactive processes.</p>
<p><strong>NOTE:</strong> When using dspConduct™ component with Integrate, if the scenario is in any status other than Published, the Designer can activate or deactivate the process in Integrate as needed to test and troubleshoot the process. Refer to <a href="../../../Master_Data_Mgmt/dspConduct/Use_Cases/Manage_Scenarios">Manage dspConduct™ Scenarios</a> for more information about working with scenarios in dspConduct™.</p></td>
</tr>
<tr class="odd">
<td><p>Active</p></td>
<td><p>If enabled, the process is active.</p></td>
</tr>
<tr class="even">
<td><p>Postings</p></td>
<td><p>Click to open the <em><a href="Process_Post_H">Process Post</a></em> page to view details about the process posts and to post data to SAP. The number displays the total of process posts added whether posted or not. If the process is not active, this icon is disabled.</p></td>
</tr>
<tr class="odd">
<td><p>Report</p></td>
<td><p>Click to open the Report  Process  to view details about the process such as the templates assigned to the process, process template loops, field mappings, and relationships.</p></td>
</tr>
</tbody>
</table>

## <span id="Process_V_All_Tabs"></span>Process V All Tabs

[Process H](Process_H)

<div class="use">

Use this page to [Create a Process](../Use_Cases/Create_a_Process)
and Activate a Process.

</div>

This page has the following tabs:

  - [General tab](#General_Tab3)
  - [Documentation tab](#Documentation_Tab1)
  - [Posting tab](#Posting_Tab)
  - [Advanced Properties tab](#Advanced_Properties_Tab)
  - [Copy tab](#Copy_Tab2)

## <span id="General_Tab3"></span>General tab

Field

Description

Templates

Click to open the *[Process Templates](Process_Templates_H)* page to
add, edit and delete the templates associated with the process.

Basic Properties

Priority

Displays the order the process appears on the *Process* page’s
*Horizontal* View.

Name

Displays the unique name for the process entered when the process was
added.

Description

Displays a description of the process.

Template ID

Select the template to be the initial template for the process.
Additional templates can be added later. This list box is only visible
when adding a process.

Data Source Properties

Data Source ID

Displays the name of the data source for the process. Integrate posts
the data stored in this data source to SAP during the post process
 depending on the template type . When adding the process, a user
selected the data source from a list of all data sources registered to
the platform.

View Name

Displays on this page when adding a process only. Select a view from
**View Name** list box depending on the template type. This field is
required when adding a process based on a BDC Script or GUI Script.
After the process is saved, the **View Name** field no longer displays
on the *Vertical* View, and so cannot be edited on this page.

**NOTE:** To streamline adding a process, the selected view is
registered as the view for all process template loops to the initially
chosen template, and the columns in the view are automatically mapped to
matching fields on the *Process Template Loop Field Mapping* page.

Integrate can automatically generate the view name when using the Auto
Generate Database Objects feature. If using this feature, do not select
a view name.

## <span id="Documentation_Tab1"></span>Documentation tab

Field

Description

Template Documentation

Notes

Displays information entered about the process.

Report

Click to open the Report  Process  to view details about the process
such as the templates assigned to the process, process template loops,
field mappings, and relationships.

## <span id="Posting_Tab"></span>Posting tab

Field

Description

Process Post

Postings

Click to open the *[*Process Post*](Process_Post_H)* page to view
details about the process posts and to post data to SAP. If the process
is inactive, the icon is disabled. The number displays the total of
process posts ready to be posted. If the icon displays no numbers, no
process posts have been added.

## <span id="Advanced_Properties_Tab"></span>Advanced Properties tab

Field

Description

Execution Options

Post Execution Method

Displays the post execution method for processes based on a BDC Script,
GUI Script or BAPI/RFC template. Values are:

  - **Asynchronous** – Executes the post for each template sequentially
    without waiting for the template post to return before executing the
    next template post. Asynchronous posting may result in locking,
    especially when posting a combination of GUI and BDC templates in
    the same process.
  - **Synchronous** – Executes the post for each template but waits for
    the post to return before executing the next post. Synchronous is a
    slower execution method but prevents most recording locking
    situations. 

Delay Between Templates

Displays the number of
<span style="font-family: &#39;Bookman Old Style&#39;, serif;">milliseconds</span>
between template execution for each post for processes based on a BDC
Script, GUI Script or BAPI/RFC template. The default value is 0 seconds,
which indicates there is no delay between the execution of templates
during a post. Enter a value greater than 0 if posting a multiple
template process that contain transactions that take some non-trivial
time to save and exit. This situation is more common when working with
GUI Script templates than with BDC Script templates.

Delay Between Records

Displays the amount of time, in milliseconds, that passes after
processing of one record is complete and processing of the next record
can begin.

Use this setting to avoid data locking issues.

The recommended time is from 250 (.25 seconds) to 1000 (1 second).

This setting is used for processes based on a BDC Script, GUI Script or
BAPI/RFC template. By default, there is no delay between record
processing.

## <span id="Copy_Tab2"></span>Copy tab

Field

Description

New Process Settings

Copy Process

Click to open the *[Copy](Copy)* page to create a process based on a
copy of the current process.
