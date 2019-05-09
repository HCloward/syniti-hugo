+++
title = 'Target Sources H'
solution = 'Migration'
+++

# Target Sources H

[Target Sources V](Target_Sources_H_Design#Target_Sources_V)

<div class="use">

Use this page to [Assign a Source to a
Target](../Use_Cases/Assign_a_Source_to_a_Target).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Design </span>in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Targets</span>icon on the
    *[Design](Design)* page.
4.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>SOURCE DATA SOURCE</p></td>
<td><p>Displays the database that stores the Source tables that contain the data that will be migrated to the Target.</p>
<p>Click the <strong>+</strong> icon in this field to open the <span style="font-style: italic;"><a href="../../../Platform/Common/Page_Desc/Data_Source_Registry_H">Data Source Registry</a></span> page to add a data Source if necessary.</p>
<p>Data sources should be registered in Common. Refer to <a href="../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common">Register a Data Source in Common</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE TYPE</p></td>
<td><p>Displays the type of Source data source.</p>
<p>Values are:</p>
<ul>
<li><span style="font-weight: bold;">Add Row -</span> A Source database that contains the data from the Source system to be moved to the Target.</li>
<li><span style="font-weight: bold;">Full Construction -</span> A Source that will be manually created using Construct. This option is set by default when a user selects {Full Construction} from the SOURCE DATA SOURCE list box. This option is not available for any other Source data sources.</li>
<li><span style="font-weight: bold;">External Source -</span> An Update Row Source that is external to the  system used in the Add Row Source when establishing a relationship.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>SYSTEM TYPE ID</p></td>
<td><p>Displays the System Type used as a basis for the Source. If no System Type is set, a user may be required to set one manually when attempting to map data from this Source to a Target in Map.</p>
<p>A Source data source can be assigned to only one System Type across all Targets. For example, the Source data source of sdbSAP has been assigned to the System Type SAPLEGACY for the Target ttMARA. If the Target ttMAKT also uses the data source of sdbSAP, it cannot use a different System Type such as SAP. The data source sdbSAP must use the System Type SAPLEGACY.</p>
<p>Refer to <a href="../Use_Cases/Sync_Data_Source_System_Types_Across_Targets">Sync Source Data Source-System Types Across all Targets</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Source Type</p></td>
<td><p>Displays the Source Type, which defines the purpose of the Source.</p>
<p>Values are:</p>
<ul>
<li><strong>Add Row</strong> – Source will be used and fields will be converted for loading data into the Target</li>
<li><strong>External Source</strong> – Data will be read from this Source to update fields in the Add Row Source only</li>
<li><strong>{Full Construction}</strong> – Data for all fields will be manually entered for loading into the Target.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Developers</p></td>
<td><p>Click to open the <em>Target Source Contacts</em> page to add Developers to the Source. Developers approve mappings submitted for this Source on the <span style="font-style: italic;"><a href="../../Map/Page_Desc/Mapping_Approval_H">Mapping Approval</a></span> page.</p>
<p>Refer to <a href="../../Map/Use_Cases/Approve_or_Reject_Mappings">Approve or Reject Field Mappings</a> and <a href="../Use_Cases/Add_Developers_and%20Business%20Contacts">Add Developers and Business Contacts to a Target or Source</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Business Contacts</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Target_Source_Contacts">Target Source Contacts</a></span> page to assign Business Contacts to the selected Source. Business Contacts are used for reporting purposes and automatically receive public reports for the Target–Source in Transform.</p>
<p>Refer to <a href="../Use_Cases/Add_Developers_and%20Business%20Contacts">Add Developers and Business Contacts to a Target or Source</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Mapping</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="../../Map/Page_Desc/Field_Mappings_H">Field Mappings</a></span> page to view mappings for the selected Source.</p></td>
</tr>
</tbody>
</table>

 

## <span id="Target_Sources_V"></span>Target Sources V

[Target Sources H](Target_Sources_H_Design)

<span style="font-weight: bold;">NOTE:</span> Fields display on this
page based on the type of Source selected.  If the Source is {Full
Construction}, use this page to [Update Completed Status of Records for
a Construct
Page](../../Construct/Use_Cases/Update_Completed_Status_of_Records).

Field

Description

Drop and Build Data Construction Table and Page

Click to drop the automatically generated page and underlying table and
build it again for the Construct page.

**NOTE**: This field displays for Sources of {Full Construction} only.

**NOTE**: This icon is dimmed until the Target Source is synced to Map.

Update Stats

Click to manually update the status of completed records for the
Construct page.

This field displays for Sources of {Full Construction} only.

Details

Source Data Source

Displays the database that stores the Source tables that contain the
data that will be migrated to the Target.

Click the + icon in this field to open the
<span style="font-style: italic;">Data Source Registry</span> page to
add a data source if necessary.

Data sources should be registered in Common. Refer to [Register a Data
Source in
Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common)
for more information.

System Type ID

Displays the System Type used as a basis for the Source. If no System
Type is set, a user may be required to set one manually when attempting
to map data from this Source to a Target in Map.

A Source data source can be assigned to only one System Type across all
Targets. For example, the Source data source of sdbSAP has been assigned
to the System Type SAPLEGACY for the Target ttMARA. If the Target ttMAKT
also uses the data source of sdbSAP, it cannot use a different System
Type such as SAP. The data source sdbSAP must use the System Type
SAPLEGACY.

Refer to [Sync Source Data Source-System Types Across all
Targets](../Use_Cases/Sync_Data_Source_System_Types_Across_Targets)
for more information.

Description

Displays a brief description of the data source.

Contacts

Functionality

Displays general information about the Source, such as whether it is
from a Mainframe System.

This field is for documentation only.

Manager

Displays information about the manager(s) of this Source, such as  phone
number,  email or emergency contact.

This field is for documentation only.

Technical Contact

Displays a technical contact for the Target Source for documentation
purposes only. This contact is not used in Mapping Approvals or with
Transform reports.

Business Contact

Displays a business contact for the Target Source for documentation
purposes only.

**NOTE:** This contact is not related to the Business Contact added on
the <span style="font-style: italic;">Horizontal</span> View. Unlike
that contact, this contact is not used in Mapping Approvals or with
Transform reports.

Comment

Displays a user-entered comment about the Source.

This field is for documentation purposes only.

Full Construction Details

**NOTE:** This section displays for Sources of {Full Construction} or
for Sources that have had pages built in Construct.

Expected Construction Records

Displays the user estimate of number of records entered manually into
the system.

**NOTE**: This field displays for Sources of {Full Construction} only.

Completed Construction Records

Displays the number of record entered marked as Construction Completed.

Total Construction Records

Displays the number of records entered into the Construction Page.

Construction Page ID

Displays the page name to enter Construction records.

To access the page select Construct \> Objects \> Targets \> page name.

Construct Auto Gen Level

Displays the Construct Auto Gen build view setting. This option controls
whether the *Construct* page is updated or overwritten. Values are:

  - **Off** - Construct objects and pages are not generated.
  - **New** - Adds new fields to the page table and new column
    properties to page. Does not rebuild page views.
  - **Rebuild** - Drops and recreates all views and column properties
    and adds new fields to the page table.

**NOTE:** This field defaults to Rebuild.

Refer to [Use Target Design with Full
Construction](../../Construct/Use_Cases/Use_Target_Design_with_Full_Construction)
for more information.

Construct Auto Gen Build View

Displays the Construct AutoGen build view setting. This option controls
how the Construct page is built with *Horizontal* and *Vertical* Views.

Values are:

  - **Horizontal Only** – All fields are displayed and editable on the
    *Horizontal* View.
  - **Horizontal/Vertical Mix** – Only required fields are displayed and
    editable on the *Horizontal* View. All other fields are on the
    *Vertical* View.
  - **Vertical Only** – Only required fields are displayed on the
    *Horizontal* View. All fields are edited on the *Vertical* View.

The tabs creation and field sorting are controlled by the Application
Screen, Field Order, and Key fields on the [Target
Fields](Target_Fields_H_Target_Design) page’s *Vertical* View.

Refer to [Use Target Design with Full
Construction](../../Construct/Use_Cases/Use_Target_Design_with_Full_Construction)
for more information.
