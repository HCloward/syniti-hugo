+++
title = 'Construct Object'
solution = 'Migration'
+++

# Construct Object

<div class="use">

Use this page to [View the Construction Page in
Construct](../Use_Cases/View_the_Construction_page_in_Construct.htm).

</div>

To access this page:

1.  Select **dspMigrate** in the *Navigation* pane.
2.  Select <span style="font-weight: bold;">Construct </span>in the
    Context bar.
3.  Click the <span style="font-weight: bold;">Objects</span>icon on the
    *[Construct Launch](Construct_Launch.htm)* page.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>OBJECT NAME</p></td>
<td><p>Displays the name of the Object that contains Targets to which Construct pages are added.</p>
<p>Objects are added in Console.</p></td>
</tr>
<tr class="odd">
<td><p>OBJECT DESCRIPTION</p></td>
<td><p>Displays a description of the Object as added in Console.</p></td>
</tr>
<tr class="even">
<td><p>COMPLETED RECORDS</p></td>
<td><p>Displays the number of completed records for all Targets in the Object. Records are complete based on client-specific requirements enforced by stored procedures registered to the Construct page to update the boaConstructComplete bit field. boaConstructComplete = 1 means that the record is considered complete.</p></td>
</tr>
<tr class="odd">
<td><p>TOTAL RECORDS</p></td>
<td><p>Displays the total number of fields in the Source data source for the Source table for all Targets in the Object.</p></td>
</tr>
<tr class="even">
<td><p>EXPECTED RECORDS</p></td>
<td><p>Displays the total number of estimated fields to be completed (as in, the number of active fields in the Target) for all Targets in the Object. This is added in Target Design for Full Construction types only on the vertical view of the Target Sources page for a Source of {Full Construction}.</p></td>
</tr>
<tr class="odd">
<td><p>Targets</p></td>
<td><p>Click to open the <em><a href="Construct_Target.htm">Construct Target</a></em> page to view each of the Targets that have Construct pages and the status of construction for each Target.</p></td>
</tr>
<tr class="even">
<td><p>Construct Pages</p></td>
<td><p>Click to open the <em><a href="Construct_Page.htm">Construct Page</a></em> page to view all of the Construct pages that have been added for the Object.</p></td>
</tr>
</tbody>
</table>
