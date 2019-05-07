+++
title = 'Logical Path (Instance) H'
solution = 'Platform'
+++

# Logical Path (Instance) H

[Logical Path (Instance) V](#LogicalPathInstanceV)

<div class="use">

Use this page to [Add Logical
Paths](../Use_Cases/Add_Logical_Paths.htm).

</div>

To access this page:

1.  Select **IO Config \> Logical Paths** in the *Navigation* pane.

<!-- end list -->

2.  Click the **Instances** icon for the desired logical path.

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>INSTANCE</p></td>
<td><p>Displays the environment name.</p>
<p><strong>NOTE:</strong> The instance configured must match the instance selected on the Automate <em><a href="Parameters.htm">Parameters</a></em> page. If the instances do not match, the file processing will not work correctly.</p></td>
</tr>
<tr class="odd">
<td><p>PATH</p></td>
<td><p>Displays either the FTP path or the complete local path where the files are read or written to.</p>
<p><strong>NOTE:</strong> For FTP transport types, do not include a ftp.// destination or a port number; only a server name or an IP address is required.</p></td>
</tr>
<tr class="even">
<td><p>HOSTNAME</p></td>
<td><p>Displays the hosting server name.</p>
<p><strong>NOTE:</strong> This field only displays for logical paths where the Transport Type is FTP.</p></td>
</tr>
<tr class="odd">
<td><p>PORT</p></td>
<td><p>Displays a value on which the server listens to the FTP connection.</p>
<p><strong>NOTE:</strong> This field only displays for logical paths where the Transport Type is FTP.</p></td>
</tr>
<tr class="even">
<td><p>USER ID</p></td>
<td><p>Displays the User ID used to control access to the FTP site.</p>
<p><strong>NOTE:</strong> This field only displays for logical paths where the Transport Type is FTP.</p></td>
</tr>
<tr class="odd">
<td><p>PASSWORD</p></td>
<td><p>Displays a masked password that is used to with the User ID to control access to the FTP site.</p>
<p><strong>NOTE:</strong> This field only displays for logical paths where the Transport Type is FTP.</p></td>
</tr>
<tr class="even">
<td><p>Test</p></td>
<td><p>Click to test the instance’s connection to the logical path.</p></td>
</tr>
<tr class="odd">
<td><p>Browse</p></td>
<td><p>Click to open the <em><a href="Logical_Path_Instance_Browse.htm">Logical Path Instance (Browse)</a></em> page to browse the FTP site or the path for other folders or files, and change the FTP site or path if necessary. Refer to <a href="../Use_Cases/Browse_FTP_Site_or_Path.htm">Browse FTP Site or Path</a> for more information.</p></td>
</tr>
</tbody>
</table>

 

# <span id="LogicalPathInstanceV"></span> Logical Path (Instance) V

[Logical Path (Instance) H](#LogicalPathInstanceH)

 

**Field**

**Description**

Transport Type

Displays the type of file transport. Options are:

  - **Local –** Local File System, which means the files are in folders
    to which the DSP can read/write.
  - **FTP –** File Transfer Protocol (FTP), which means the files are
    located in an FTP address. FTP is a standard network protocol used
    to copy a file from one host to another over a TCP/IP-based network.
    All transmissions are in clear text; user names, passwords, FTP
    commands and transferred filed can be read by anyone on the network.

Instance

Displays the environment name.

**NOTE:** The instance configured must match the instance selected on
the *Vertical* View of the Automate *[Parameters](Parameters.htm)* page.
If the instances do not match, the file processing will not work
correctly.

Connection Information

Hostname

Displays the hosting server name.

**NOTE:** This field only displays for logical paths where the Transport
Type is FTP.

Port

Displays a value on which the server listens to the FTP connection.

**NOTE:** This field only displays for logical paths where the Transport
Type is FTP.

Path

Displays either the FTP path or the complete logical path where the
files are read or written to.

**NOTE:** For FTP transport types, do not include a ftp.// destination
or a port number; only a server name or an IP address is required.

Security Information

User ID

Displays the User ID used to control access to the FTP site.

**NOTE:** This field only displays for logical paths where the Transport
Type is FTP.

Password

Displays a masked password that is used to with the User ID to control
access to the FTP site.

**NOTE:** This field only displays for logical paths where the Transport
Type is FTP.

Permissions

Can Read

If checked, users have reading privileges to this instance.

If unchecked, users do not have reading privileges to this instance.

It is unchecked by default.

Can Write

If checked, users have writing privileges to this instance.

If unchecked, users do not have writing privileges to this instance.

It is unchecked by default.

Can Delete

If checked, users have deleting privileges to this instance.

If unchecked, users do not have deleting privileges to this instance.

It is unchecked by default.

Actions

Test

Click to test the instance’s connection to the logical path.

Browse

Click to open the *[Logical Path Instance
(Browse)](Logical_Path_Instance_Browse.htm)* page to browse the FTP site
or the path for other folders or files, and change the FTP site or path
if necessary. Refer to [Browse FTP Site or
Path](../Use_Cases/Browse_FTP_Site_or_Path.htm) for more information.
