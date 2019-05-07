+++
title = 'Update Custom Attributes for Governance Elements'
solution = 'Master Data Management'
+++

# Update Custom Attributes for Governance Elements

Data entered in IGC™ and imported into dspConduct™ cannot be updated in
dspConduct™. Records cannot be deleted, and elements cannot be activated
or deactivated.

Additionally, a governance hierarchy imported from the IGC™ cannot have
elements added or deleted (e.g., a Designer cannot add a scenario in
dspConduct™ to a business process that was added in IGC™).

Some settings that are not set in IGC™ can be updated for IGC™ elements
in dspConduct™.

**NOTE**: A Process Designer must assign an owner in dspConduct™ to any
roles, scenarios, business processes or categories that were added in
IGC™.

**NOTE**: By default, the initial business process scenario imported
from IGC™ has a priority of 100. The priority of each subsequent
business process scenario is incremented by 10. A user can update this
value as needed.

**NOTE**: When a role is imported from IGC™ and the SLA fields are blank
in dspConduct™, the values entered in IGC™ are used at the scenario role
level and the business process scenario role level. If the fields
already contain values in dspConduct™, the SLA values are not updated at
these levels. At the role level, the SLA values are updated when a role
is imported from IGC™ with SLA data whether the fields have values in
dspConduct™ or not.

Governance elements added in IGC™ are not used in dspConduct™ to create
new business processes. For example, a role added in IGC™ cannot be used
in a scenario added in dspConduct™.

**NOTE**:All IGC™ elements can be copied as the basis for a new element
that can be used in dspConduct™.

The following settings and features are available to update for IGC™
elements in dspConduct™.

<table>
<tbody>
<tr class="odd">
<td><p>IGC™ Governance Element</p></td>
<td><p>Editable Settings in dspConduct™</p></td>
</tr>
<tr class="even">
<td><p>Category</p></td>
<td><ul>
<li>WebApp ID</li>
<li>Owner</li>
</ul>
<p><strong>NOTE:</strong> The fields above are required and must be set in dspConduct™.</p>
<ul>
<li>Request Page ID</li>
<li>Control Table Prefix</li>
<li>Condition Table Datasource Id</li>
<li>Audit Datasource Id</li>
<li>Posting Processes</li>
<li>Data Driven Dependency conditions</li>
<li>Default Value Rules</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Business Process</p></td>
<td><ul>
<li>Owner</li>
</ul>
<p><strong>NOTE:</strong> The field above is required and must be set in dspConduct™.</p>
<ul>
<li>Element Documentation</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Business Process Scenario</p></td>
<td><p>Priority</p></td>
</tr>
<tr class="odd">
<td><p>Business Process Scenario Role</p></td>
<td><ul>
<li>Work Days</li>
<li>Work Hours</li>
<li>Work Minutes</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Scenario</p></td>
<td><ul>
<li>Scenario dependencies</li>
<li>Posting Processes</li>
<li>Default Rules</li>
<li>Element Documentation</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Scenario Role</p></td>
<td><ul>
<li> Work Days</li>
<li>Work Hours</li>
<li>Work Minutes</li>
<li>Auto Finish Role</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Role</p></td>
<td><ul>
<li>Auto Finish Role</li>
<li>Auto Post Role</li>
<li>Scheduled Post Allowed</li>
<li>Auto Extend Display</li>
<li>Priority</li>
<li>Send Workflow</li>
<li>Element Documentation</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Task</p></td>
<td><ul>
<li>Variants</li>
<li>Final Finish Tables</li>
<li>Element Documentation</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Role Tasks</p></td>
<td><ul>
<li>Priority</li>
<li>Read Only</li>
</ul>
<p><strong>NOTE:</strong> Though it can be edited, the Read Only field is not generally updated for IGC™ elements.</p></td>
</tr>
</tbody>
</table>

<div>

-----

</div>
