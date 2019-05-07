+++
title = 'Plugin Validation Rules'
solution = 'Platform'
+++

# Plugin Validation Rules

<div class="use">

Use this page to [View Where Plugin is Used within the
DSP](../Use_Cases/View%20Where%20Plugin%20is%20Used.htm).

</div>

To access this page:

1.  Select **Admin \> WebApps** in the *Navigation* pane.

2.  Click the **Plugins** icon for the desired WEBAPP NAME.

3.  Click the **Plugins** icon for the desired RELATIVE ASSEMBLY PATH.

4.  Click the**Validation Rules** icon for the desired PLUGIN NAME
    DESCRIPTION.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>WEB APP NAME</p></td>
<td><p>Displays the name of the WebApp where the validation rule resides.</p></td>
</tr>
<tr class="odd">
<td><p>PAGE NAME</p></td>
<td><p>Displays the page name within the WebApp where the validation rule runs.</p></td>
</tr>
<tr class="even">
<td><p>EVENT NAME</p></td>
<td><p>Displays the event that runs on the page. </p></td>
</tr>
<tr class="odd">
<td><p>EVENT DESCRIPTION</p></td>
<td><p>Displays a brief description of the event.</p></td>
</tr>
<tr class="even">
<td><p>SEVERITY</p></td>
<td><p>Displays the severity level for the validation rule. Options are:</p>
<ul>
<li><p><strong>Error –</strong> If the record fails this validation, that status is marked as Invalid.</p></li>
<li><p><strong>Message –</strong> Used as an informative validation rule that works the same as other severities, but does not negatively affect the validity of the record itself. For example, failing a message will not fail the record validation.</p></li>
<li><p><strong>Warning –</strong> If the record fails this type of validation, the user must determine whether to pass or fail the record by clicking Yes or No when prompted.</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p>CONDITIONAL COLUMN</p></td>
<td><p>Displays a column on the Horizontal View or the Vertical View that controls whether or not the validation rule is enabled.</p></td>
</tr>
<tr class="even">
<td><p>IS ACTIVE</p></td>
<td><p>If checked, the validation rule runs for the event.</p>
<p>If unchecked, the validation rule does not run for the event. </p></td>
</tr>
</tbody>
</table>
