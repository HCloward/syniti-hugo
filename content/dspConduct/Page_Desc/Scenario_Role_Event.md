+++
title = 'Scenario Role Event'
solution = 'Data Quality'
+++

# Scenario Role Event

<div class="use">

Use this page to [add a custom business
rule](../Use_Cases/Add_Custom_Business_Rules.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspConduct
    \></span>**Design** in the *Navigation* pane.
2.  Click the **Scenarios** icon.
3.  Click the **Roles** icon for a scenario.
4.  Click the **Events** icon for a role.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>EVENT ID</p></td>
<td><p>Displays the name of the event to which custom business rules are registered. Values are:</p>
<ul>
<li><strong>TaskID</strong> rules run when the Task ID button is clicked on the <a href="Request_Role_Task.htm">Request Role Task</a> page to access a Content page for entering or updating request data.</li>
</ul>
<p><strong>NOTE:</strong> The TaskID should not be an expected parameter of the custom rule. Custom rules registered at this level are not specific to a particular content page. Rules specific to a particular page must be registered to that content page.</p>
<ul>
<li><strong>Validate</strong> rules execute when the Validate button is clicked on the <span style="font-style: italic;"><a href="Request_Role_H.htm">Request Role</a></span> page for any role.</li>
<li><strong>Finish</strong> rules run when the Finish button is clicked on the <span style="font-style: italic;">Request Role</span> page for the Application role or Post role, or when the Approve button is clicked for the Review role.</li>
<li><strong>FinalFinish</strong> rules run when the FinalFinish event executes for the Post Role.</li>
<li><strong>Reset</strong> rules run when the Reset button is clicked on the <span style="font-style: italic;">Request Role</span> page for the Application role or the Reject button for the Review role.</li>
<li><strong>ForegroundPost</strong> rules run before the Integrate posting adapter is called.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Rules</p></td>
<td><p>Click to open the <em><a href="Scenario_Role_Event_Rule.htm">Scenario Role Event Rule</a></em> page to add, edit and delete rules registered to the scenario role combination that run when specified request-level event occurs.</p></td>
</tr>
</tbody>
</table>
