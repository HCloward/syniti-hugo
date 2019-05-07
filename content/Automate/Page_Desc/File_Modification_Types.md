+++
title = 'File Modification Types'
solution = 'Platform'
+++

# File Modification Types

<div class="use">

Use this page to [Add Logical
Paths](../Use_Cases/Add_Logical_Paths.htm).

</div>

To access this page, select **IO Config \> File Format Types** in the
*Navigation* pane.

**NOTE:** It is not recommended to add new file modification types or to
edit the delivered file modification types; the Automate code would need
to be updated for the file modification type to properly work.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>FILE MODIFICATION</p></td>
<td><p>Displays the descriptions of the file modification types. Options are:</p>
<ul>
<li><strong>Batched —</strong> When the files are copied to the destination, they are broken into files with the amount of record noted in the Batch Size field (on the <em>Vertical</em> View of the <em><a href="Logical_Paths.htm#LogicalPathsV">Logical Paths</a></em> page).</li>
<li><strong>SegmentByField —</strong> When the files are written to the destination, a file is created for each unique value in the Segment Field (configured on the <em>Vertical</em> View of the <em><a href="Logical_Paths.htm#LogicalPathsV">Logical Paths</a></em> page).</li>
<li><strong>None —</strong> File is not modified. This is the recommended selection when moving files from one folder to another.</li>
</ul></td>
</tr>
</tbody>
</table>
