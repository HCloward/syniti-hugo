+++
title = 'Scenario H'
solution = 'Master Data Management'
+++

# Scenario H

[Scenario V](#Scenario_V)

<div class="use">

Use this page to:

  - [Add a Scenario](../Use_Cases/Add_Scenario.htm)
  - [Deactivate a Scenario](../Use_Cases/Deactivate_Scenario.htm)
  - [Add a Role to a
    Scenario](../Use_Cases/Add_a_Role_to_a_Scenario.htm)
  - [Add a Dependent Scenario to a
    Scenario](../Use_Cases/Add_a_Dependent_Scenario.htm)
  - [Add a Process to a
    Scenario](../Use_Cases/Add_an_Integrate_Process_to_a_Scenario.htm)

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspConduct
    \></span><span style="font-weight: bold;">Design</span> in the
    <span style="font-style: italic;">Navigation</span> pane; the
    <span style="font-style: italic;">Category</span> page displays.
2.  Click the **Scenario** icon for the category.

**NOTE:** If a scenario was created and imported from IGC™, data that
was entered in IGC™ cannot be updated from within dspConduct™, and many
of the fields and icons associated with the record are not active for
that scenario. Refer to [Update Custom Attributes for IGC™ Governance
Elements in
dspConduct™](../Use_Cases/Update_Custom_Attributes_for_Governance_Elements.htm)
for more information.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>From IGC</p></td>
<td><p>Displays to indicate that the scenario was created in IGC™.</p>
<p>This column displays after the IGC™ parameters are configured in Common on initial install. Refer to the <em>BackOffice Associates® Installation and Upgrade Manual</em> for more information.</p>
<p><strong>NOTE</strong>: Data entered in IGC™ cannot be updated from within dspConduct™.</p>
<p><strong>NOTE</strong>: Records that come from IGC™ cannot be deleted.</p></td>
</tr>
<tr class="odd">
<td><p>Activate</p></td>
<td><p>Click to activate one or more scenarios selected on the page.</p>
<p>Activated scenarios can be assigned to business processes.</p></td>
</tr>
<tr class="even">
<td><p>Deactivate</p></td>
<td><p>Click to deactivate one or more scenarios selected on the page.</p>
<p>Deactivated scenarios are not available to be assigned in a business process.</p></td>
</tr>
<tr class="odd">
<td><p>NAME</p></td>
<td><p>Displays the scenario name.</p>
<p>The scenario name must be unique within a category.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays the description of the scenario.</p></td>
</tr>
<tr class="odd">
<td><p>TYPE</p></td>
<td><p>Displays the type of scenario.</p>
<p>Values are:</p>
<ul>
<li><strong>Create</strong> - Creates new business objects, such as materials, customers, vendors, profit centers, GL accounts, etc.</li>
<li><strong>Change</strong> - Updates the data in a logical way for an existing business object, such as by material group (Basic Data) for an existing material, pricing procedure (Sales Data) for an existing customer or incoterms (Purchasing Data) for an existing vendor.</li>
<li><strong>BusinessExtend</strong> - Makes a new business object that is associated with an existing business object, such as a new BOM (Bill of Material) for an existing material, a new ship-to for an existing customer or a new order from address for an existing vendor.</li>
<li><strong>OrganizationalExtend</strong> - Extends an existing business object to one or more Org Units, such as an existing material to a new plant, an existing customer to a new sales organization or company or an existing vendor to a new purchasing organization or company.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the scenario can be used in a business process. If disabled the scenario cannot be used in a business process.</p>
<p>To enable or disable multiple scenarios, select the rows, and then click the Deactivate or Activate icon on the toolbar.</p>
<p><strong>NOTE:</strong> The scenario can be disabled regardless of the status by disabling the ACTIVE check box. However, If the scenario is used within an active business process, it cannot be disabled.</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE IN BUSINESS PROCESSES</p></td>
<td><p>Indicates whether the scenario is currently active within a business process.</p>
<p>If the scenario is active within a business process, it cannot be disabled, changed or deleted.</p>
<p><strong>NOTE:</strong> Hover over the indicator to see the number of business processes in which the scenario is active.</p></td>
</tr>
<tr class="even">
<td><p>STATUS</p></td>
<td><p>Displays the status of the scenario.</p>
<p>Values are:</p>
<ul>
<li><strong>In Design</strong> - Scenario is being changed.</li>
<li><strong>Design Complete</strong> - Scenario changes are complete but have not been approved.</li>
<li><strong>Pending Approval</strong> - Scenario changes are awaiting Approval.</li>
<li><strong>Design Rejected</strong> - Scenario changes have been rejected.</li>
<li><strong>Design Approved</strong> - Scenario changes have been completed and have been approved.</li>
<li><strong>Published</strong> - Scenario changes have been approved, and the scenario is available for use.</li>
</ul>
<p><strong>NOTE</strong>: All scenarios imported from IGC™ have a status of Published. No other statuses can be set.</p>
<p><strong>NOTE:</strong> If the scenario is in any status other than Published, the Designer can activate or deactivate the process in Integrate as needed to test and troubleshoot the process. Refer to <a href="../../../Platform/Integrate/Use_Cases/Manage_Processes.htm">Manage Processes</a> and <a href="../../../Platform/Integrate/Use_Cases/Activate_the_Process.htm">Activate the Process</a> for more information about working with processes in Integrate.</p></td>
</tr>
<tr class="odd">
<td><p>Roles</p></td>
<td><p>Click to open the <a href="Scenarios_Roles_H.htm"><em>Scenario (Roles)</em></a> page to add roles to a scenario. Refer to <a href="../Use_Cases/Add_a_Role_to_a_Scenario.htm">Add a Role to a Scenario</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Dependencies</p></td>
<td><p>Click to open the <em><a href="Scenarios_Dependencies.htm">Scenario (Dependencies)</a></em> page to add dependent scenarios. Refer to <a href="../Use_Cases/Add_a_Dependent_Scenario.htm">Add a Dependent Scenario to a Scenario</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Processes</p></td>
<td><p>Click to open the <em><a href="Scenario_Process.htm">Scenario Process</a></em> page to add Integrate processes. Refer to <a href="../Use_Cases/Add_an_Integrate_Process_to_a_Scenario.htm">Add a Process to a Scenario</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Default Rules</p></td>
<td><p>Click to open the <a href="Scenario_Default_Rules.htm">Scenario (Default Rules)</a> page to assign a default value rule at the scenario level. Refer to <a href="../Use_Cases/Assign_a_Default_Value_Rule_to_a_Scenario.htm">Assign a Default Value Rule to a Scenario</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Where Used</p></td>
<td><p>Click to open the <span style="font-style: italic;">Where Used – Scenario</span> page to view the tasks and roles that are part of the scenario, including a count of active and inactive tasks and roles.</p></td>
</tr>
<tr class="even">
<td><p>Scenario Report</p></td>
<td><p>Click to open the <span style="font-style: italic;">Element Report Frame</span> page that displays basic information about the scenario; default value rules associated with the scenario (if applicable); dependent scenarios (if applicable); information about each role used in the scenario (dependencies and conflicts, tasks, and positions); and the Integrate process used to post requests for the scenario.</p></td>
</tr>
</tbody>
</table>

## <span id="Scenario_V"></span>Scenario V

[Scenario H](Scenario_H.htm)

This page contains the following tabs:

  - [General](#General)
  - [Copy Options](#Copy_Options)

## <span id="General"></span>General

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Name</p></td>
<td><p>Displays the scenario name.</p>
<p>The scenario name must be unique within a category.</p></td>
</tr>
<tr class="odd">
<td><p>Description</p></td>
<td><p>Displays the description of the scenario.</p></td>
</tr>
<tr class="even">
<td><p>Owner</p></td>
<td><p>Displays the owner of the scenario.</p>
<p><strong>NOTE:</strong> Owner defaults to the parent category owner. A different owner can be selected.</p></td>
</tr>
<tr class="odd">
<td><p>Status</p></td>
<td><p>Displays the status of the scenario.</p>
<p>Values are:</p>
<ul>
<li><strong>In Design</strong> - Scenario is being changed.</li>
<li><strong>Design Complete</strong> - Scenario changes are complete but have not been approved.</li>
<li><strong>Pending Approval</strong> - Scenario changes are awaiting Approval.</li>
<li><strong>Design Rejected</strong> - Scenario changes have been rejected.</li>
<li><strong>Design Approved</strong> - Scenario changes have been completed and have been approved.</li>
<li><strong>Published</strong> - Scenario changes have been approved, and the scenario is available for use.</li>
</ul>
<p><strong>NOTE:</strong> If the scenario is in any status other than Published, the Designer can activate or deactivate the process in Integrate as needed to test and troubleshoot the process. Refer to <a href="../../../Platform/Integrate/Use_Cases/Manage_Processes.htm">Manage Processes</a> and <a href="../../../Platform/Integrate/Use_Cases/Activate_the_Process.htm">Activate the Process</a> for more information about working with processes in Integrate.</p></td>
</tr>
<tr class="even">
<td><p>Active</p></td>
<td><p>If enabled, the scenario can be used in a business process. If disabled the scenario cannot be used in a business process.</p>
<p><strong>NOTE:</strong> The scenario can be disabled regardless of the status by disabling the ACTIVE check box. However, If the scenario is assigned to an active business process, it cannot be disabled.</p></td>
</tr>
<tr class="odd">
<td><p>Type</p></td>
<td><p>Displays the type of scenario.</p>
<ul>
<li>Values are:</li>
<li><strong>Create</strong> - Creates new business objects, such as materials, customers, vendors, profit centers, GL accounts, etc.</li>
<li><strong>Change</strong> - Updates the data in a logical way for an existing business object, such as by material group (Basic Data) for an existing material, pricing procedure (Sales Data) for an existing customer or incoterms (Purchasing Data) for an existing vendor.</li>
<li><strong>BusinessExtend</strong> - Makes a new business object that is associated with an existing business object, such as a new BOM (Bill of Material) for an existing material, a new ship-to for an existing customer or a new order from address for an existing vendor.</li>
<li><strong>OrganizationalExtend</strong> - Extends an existing business object to one or more Org Units, such as an existing material to a new plant, an existing customer to a new sales organization or company or an existing vendor to a new purchasing organization or company.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Child Scenario Criteria</p></td>
<td><p>Displays the org unit to be used to create child requests for the scenario.</p>
<p>Refer to <a href="../Use_Cases/Configure_Child_Scenario_Criteria.htm">Configure Child Scenario Criteria</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Use In Other Category</p></td>
<td><p>Click to open the <em><a href="Scenario_Use_in_Other_Category.htm">Scenario Use In Other Category</a></em> page. Refer to <span><a href="../Use_Cases/Allow_a_Scenario_to_be_used_in_Other_Categories.htm">Allow a Scenario to be used in other Categories</a></span> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Documentation</p></td>
<td><p>Click to open the <em><a href="Element_Documentation.htm">Element Documentation</a></em> page to upload or download documentation regarding the scenario.</p>
<p>Refer to <a href="../Use_Cases/Upload_Documentation_at_the_Scenario_Role_Level.htm">Upload Documentation at the Scenario Role Level</a>  for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Default Rules</p></td>
<td><p>Click to open the <a href="Scenario_Default_Rules.htm">Scenario (Default Rules)</a> page to assign a default value rule at the scenario level. Refer to <a href="../Use_Cases/Assign_a_Default_Value_Rule_to_a_Scenario.htm">Assign a Default Value Rule to a Scenario</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Where Used</p></td>
<td><p>Click to open the <em>Where Used – Scenario</em> page to view the tasks and roles that are part of the scenario, including a count of active and inactive tasks and roles.</p></td>
</tr>
<tr class="odd">
<td><p>Scenario Report</p></td>
<td><p>Click to open the <span style="font-style: italic;">Element Report Frame</span> page that displays basic information about the scenario; default value rules associated with the scenario (if applicable); dependent scenarios (if applicable); information about each role used in the scenario (dependencies and conflicts, tasks, and positions); and the Integrate process used to post requests for the scenario.</p></td>
</tr>
<tr class="even">
<td><p>Comment</p></td>
<td><p>Displays comments regarding the scenario.</p></td>
</tr>
</tbody>
</table>

## <span id="Copy_Options"></span>Copy Options

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>New Scenario Name</p></td>
<td><p>Displays the name of the new scenario created as a result of copying the selected scenario.</p>
<p>The new scenario name must be unique.</p></td>
</tr>
<tr class="odd">
<td><p>Copy</p></td>
<td><p>Click to create a copy of the selected scenario.</p></td>
</tr>
</tbody>
</table>
