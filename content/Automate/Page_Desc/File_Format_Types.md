+++
title = 'File Format Types'
solution = 'Platform'
+++

# File Format Types

<div class="use">

Use this page to [Add Logical
Paths](../Use_Cases/Add_Logical_Paths).

</div>

To access this page, select **IO Config \> File Modification Types** in
the *Navigation* pane.

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
<td><p>FILE FORMAT</p></td>
<td><p>Displays the names of the file formats. Options are:</p>
<ul>
<li><strong>Delimited —</strong> For each record in each file, fields are separated by a delimiter (configured by the Delimiter field on the <em>Vertical</em> View of the <em><a href="Logical_Paths#LogicalPathsV">Logical Paths</a></em> page). In a comma-separated values (CSV) file, the data items are separated using commas as a delimiter, while in a tab-separated values (TSV) file, the data items are separated using tabs as a delimiter. Column headers are sometimes included as the first line, and each subsequent line is a row of data.</li>
<li><strong>Excel —</strong> Each file is an Excel file. When performing a straight copy of Excel files, the version does not matter. Excel libraries may need to be installed on the DSP application server if Segment By Field or Batched (on the <em>Vertical</em> View of the <a href="Logical_Paths#LogicalPathsV"><em>Logical Paths</em></a> page) are used when copying Excel files.</li>
<li><strong>FixedWidth —</strong> Fixed width text files are special cases of text files where the format is specified by column widths, pad character and left/right alignment. Column widths are measured in units of characters. For example, if you have data in a text file where the first column always has exactly 10 characters, and the second column has exactly 5, the third has exactly 12 (and so on), this would be categorized as a fixed width text file.</li>
</ul></td>
</tr>
</tbody>
</table>
