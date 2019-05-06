# Add Reserved Columns to Tables

Reserved columns have assigned behaviors and can be added to any table.

The Data Type indicated must be used for the assigned behavior to work
as expected.

This table lists the most commonly used Reserved columns.

<table>
<tbody>
<tr class="odd">
<td><p>Column</p></td>
<td><p>Data Type</p></td>
<td><p>Notes</p></td>
</tr>
<tr class="even">
<td><p>boaStatus</p></td>
<td><p>int</p></td>
<td><ul>
<li>As a best practice, should be added to all page tables to record the event status of a record</li>
</ul>
<p><strong>NOTE</strong>: This column is required if there is an OnValidate event on the page where the DSP® needs to set the status of the field.</p>
<ul>
<li>Can be added to a web view to display the current event status of a record</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>boaAudit</p></td>
<td><p>int</p></td>
<td><ul>
<li>Can be added to a web view to control the accessibility of the Audit column when Audit is set up for that table within the DSP®</li>
<li>Accepts standard Control Status values (0, 1, 2)</li>
</ul></td>
</tr>
<tr class="even">
<td><p>boaAdd</p></td>
<td><p>int</p></td>
<td><ul>
<li>Can be added to a web view to control the ability to add records when Insert is supported for the page</li>
<li>Accepts standard Control Status values (0, 1 ,2)</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>boaEdit</p></td>
<td><p>int</p></td>
<td><ul>
<li>Can be added to a web view to control the ability to edit records when Update is supported for the page</li>
<li>Accepts standard Control Status values (0, 1, 2)</li>
</ul></td>
</tr>
<tr class="even">
<td><p>boaDelete</p></td>
<td><p>int</p></td>
<td><ul>
<li>Can be added to a web view to control the ability to delete records when Delete is supported for the page</li>
<li>Accepts standard Control Status values (0, 1, 2)</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>AddedOn</p></td>
<td><p>smalldatetime</p></td>
<td><ul>
<li>As a best practice should be added to all page tables to record the date and time when the record was added</li>
<li>Generally not included in the web views</li>
</ul></td>
</tr>
<tr class="even">
<td><p>AddedBy</p></td>
<td><p>nvarchar (50)</p></td>
<td><ul>
<li>As a best practice should be added to all page tables to record the UserID who added the record</li>
<li>Generally not included in the web views</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>AddedVia</p></td>
<td><p>nvarchar(50)</p></td>
<td><p>As a best practice should be added to all page tables to record the DSP® process that added the record.</p></td>
</tr>
<tr class="even">
<td><p>ChangedOn</p></td>
<td><p>smalldatetime</p></td>
<td><ul>
<li>As a best practice should be added to all page tables to record the date and time when the record was changed</li>
<li>Generally not included in the web views</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>ChangedBy</p></td>
<td><p>nvarchar (50)</p></td>
<td><ul>
<li>As a best practice should be added to all page tables to record the UserID who changed the record</li>
<li>Generally not included in the web views.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>ChangedVia</p></td>
<td><p>nvarchar(50)</p></td>
<td><p>As a best practice should be added to all page tables to record the DSP® process that changed the record.</p></td>
</tr>
<tr class="odd">
<td><p>LockedBy</p></td>
<td><p>nvarchar (50)</p></td>
<td><ul>
<li>As a best practice should be added to any page table where multiple users are expected to update the same page</li>
<li>This records the UserID of the person currently locking a record (has the record in EDIT mode)</li>
<li>This also prevents the record from being edited by another user at the same time</li>
<li>Generally not included in the web views</li>
</ul></td>
</tr>
<tr class="even">
<td><p>LockedOn</p></td>
<td><p>smalldatetime</p></td>
<td><ul>
<li>As a best practice should be added to any page table where multiple users are expected to update the same page</li>
<li>This records the date and time when a record was locked</li>
<li>Generally not included in the web views</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>WorkflowedOn</p></td>
<td><p>smalldatetime</p></td>
<td><ul>
<li>As a best practice should be added to all page tables to record the date and time when workflow event was executed from this record</li>
<li>Generally not included in the web views</li>
</ul></td>
</tr>
<tr class="even">
<td><p>WorkflowedBy</p></td>
<td><p>nvarchar(50)</p></td>
<td><ul>
<li>As a best practiceshould be added to all page tables to record the UserID who executed the workflow event from this record</li>
<li>Generally not included in the web views</li>
</ul></td>
</tr>
</tbody>
</table>
