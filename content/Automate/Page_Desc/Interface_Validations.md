# <span id="InterfaceValidationsH"></span> Interface Validations H

[Interface Validations V](#InterfaceValidationsV)

<div class="use">

Use this page to [Register Interface
Validations](../Use_Cases/Register_Interface_Validations.htm).

</div>

To access this page:

1.  Select **Interface** in the *Navigation* pane.
2.  Click the **Validations** icon for the desired interface.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>VALIDATION ID</p></td>
<td><p>Displays a system-generated ID to uniquely identify the validation.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays a value that determines the order in which the validation runs.</p></td>
</tr>
<tr class="even">
<td><p>VALIDATION TYPE</p></td>
<td><p>Displays the type of validation rule for the interface. Options are:</p>
<ul>
<li>External Process</li>
<li>Stored Procedure</li>
<li>View</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>VALIDATION PURPOSE</p></td>
<td><p>Displays why the validation is needed. Options are:</p>
<ul>
<li><strong>Validation –</strong> Interface is not run if the view returns records.</li>
<li><strong>Requirement –</strong> If the view returns a value, then the validation has failed.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>VALIDATION WHEN</p></td>
<td><p>Displays when the validation runs in relation to the event. Options are:</p>
<ul>
<li><strong>Pre –</strong> Validation runs before the event runs.</li>
<li><strong>Post –</strong> Validation runs after the event runs. This option is typically used to determine if an event has run to completion.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>DISPOSITION</p></td>
<td><p>Displays what happens next if the event fails the validation. Options are:</p>
<ul>
<li><strong>Abort –</strong> Unexpected condition. If the validation fails, the interface is turned off, and workflow emails are sent to the business and technical roles.</li>
<li><strong>Consider Complete –</strong> Expected condition. The interface does not retry, the event is considered complete and the next event runs.</li>
<li><strong>Retry –</strong> Expected condition. The interface retries this event/validation until there are no more event validation failures.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the view name as selected from the Validation View, Validation Procedure or Validation Plugin (depending on the Validation Type) on the <em><a href="#InterfaceValidationsV">Vertical</a></em> View.</p></td>
</tr>
<tr class="odd">
<td><p>COMMENT</p></td>
<td><p>Displays description of the validation entered on the <em><a href="#InterfaceValidationsV">Vertical</a></em> View</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If checked, the validation has been tested and is ready to be run.</p>
<p>If unchecked, the validation does not run when the interface is either manually run or set to run on a schedule.</p>
<p>It is checked by default.</p></td>
</tr>
<tr class="odd">
<td><p>OPERATION NAME</p></td>
<td><p>If the External Page is Izzy.IO.CheckForFile, this field displays the file operation that is passed to the FileInterator event.</p>
<p>If the External Page is any other value, this field is blank.</p></td>
</tr>
</tbody>
</table>

 

 

# <span id="InterfaceValidationsV"></span> Interface Validations V

[Interface Validations H](#InterfaceValidationsH)

 

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Validation ID</p></td>
<td><p>Displays a system-generated ID to uniquely identify the validation.</p></td>
</tr>
<tr class="odd">
<td><p>Priority</p></td>
<td><p>Displays a value that determines the order in which the validation runs.</p></td>
</tr>
<tr class="even">
<td><p>Validation Type</p></td>
<td><p>Displays the type of validation rule for the interface. Options are:</p>
<ul>
<li>External Process</li>
<li>Stored Procedure</li>
<li>View</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Validation Purpose</p></td>
<td><p>Displays why the validation is needed. Options are:</p>
<ul>
<li><strong>Validation –</strong> Interface is not run if the view returns records.</li>
<li><strong>Requirement –</strong> If the view returns a value, then the validation has failed.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Validation When</p></td>
<td><p>Displays when the validation runs in relation to the event. Options are:</p>
<ul>
<li><strong>Pre –</strong> Validation runs before the event runs.</li>
<li><strong>Post –</strong> Validation runs after the event runs. This option is typically used to determine if an event has run to completion.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Disposition</p></td>
<td><p>Displays what happens next if the event fails the validation. Options are:</p>
<ul>
<li><strong>Abort –</strong> Unexpected condition. If the validation fails, the interface is turned off, and workflow emails are sent to the business and technical roles.</li>
<li><strong>Consider Complete –</strong> Expected condition. The interface does not retry, the event is considered complete and the next event runs.</li>
<li><strong>Retry –</strong> Expected condition. The interface retries this event/validation until there are no more event validation failures.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Validation Plugin</p></td>
<td><p>Displays the plugin name assigned to the external process validation. The selection populates the NAME field on the <em><a href="#InterfaceValidationsH">Horizontal</a></em> View.</p>
<p><strong>NOTE:</strong> This field only displays for External Process validations.</p></td>
</tr>
<tr class="odd">
<td><p>Validation Procedure</p></td>
<td><p>Displays the registered validation view. Only views ending in “Val” display, as defined by the Validation Filter field on the<em></em><a href="Parameters.htm">Parameters</a> page. The selection populates the NAME field on the <em><a href="#InterfaceValidationsH">Horizontal</a></em> View.</p>
<p><strong>NOTE:</strong> This field only displays for Stored Procedure validations.</p></td>
</tr>
<tr class="even">
<td><p>Validation View</p></td>
<td><p>Displays the registered validation view. The selection populates the NAME field on the <em><a href="#InterfaceValidationsH">Horizontal</a></em> View.</p>
<p><strong>NOTE:</strong> This field only displays for View validations.</p></td>
</tr>
<tr class="odd">
<td><p>Comment</p></td>
<td><p>Displays a description of the validation. Only views ending in “Val” display, as defined by the Validation Filter field on the <em><a href="Parameters.htm">Parameters</a></em> page.</p>
<p><strong>NOTE:</strong> This field only displays for View validations.</p></td>
</tr>
<tr class="even">
<td><p>Active</p></td>
<td><p>If checked, the validation has been tested and is ready to be run.</p>
<p>If unchecked, the validation does not run when the interface is either manually run or set to run on a schedule.</p>
<p>It is checked by default.</p></td>
</tr>
</tbody>
</table>
