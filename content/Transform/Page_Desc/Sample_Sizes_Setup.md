# Sample Sizes (Setup)

<div class="use">

Use this page to [Configure Sample
Size.](../Config/Configure_Sample_Size.htm)

</div>

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).

2.  Select **Configuration \> Setup \> Sampling Methods(Setup)** in the
    *Navigation* pane.

3.  Click the **Sample Size** icon next to the sampling method you want
    to use. For example, ANSI/ASQC Z1.4 GI I or Square Root.
    
    **NOTE:** This is the method used in Transform if it meets auditing
    requirements.
    
    **NOTE:** Using the number of records in your table, locate the
    range that it falls between. The sample size will determine how many
    sample records will be returned.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>RANGE LOW</p></td>
<td><p>Displays the lowest number in the range used to identify the sample size. This value is part of the sampling method used to determine the sample size, or number of rows from the target table to be selected at random for quality verification before or after a data load.</p>
<p>For example, if 300 is entered and there are 500 records in the table being audited, this sampling would be available for use as long as the number 500 does not exceed Range High.</p></td>
</tr>
<tr class="odd">
<td><p>RANGE HIGH</p></td>
<td><p>Displays the highest number in the range used to identify the sample size. This value is part of the sampling method used to determine the sample size, or number of rows from the target table to be selected at random for quality verification before or after a data load.</p>
<p>For example, if 1000 is entered and there are 500 records in the table being audited, this sampling would be available for use as long as the number 500 is not lower than Range Low.</p></td>
</tr>
<tr class="even">
<td><p>SAMPLE SIZE</p></td>
<td><p>Displays the number of records produced for the sample.</p></td>
</tr>
<tr class="odd">
<td><p>COMMENT</p></td>
<td><p>Displays user-entered comments about the sample size.</p></td>
</tr>
</tbody>
</table>
