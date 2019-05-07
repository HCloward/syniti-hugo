+++
title = 'Disposition'
solution = 'Platform'
+++

# Disposition

<div class="use">

Use this page to:

  - [Register External Process
    Validations](../Use_Cases/Register_External_Process_Validations.htm)
  - [Register Stored Procedure
    Validations](../Use_Cases/Register_Stored_Procedure_Validations.htm)
  - [Register View
    Validations](../Use_Cases/Register_View_Validations.htm)
  - [Run Interface Events
    Sequentially](../Use_Cases/Run_Interface_Events_Sequentially.htm)

</div>

To access this page, select **Configuration \> Disposition** in the
*Navigation* pane.

**NOTE:** It is not recommended to add new dispositions or to edit
delivered dispositions; the Automate code would need to be updated for
the disposition to properly work.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>DISPOSITION</p></td>
<td><p>Displays the name of the disposition, which defines what happens next if the event fails the validation rule. Options are:</p>
<ul>
<li><strong>Abort —</strong> Unexpected condition. The event stops running and a workflow email is sent to the Business and Development roles.</li>
<li><strong>Consider Complete —</strong> Expected condition. Even if the event validation rule fails, the event completes and the next event runs.</li>
<li><strong>Retry —</strong> Expected condition. The interface retries the event validation rule until there are no more event validation rule failures.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>COMMENT</p></td>
<td><p>Displays a description of the disposition.</p></td>
</tr>
</tbody>
</table>
