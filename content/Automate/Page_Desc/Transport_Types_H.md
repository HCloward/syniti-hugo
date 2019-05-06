# <span id="TransportTypeH"></span> Transport Types H

[Transport Types V](#TransportTypeV)

<div class="use">

Use this page to [Add Logical
Paths](../Use_Cases/Add_Logical_Paths.htm).

</div>

To access this page, select **IO Config \> Transport Types** in the
*Navigation* pane.

**NOTE:** It is not recommended to add new transport types or to edit
the delivered transport types; the Automate code would need to be
updated for the transport type type to properly work.

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>DEFAULT</p></td>
<td><p>If checked, the option is the Transport Type used when adding an instance to a logical path on the <em><a href="Logical_Path_Instance.htm"><em>Logical Path (Instance)</em></a></em> page.</p>
<p>If unchecked, the option is not used as the Transport Type when adding an instance to a logical path on the<em><a href="Logical_Path_Instance.htm">Logical Path (Instance)</a></em> page.</p></td>
</tr>
<tr class="odd">
<td><p>TRANSPORT TYPE</p></td>
<td><p>Displays methods to move files from one location to another. Options are:</p>
<ul>
<li><p><strong>Local –</strong> Local File System, which means the files are in folders to which the DSP can read/write.</p></li>
<li><p><strong>FTP –</strong> File Transfer Protocol (FTP), which means the files are located in an FTP address. FTP is a standard network protocol used to copy a file from one host to another over a TCP/IP-based network. All transmissions are in clear text; user names, passwords, FTP commands and transferred filed can be read by anyone on the network.</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a brief description of the transport type.</p></td>
</tr>
<tr class="odd">
<td><p>PORT</p></td>
<td><p>Displays a value on which the server listens to the FTP connection.</p>
<p><strong>NOTE:</strong> This field only used for Transport Type FTP.</p></td>
</tr>
</tbody>
</table>

# <span id="TransportTypeV"></span> Transport Types V

[Transport Types H](#TransportTypeH)

<div class="use">

This page contains the following tabs:

  - [General tab](#_General_1)
  - [Defaults tab](#_Defaults)
  - [Required Fields tab](#_Required_Fields)
  - [Delimiters
tab](#_Delimiters)

</div>

## <span id="_General_1"></span><span class="Hyperlink">General</span> <span class="Hyperlink"> tab</span>

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>Default</p></td>
<td><p>If checked, the option is the Transport Type used when adding an instance to a logical path on the <em><a href="Logical_Path_Instance.htm">Logical Path (Instance)</a></em> page.</p>
<p>If unchecked, the option is not used as the Transport Type when adding an instance to a logical path on the <em><a href="Logical_Path_Instance.htm">Logical Path (Instance)</a></em> page.</p></td>
</tr>
<tr class="odd">
<td><p>Transport Type</p></td>
<td><p>Displays methods to move files from one location to another. Options are:</p>
<ul>
<li><p><strong>Local —</strong> Local File System, which means the files are in folders to which the DSP can read/write.</p></li>
<li><p><strong>FTP —</strong> File Transfer Protocol (FTP), which means the files are located in an FTP address. FTP is a standard network protocol used to copy a file from one host to another over a TCP/IP-based network. All transmissions are in clear text; user names, passwords, FTP commands and transferred filed can be read by anyone on the network.</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p>Description</p></td>
<td><p>Displays a brief description of the transport type.</p></td>
</tr>
</tbody>
</table>

## <span id="_Defaults"></span><span class="Hyperlink">Defaults</span> <span class="Hyperlink"> tab</span>

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>Port</p></td>
<td><p>Displays the default port value when adding an instance to a logical path on the <a href="Logical_Path_Instance.htm"><em>Logical Path (Instance)</em></a> page. Port is where the server listens to the FTP connection.</p>
<p><strong>NOTE:</strong> This field only used for Transport Type FTP.</p></td>
</tr>
<tr class="odd">
<td><p>Path</p></td>
<td><p>Displays the default path value when adding an instance to a logical path on the <a href="Logical_Path_Instance.htm"><em>Logical Path (Instance)</em></a><em></em>page. Path is the FTP path or the complete path where the files are read or written to.</p></td>
</tr>
<tr class="even">
<td><p>Shared Network Name</p></td>
<td><p>This field is not used.</p></td>
</tr>
</tbody>
</table>

## <span id="_Required_Fields"></span> Required Fields tab

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>User ID</p></td>
<td><p>If checked, the logical path instance requires a user ID.</p>
<p>If unchecked, the logical path instance does not require a user ID.</p>
<p>User ID is used to control access to the FTP site.</p>
<p>It is checked by default for FTP transport types and unchecked by default for Local transport types.</p>
<p><strong>NOTE:</strong> This field only used for Transport Type FTP.</p></td>
</tr>
<tr class="odd">
<td><p>Password</p></td>
<td><p>If checked, the logical path instance requires a password.</p>
<p>If unchecked, the logical path instance does not require a password.</p>
<p>Password is a masked password that is used to with the User ID to control access to the FTP site.</p>
<p>It is checked by default for FTP transport types and unchecked by default for Local transport types.</p>
<p><strong>NOTE:</strong> This field only used for Transport Type FTP.</p></td>
</tr>
<tr class="even">
<td><p>Hostname</p></td>
<td><p>If checked, the logical path instance requires a host name.</p>
<p>If unchecked, the logical path instance does not require a host name.</p>
<p>Host name is the hosting server name.</p>
<p>It is checked by default for FTP transport types and unchecked by default for Local transport types.</p>
<p><strong>NOTE:</strong> This field only used for Transport Type FTP.</p></td>
</tr>
<tr class="odd">
<td><p>Path</p></td>
<td><p>If checked, the logical path instance requires a path.</p>
<p>If unchecked, the logical path instance does not require a path.</p>
<p>Path is the FTP path or the complete path where the files are read or written to.</p>
<p>It is checked by default for Local transport types and unchecked by default for FTP transport types.</p></td>
</tr>
<tr class="even">
<td><p>Shared Network Name</p></td>
<td><p>If checked, the transport type requires a Shared Network Name.</p>
<p>If unchecked, the transport type does not require a Shared Network Name.</p>
<p>It is unchecked by default.</p></td>
</tr>
</tbody>
</table>

## <span id="_Delimiters"></span> Delimiters tab

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>Delimiter</p></td>
<td><p>Displays the default character used to parse data to <em><a href="../Use_Cases/Add_Logical_Paths.htm">Add Logical Paths</a></em>.</p>
<p>The default value for FTP transport types is “/”.</p>
<p>The default value for Local transport types is “\”.</p></td>
</tr>
<tr class="odd">
<td><p>Alternate Delimiter</p></td>
<td><p>This field is not used.</p>
<p>The default value for FTP transport types is “\”.</p>
<p>The default value for Local transport types is “/”.</p></td>
</tr>
</tbody>
</table>
