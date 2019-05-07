+++
title = 'Objects H'
solution = 'Migration'
+++

# Objects H

[Objects V (All Tabs)](#Objects_V_All_Tabs)

<div class="use">

Use this page to [Create the Contexts for Migration
Projects](../Use_Cases/Create_Contexts_for_Migration_Projects.htm) and
[Configure an Object](../Use_Cases/Configure_Object.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane, or select
    <span style="font-weight: bold;">Console</span> in the Context bar.
2.  Select <span style="font-weight: bold;">Elements \> Object</span> in
    the <span style="font-style: italic;">Navigation</span> pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Copy Object</p></td>
<td><p>Click to open the <em><a href="Copy_Object.htm">Copy Object</a></em> page to create an object based on a copy of the selected Object.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the Object displays on the <em><a href="#">Objects</a></em> page.</p>
<p><strong>NOTE:</strong> When a Wave-Process Area uses the Object, the Object priority cascades down to Target Design. Once the target that belongs to the object is synced with Map, the priority is also available in Map and displays on the <span style="font-style: italic;">Objects</span> page. The Priority field in Transform is not updated. To change the order the Object is processed, the Priority field can be updated manually in Transform on the <span style="font-style: italic;">Targets</span> page.</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the name of the migration Object.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the migration Object.</p></td>
</tr>
<tr class="even">
<td><p>Contacts</p></td>
<td><p>Click to open the <em><a href="Object_Contacts.htm">Object Contacts</a></em> page to add contacts for the selected Object.</p></td>
</tr>
<tr class="odd">
<td><p>Decisions</p></td>
<td><p>Click to open the <em><a href="Object_Decisions_H.htm">Object Decisions</a></em> page to enter and track issues related to the selected migration Object.</p></td>
</tr>
<tr class="even">
<td><p>History</p></td>
<td><p>Click to open the <em><a href="Object_History_H.htm">Object History</a></em> page, to view the history for the selected Object. History is not tracked for an Object unless the <strong>Build History</strong> check box is checked on the <em>Objects</em> page’s <em>Vertical</em> View.</p></td>
</tr>
</tbody>
</table>

## <span id="Objects_V_All_Tabs"></span>Objects V

[Objects H](Objects_H.htm)

<div class="use">

Use this page to [Create the Contexts for Migration
Projects](../Use_Cases/Create_Contexts_for_Migration_Projects.htm) and
[Configure an Object](../Use_Cases/Configure_Object.htm).

</div>

Field

Description

Basic

Name

Displays the Object name.

Description

Displays a description of the Object.

Priority

Displays the Object’s priority, which is the order the Object displays
on the *Objects* page’s *Horizontal* View.

**NOTE:** When a Wave-Process Area uses the Object, the Object priority
cascades down to Target Design. Once the Target that belongs to the
Object is synced with Map, the priority is also available in Map and
displays on the <span style="font-style: italic;">Objects</span> page.
The Priority field in Transform is not updated. To change the order the
Object is processed, the Priority field can be updated manually in
Transform on the
<span style="font-style: italic;">[Targets](../../Transform/Page_Desc/Targets_H.htm)</span>
page.

Comment

Displays user-entered comments about the Object.

System Details

Target System

Displays the name of the Target system for the migration Object. This is
a free-form text field to store data and is not validated.

Target Tables

Displays the Target tables in the target system for the migration
Object. This is a free-form text field to store data and is not
validated.

Version

Displays the version of the Object. SAP allows different versions for
recordings. This is a free-form text field to store data and is not
validated.

T Code

Displays the SAP Transaction Code or the Target System Type transaction
code. This is a free-form text field to store data and is not validated.

Legacy Systems

Displays the name of the legacy system to load from. This is a free-form
text field to store data and is not validated.

Content Details

Complexity

Displays the complexity for building the Object. This value can be used
to evaluate work assignments. Options include Average, Simple or
Complex. These options can be configured on the *[List Value
Configuration](List_Value_Configuration.htm)* page. If a target is
created in Map that does not have an assigned Complexity, this value
will be passed to Transform to complete the required **Complexity**
field on the *Targets* page’s *Vertical* View on the **Documentation**
tab. A user can then update the complexity in Transform.

Data Type

Displays the type of data represented by the Object. Options include
Master Data, Ref/Conditional, and Transactional. These options can be
configured on the *List Value Configuration* page.

Load Type

Displays the method used to load the object during a Mock Wave. Options
include Automatic, Manual or ALE. These options can be configured on the
*List Value Configuration* page.

Approx Volume

Displays an estimate of the number of records to load for the Object.
This is a free-form text field to store data and is not validated.

Content Driver

Displays the name of the group that is driving the contents. Options
include BU (Business Unit), Company, Enterprise, Legal and team. These
options can be configured on the *List Value Configuration* page.

Spec

Click **Upload** to upload the specifications document to the web
server. If a specifications document has been uploaded, the download
icon is available. Click **Download** to download the document from the
web server.

RICEFW

Displays a RICEFW number. RICEFW is a generic industry term for
"Reports, Interfaces, Conversions, Extensions, Forms and Workflow.” In
the overall Project Plan, Deliverables are often assigned a RICEFW
number to identify and track the development progress of that
item.  Conversion Objects are a deliverable, so therefore they may be
assigned a RICEFW number by the PMO.

Documentation and History

Build History

If checked, Map tracks the history for this Object and display this
information on the *[Object History](Object_History_H.htm)* page.

History Requirements

Displays the user-entered history requirements.

Notes

Displays user-entered notes about the Object.
