+++
title = 'Data Source Instances H'
solution = 'Platform'
+++

# Data Source Instances H

[Data Source Instances V](#Data)

<div class="use">

Use this page to [Add a Data Source
Instance](../Use_Cases/AddDataSourceInstance.htm).

</div>

To access this page in System Administration:

1.  Click **Data Sources** in the *Navigation* pane.
2.  Click the **Instances** icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Test Connection</p></td>
<td><p>Click to test the connection to the Data Source, which verifies the database User ID and Password are connected to the database.</p>
<p><strong>NOTE:</strong> This option is only available for Data Source Types of SQL Server, Oracle, OLE and ODBC.</p></td>
</tr>
<tr class="odd">
<td><p>Recompile Objects</p></td>
<td><p>Click to verify the data is available in the database.</p>
<p><strong>NOTE:</strong> Objects should only be recompiled for SQL Server databases created for the project. Objects may need to be recompiled a few times. If the recompile fails after three attempts, submit an issue to BackOffice Support.</p>
<p><strong>NOTE:</strong> When recompiling a data source, SQL inline Table-Valued functions are not supported.</p></td>
</tr>
<tr class="even">
<td><p>INSTANCE</p></td>
<td><p>Displays the logical platform &quot;instance&quot; (for example, Dev, QA, or Production) this physical instance of the DSP represents.</p></td>
</tr>
<tr class="odd">
<td><p>DATA SOURCE TYPE</p></td>
<td><p>Displays the type of data source.</p>
<p><strong>NOTE:</strong> This field is auto-populated. The data source type value is determined when the data source is registered. Refer to <a href="../Use_Cases/Register_a_Data_Source.htm">Register a Data Source</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>DATABASE</p></td>
<td><p>Displays the name of the SQL Server database used in this Data Source connection. For Oracle it's the Net Service Name stored in the TNS Names file.</p></td>
</tr>
</tbody>
</table>

## <span id="Data"></span>Data Source Instances V

[Data Source Instances H](#top)

This page contains the following tabs: 

  - [General tab](#General)
  - [Advanced Properties tab](#Advanced)

## <span id="General"></span>General tab

Field

Description

Test Connection

Click to test the connection to the Data Source, which verifies the
database User ID and Password are connected to the database.

**NOTE:** This option is only available for Data Source Types of SQL
Server, Oracle, OLE and ODBC.

Recompile Objects

Click to verify the data is available in the database.

**NOTE:** Objects should only be recompiled for SQL Server databases
created for the project. Objects may need to be recompiled a few times.
If the recompile fails after three attempts, submit an issue to
BackOffice Support.

Append Columns

Click to append the BackOffice reserved columns to all tables that do
not already contain them. The following are BackOffice reserved columns:

  - boaStatus\*
  - AddedOn\*
  - AddedBy\*
  - AddedVia\*
  - ChangedBy\*
  - ChangedOn\*
  - ChangedVia\*
  - LockedOn
  - LockedBy
  - BoaLockType

Refer to [Append BOA Reserved Columns to
Tables](../../WebApp_Dev/Append_BOA_Reserved_Columns_to_Tables.htm) for
more information.

Instance

Displays the platform instance (for example, Dev, QA, or Production)
this physical instance represents.

Data Source Type

Displays the type of data source.

**NOTE:** This field is auto-populated. The data source type value is
determined when the data source is registered. Refer to [Register a Data
Source](../Use_Cases/Register_a_Data_Source.htm) for more information.

Connection Settings

Server Address

Displays address of the server this data source connects to.

Database

Displays the name of the SQL Server database used in this Data Source
connection. For Oracle it's the Net Service Name stored in the TNS Names
file.

User ID

Displays the user name used to connect to the data source.

Password

Displays the password associated with the User ID used to connect to the
data source.

## <span id="Advanced"></span>Advanced Properties tab

Field

Description

Protected

If checked, the data source is protected (as in, read only) and features
that make changes to the data source are hidden/disabled (for example,
Recompile Objects, Append System Columns, building System Views,
indexing, auditing, encryption, and building WebApps).

Connection Properties

Port

Displays the TCP/IP Port to use when connecting to the data source. FTP,
HTTP, and databases can use non-default ports for security and
management.

Trusted Connection

If checked, the usage of the User ID and Password fields are bypassed
when connecting to the data source.

If unchecked, the User ID and Password fields are used to verify the
connection.

Connection Timeout

Displays the number of seconds until the connection times out and the
DSP displays an error message stating that the connections failed.
Generally, this value does not need to be changed to a value higher than
30 seconds, and adjustment to values above that should be made after
checking with BackOffice product Support.

Command Timeout

Displays the number of seconds until the command times out, the
execution of the command fails, and the DSP displays a notification
about the error. Insufficient command timeouts are the main cause of
timeout errors in the DSP and this parameter may be increased to a high
value to accommodate long-running processes.
