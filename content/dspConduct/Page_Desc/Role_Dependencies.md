+++
title = 'Role Dependencies'
solution = 'Master Data Management'
+++

# Role Dependencies

<div class="use">

Use this page to [Add Dependencies to
Roles](../Use_Cases/Role_Dependencies.htm#Add_Dependencies_to_Roles).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspConduct
    \></span><span style="font-weight: bold;">Design</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    category.
3.  Click the <span style="font-weight: bold;">Dependencies</span> icon
    for a role.

**NOTE:** If a role dependency was imported from IGC™, data that was
entered in IGC™ cannot be updated from within dspConduct™, and many of
the fields and icons associated with the record are not active for that
role dependency. Refer to [Update Custom Attributes for Governance
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
<td><p>Displays to indicate that the role dependency was created in IGC™.</p>
<p>This column displays after the IGC™ parameters are configured in Common on initial install. Refer to the <em>BackOffice Associates® Installation and Upgrade Manual</em> for more information.</p>
<p><strong>NOTE</strong>: Data entered in IGC™ cannot be updated from within dspConduct™.</p>
<p><strong>NOTE</strong>: Records that come from IGC™ cannot be deleted.</p>
<p><strong>NOTE</strong>: When an IGC™ business process is imported into dspConduct™, the business process, scenario and role dependencies are also imported.</p></td>
</tr>
<tr class="odd">
<td><p>DEPENDENT ROLE ID</p></td>
<td><p>Displays the name of the role that must be finished before the current role can start.  For example, the Review role must have all the Application roles listed as dependent roles. The Review role cannot start until work on the Application roles is complete.</p>
<p>Refer to <a href="../Use_Cases/Role_Dependencies.htm#Dependencies_and_Role_Types">Dependencies and Role Types</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Conditions</p></td>
<td><p>Click to open the <a href="Role_Depend_Cond_Assin_Page.htm">Role Dependency Condition Assignment</a> page to configure data driven dependencies if needed.</p>
<p>Refer to <a href="../Use_Cases/Role_Dependencies.htm#Assign_a_Condition_to_a_Role_Dependency_Relationship">Assign a Condition to a Role Dependency Relationship</a> more information.</p></td>
</tr>
</tbody>
</table>
