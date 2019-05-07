+++
title = 'Mapping Approval H <span id="top"></span>'
solution = 'Migration'
+++

# Mapping Approval H <span id="top"></span>

[Mapping Approval V](#MappingV)

<div class="use">

Use this page to [Approve or Reject
Mappings](../Use_Cases/Approve_or_Reject_Mappings.htm).

</div>

To access this page, click the green
<span style="font-weight: bold;">Mapping Approval</span> tab on the
Quick Panel.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Approve</p></td>
<td><p>Click to Approve the selected mapping (s).</p></td>
</tr>
<tr class="odd">
<td><p>Complete</p></td>
<td><p>Click to approve the mapping and set the Mapping Status and Rule Status for the selected mapping to Complete.</p>
<p>When a mapping is approved, the Rule Status is set to In Process by default. If a user clicks Complete, the Rule Status bypasses the In Process status. The rule can then be created in SQL AutoGen.</p></td>
</tr>
<tr class="even">
<td><p>Reject</p></td>
<td><p>Click to Reject the selected mapping(s) after a rejection reason has been saved in the Comment field on the <em><a href="#">Mapping Approval</a></em> page’s <em>Vertical</em> View.</p>
<p><strong>NOTE:</strong> If the mapping action is Rule or RuleXref, the Rule SQL field must also have been completed with the correct SQL for the rule.</p></td>
</tr>
<tr class="odd">
<td><p>Download List</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Mapping_Approvals_Download_List.htm">Mapping Approvals Download List</a></span> page to download all mappings waiting for review into an Excel file or a Word document.</p></td>
</tr>
<tr class="even">
<td><p>Wave NAME</p></td>
<td><p>Displays the name of the Wave as created in Console that contains the Process Area and Object where the new or changed field mapping resides.</p></td>
</tr>
<tr class="odd">
<td><p>Process Area</p></td>
<td><p>Displays the name of the Process Area as created in Console that contains the Object where the new or changed field mapping resides.</p></td>
</tr>
<tr class="even">
<td><p>OBJECT</p></td>
<td><p>Displays the name of the Object as created in Console where the new or changed field mapping resides.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET</p></td>
<td><p>Displays the Target table name where the data that is mapped will reside.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE</p></td>
<td><p>Displays the Source table name where the data used in the mapping originates.</p></td>
</tr>
<tr class="odd">
<td><p><span id="Mapping Actions" class="popUpLink">ACTION</span></p></td>
<td><p>Displays the action used in the mapping.</p></td>
</tr>
<tr class="even">
<td><p>Approved</p></td>
<td><p>If checked, the selected mapping has been approved by a Developer on this page.</p>
<p>If unchecked, the mapping is waiting for Developer review.</p></td>
</tr>
</tbody>
</table>

## <span id="MappingV"></span>Mapping Approval V

[Mapping Approval H](#top)

<div class="use">

Use this page to [Approve or Reject
Mappings](../Use_Cases/Approve_or_Reject_Mappings.htm).

</div>

|                                                            |                                                                                                                                                                                                                  |
| ---------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                                                      | Description                                                                                                                                                                                                      |
| Wave Name                                                  | Displays the name of the Wave as created in Console that contains the Process Area and Object where the new or changed field mapping resides.                                                                    |
| Process Area                                               | Displays the name of the Process Area as created in Console that contains the Object where the new or changed field mapping resides.                                                                             |
| Object                                                     | Displays the name of the Object as created in Console where the new or changed field mapping resides.                                                                                                            |
| Target                                                     | Displays the Target table name where the data that is mapped will reside.                                                                                                                                        |
| Source                                                     | Displays the Source table name where the data used in the mapping originates.                                                                                                                                    |
| <span id="Mapping Actions" class="popUpLink">Action</span> | Displays the action used in the mapping.                                                                                                                                                                         |
| Description                                                | Displays details about the mapping, including field name, mapping group, and rule name.                                                                                                                          |
| Comment                                                    | Enter the rejection reason when rejecting a mapping.                                                                                                                                                             |
| Rule SQL                                                   | Enter the SQL for the field mapping if the Action is Rule or RuleXref. This field must be completed if a field mapping is to be rejected. This field only displays when the mapping action is Rule or RuleXref.. |
| Mapped By                                                  | Displays the Mapper’s name.                                                                                                                                                                                      |
