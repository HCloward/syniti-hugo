+++
title = ''
solution = 'Platform'
+++

# <span id="LogicalPathsH"></span> Logical Paths H

[Logical Paths V](#LogicalPathsV)

<div class="use">

Use this page to [Add Logical
Paths](../Use_Cases/Add_Logical_Paths.htm).

</div>

To access this page, select **IO Config \> Logical Paths** in the
*Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>LOGICAL PATH</p></td>
<td><p>Displays the file path of the folder or the FTP site.</p></td>
</tr>
<tr class="odd">
<td><p>TRANSPORT TYPE</p></td>
<td><p>Displays the type of file transport. Options are:</p>
<ul>
<li><strong>Local –</strong> Local File System, which means the files are in folders to which the DSP can read/write.</li>
<li><strong>FTP –</strong> File Transfer Protocol (FTP), which means the files are located in an FTP address. FTP is a standard network protocol used to copy a file from one host to another over a TCP/IP-based network. All transmissions are in clear text; user names, passwords, FTP commands and transferred filed can be read by anyone on the network.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>FILE MODIFICATION</p></td>
<td><p>Displays how files are modified when copied to the destination. Options are:</p>
<ul>
<li><strong>Batched –</strong> Files are grouped with the amount of records specified in the Batch Size field configured on the <em><a href="#LogicalPathsV">Vertical</a></em> View.</li>
<li><strong>SegmentByFile –</strong> A file is created for each unique value in the Segment Field field configured on the <em><a href="#LogicalPathsV">Vertical</a></em> View.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>FILE FORMAT</p></td>
<td><p>Displays the format of the file. Options are:</p>
<ul>
<li><strong>Delimited –</strong> For each record in each file, fields are separated by a delimiter (configured by the Delimiter field on the <em><a href="#LogicalPathsV">Vertical</a></em> View).  In a comma-separated values (CSV) file, the data items are separated using commas as a delimiter, while in a tab-separated values (TSV) file, the data items are separated using tabs as a delimiter. Column headers are sometimes included as the first line, and each subsequent line is a row of data.</li>
<li><strong>Excel –</strong> Each file is an Excel file. When performing a straight copy of Excel files, the version does not matter. Excel libraries may need to be installed on the DSP application server if Segment By Field or Batched are used when copying Excel files.</li>
<li><strong>FixedWidth –</strong> Each field is specified by column widths, pad character and left/right alignment.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Instances</p></td>
<td><p>Click to open the <em><a href="Logical_Path_Instance.htm">Logical Path (Instance)</a></em> page to configure the environment for the logical path. The count on the icon is the total number of instances registered to the selected logical path.</p>
<p>The count on the icon is the total number of instances registered to the selected logical path.</p></td>
</tr>
</tbody>
</table>

 

# <span id="LogicalPathsV"></span> Logical Paths V

[Logical Paths H](#LogicalPathsH)

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>Logical Path</p></td>
<td><p>Displays the file path of the folder or the FTP site.</p></td>
</tr>
<tr class="odd">
<td><p>Transport Type</p></td>
<td><p>Displays the type of file transport. Options are:</p>
<ul>
<li><strong>Local –</strong> Local File System, which means the files are in folders to which the DSP can read/write.</li>
<li><strong>FTP –</strong> File Transfer Protocol (FTP), which means the files are located in an FTP address. FTP is a standard network protocol used to copy a file from one host to another over a TCP/IP-based network. All transmissions are in clear text; user names, passwords, FTP commands and transferred filed can be read by anyone on the network.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>File Modification</p></td>
<td><p>Displays how files are modified when copied to the destination. Options are:</p>
<ul>
<li><strong>Batched –</strong> Files are grouped with the amount of records specified in the Batch Size field.</li>
<li><strong>SegmentByFile –</strong>A file is created for each unique value in the Segment By Field field.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Batch Size</p></td>
<td><p>Displays a number to indicate the batch size.</p>
<p><strong>NOTE:</strong> Populate this field if the File Modification is Batched.</p></td>
</tr>
<tr class="even">
<td><p>Delimiter</p></td>
<td><p>Displays a character used to parse data.</p>
<p><strong>NOTE:</strong> Populate this field if the File Format is Delimited.</p></td>
</tr>
<tr class="odd">
<td><p>Text Qualifier</p></td>
<td><p>Displays a character used to enclose text strings.</p>
<p><strong>NOTE:</strong> Populate this field if the File Format is Delimited.</p></td>
</tr>
<tr class="even">
<td><p>Contains Header</p></td>
<td><p>If checked, there is a header record in the file that must be ignored.</p>
<p>If unchecked, there is not a header record in the file.</p>
<p>It is unchecked by default.</p></td>
</tr>
<tr class="odd">
<td><p>Segment By Field</p></td>
<td><p>Displays the name of the fields by which to divide the file.</p>
<p><strong>NOTE:</strong> Populate this field if the File Modification is SegmentByField.</p></td>
</tr>
<tr class="even">
<td><p>File Format</p></td>
<td><p>Displays the format of the file. Options are:</p>
<ul>
<li><strong>Delimited –</strong> For each record in each file, fields are separated by a delimiter (configured by the Delimiter field on the Vertical View).  In a comma-separated values (CSV) file, the data items are separated using commas as a delimiter, while in a tab-separated values (TSV) file, the data items are separated using tabs as a delimiter. Column headers are sometimes included as the first line, and each subsequent line is a row of data.</li>
<li><strong>Excel –</strong> Each file is an Excel file. When performing a straight copy of Excel files, the version does not matter. Excel libraries may need to be installed on the DSP application server if Segment By Field or Batched are used when copying Excel files.</li>
<li><strong>FixedWidth –</strong> Each field is specified by column widths, pad character and left/right alignment.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Instances</p></td>
<td><p>Click to open the <em><a href="Logical_Path_Instance.htm">Logical Path (Instance)</a></em> page to configure the environment for the logical path.</p>
<p>The count on the icon is the total number of instances registered to the selected logical path.</p></td>
</tr>
</tbody>
</table>
