+++
title = 'File Operations H'
solution = 'Platform'
+++

# File Operations H

[File Operations V](#_File_Operations_V)

<div class="use">

Use this page to:

  - [Add File Operations](../Use_Cases/Add_File_Operations)
  - [Set up a Looping
    Process](../Use_Cases/Set_up_a_Looping_Process)

</div>

To access this page, select **IO Config \> File Operations** in the
*Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>OPERATION</p></td>
<td><p>Displays the name of the operation to be performed.</p></td>
</tr>
<tr class="odd">
<td><p>LOGICAL PATH IN</p></td>
<td><p>Displays the registered data source from which files are transferred.</p></td>
</tr>
<tr class="even">
<td><p>FILE SPEC</p></td>
<td><p>Displays the name of the file specification, indicating the filename or wildcard pattern for the files to be transferred.</p></td>
</tr>
<tr class="odd">
<td><p>LOGICAL PATH OUT</p></td>
<td><p>Displays a registered target, which is the destination to which files are transferred.</p></td>
</tr>
<tr class="even">
<td><p>LOGICAL PATH BACKUP</p></td>
<td><p>Displays the registered target, which is the destination to which a copy of the files is stored.</p></td>
</tr>
<tr class="odd">
<td><p>APPEND DATE</p></td>
<td><p>If checked, the current date is appended to the LOGICAL PATH OUT field.</p>
<p>If unchecked, the current date is not appended to the LOGICAL PATH OUT field.</p>
<p>It is unchecked by default.</p></td>
</tr>
<tr class="even">
<td><p>APPEND TIME</p></td>
<td><p>If checked, the current time is appended to the LOGICAL PATH OUT field.</p>
<p>If unchecked, the current time is not appended to the LOGICAL PATH OUT field.</p>
<p>It is unchecked by default.</p></td>
</tr>
</tbody>
</table>

## <span id="_File_Operations_V"></span> File Operations V

[File Operations H](#_File_Operations_H)

Field

Description

Operation

Displays the name of the operation to be performed.

Logical Path In

Displays the registered data source from which files are transferred.

Logical Path In URI

For FTP sites, displays the entire path of the registered data source,
including log in credentials (user ID and password).

For Local files, displays only the path of the registered data source.

Logical Path Out

Displays a registered target, which is the destination to which files
are transferred.

Logical Path Out URI

For FTP sites, displays the entire path of the registered target,
including log in credentials (user ID and password).

For Local files, displays only the path of the registered target.

Logical Path Backup

Displays the registered target, which is the destination to which a copy
of the files is stored.

Logical Path Backup URI

For FTP sites, displays the entire path of the registered target (with
login credentials, including user ID and password) where a copy of the
files is stored.

For Local files, displays only the path of the registered target, which
is a copy of the files is stored.

File Spec

Displays the name of the file specification, indicating the filename or
wildcard pattern for the files to be transferred.

Append Date

If checked, the current date is appended to the LOGICAL PATH OUT field.

If unchecked, the current date is not appended to the LOGICAL PATH OUT
field.

It is unchecked by default.

Append Time

If checked, the current time is appended to the LOGICAL PATH OUT field.

If unchecked, the current time is not appended to the LOGICAL PATH OUT
field.

It is unchecked by default.

Script Path

Displays the path to the VBS script that executes after acquiring source
file(s) and before transferring files to the target.

Commands

Monitor

Click to open the *[Monitor I/O
Operations](../Use_Cases/Monitor_I_O_Operations)* page. Use this
page to view a record of file operations: when they ran, and whether
they completed or failed processing.

Submit

Click to submit the file operations to the job queue (i.e., to run in
the background).
