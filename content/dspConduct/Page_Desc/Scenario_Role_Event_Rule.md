+++
title = 'Scenario Role Event Rule'
solution = 'Data Quality'
+++

# Scenario Role Event Rule

<div class="use">

Use this page to [add a custom business
rule](../Use_Cases/Add_Custom_Business_Rules.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Design** in the *Navigation* pane.
2.  Click the **Scenarios** icon for a category on the Category page.
3.  Click the **Roles** icon for a scenario.
4.  Click the **Events** icon for a role.
5.  Click the **Rules** icon for an event.

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
<td><p>PRIORITY</p></td>
<td><p>Displays priority in which the rule is run when the event occurs, if there is more than one rule registered for the event.</p></td>
</tr>
<tr class="odd">
<td><p>DATA SOURCE ID</p></td>
<td><p>Displays data source in which the rule is stored.</p></td>
</tr>
<tr class="even">
<td><p>RULE</p></td>
<td><p>Displays name of the rule that is executed when the event occurs. The rule is a stored procedure in the data source.</p>
<p><strong>NOTE</strong>: When adding a custom business rule, the Designer selects the rule from a list of stored procedures from the selected data source. These stored procedures can only accept the inputs RequestID and RoleID.</p></td>
</tr>
</tbody>
</table>
