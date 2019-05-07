+++
title = 'Business Process (Scenarios)'
solution = 'Master Data Management'
+++

# Business Process (Scenarios)

<div class="use">

Use this page to [Add a Scenario to a Business
Process](../Use_Cases/Add_a_Scenario_to_a_Business_Process.htm).

</div>

To access this page:

1.  Select **dspConduct \> Design** in the *Navigation* pane.
2.  Click the **Business Processes** icon for a category.
3.  Click the <span style="font-weight: bold;">Scenarios</span> icon.

**NOTE:** If a scenario was assigned to a business process and imported
from IGC™, data that was entered in IGC™ cannot be updated from within
dspConduct™, and many of the fields and icons associated with the record
are not active for that business process scenario. Refer to [Update
Custom Attributes for Governance
Elements](../Use_Cases/Update_Custom_Attributes_for_Governance_Elements.htm)
for more information.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>From IGC</p></td>
<td><p>Displays to indicate that the scenario was assigned to the business process in IGC™.</p>
<p>This column displays after the IGC™ parameters are configured in Common on initial install. Refer to the <em>BackOffice Associates® Installation and Upgrade Manual</em> for more information.</p>
<p><strong>NOTE</strong>: Data entered in IGC™ cannot be updated from within dspConduct™.</p>
<p><strong>NOTE</strong>: Records that come from IGC™ cannot be deleted.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order in which the scenario is processed within the business process.</p>
<p><strong>NOTE</strong>: If the business process scenario was imported from IGC™, the priority is set to 100 by default for the initial business process scenario, then incremented by 10 for each successive business process scenario. A user can update this value as needed.</p></td>
</tr>
<tr class="even">
<td><p>SCENARIO ID</p></td>
<td><p>Displays the scenario ID and description. Click the link to open the <em><a href="Scenario_H.htm">Scenario</a></em> page to display details about the scenario.</p>
<p>When adding scenarios to a business process, if a scenario is not in the list box, the user can click the <strong>Click to add a new item</strong> link to open the <em>Scenario</em> page in another browser tab. Refer to <a href="../Use_Cases/Add_Scenario.htm">Add a Scenario</a> for more information.</p>
<p>One or more different scenarios can be added to a business process. A particular scenario can only be added to a business process once.</p>
<p>A scenario from a different category than the business process’s parent category can be added as long as it is not assigned the lowest priority in the business process. It also cannot be a dependent of any other scenarios in its parent category.</p>
<p>Refer to <a href="../Use_Cases/Allow_a_Scenario_to_be_used_in_Other_Categories.htm">Allow a Scenario to be used in other Categories</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Role SLA</p></td>
<td><p>Click to open the <a href="Business_Process_Scenario_Roles.htm">Business Process (Scenario Roles)</a> page to configure SLA settings at the business process scenario role level.</p>
<p>Refer to <a href="../Config/Configure_SLA_Settings_at_the_BPSR_Level.htm">Configure SLA settings at the Business Process Scenario Role Level</a> for more information.</p></td>
</tr>
</tbody>
</table>
