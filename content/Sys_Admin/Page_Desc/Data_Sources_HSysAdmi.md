+++
title = 'Data Sources H'
solution = 'Platform'
+++

# Data Sources H

<span style="font-weight: bold;">NOTE:</span> It is recommended that
data sources be registered in Common instead of System Administration. A
Data Services data source must be registered in Common and cannot be
registered in System Administration.

<div class="use">

Use this page to:

  - [Register a Data Source](../Use_Cases/Register_a_Data_Source)
  - [Register the Database for a Custom
    WebApp](../../WebApp_Dev/Register_the_Database_for_a_Custom_WebApp)
  - [Append BOA Reserved Columns to
    Tables](../../WebApp_Dev/Append_BOA_Reserved_Columns_to_Tables)
  - [Encrypt a Column](../../WebApp_Dev/Encrypt_a_Column)

</div>

The configuration of the
<span style="font-style: italic;">Vertical</span> View depends on the
Data Source Type. Options are:

  - [SQL Server](#Data_Sources_V:_SQL_Server)
  - [ODBC](#Data_Sources_V:_ODBC)
  - [Local File](#Data_Sources_V:_Local_File)
  - [OleDB](#Data_Sources_V:_OleDB)
  - [Oracle](#Data_Sources_V:_Oracle)
  - [Remote File (FTP)](#Data_Sources_V:_Remote_File__FTP_)
  - [Remote File (HTTP)](#Data_Sources_V:_Remote_File__HTTP_)
  - [Remote File (UNC)](#Data_Sources_V:_Remote_File__UNC_)

To access this page, select  **Admin \> Data Sources** in the
*Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Test Connection</p></td>
<td><p>Click to test the connection to the data source, which verifies that</p>
<ul>
<li>The user ID and password are valid for databases or</li>
<li>Permissions have been granted to access the specified path in the file system for remote files.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Recompile Objects</p></td>
<td><p>Click to verify the data is available in the database.</p>
<p><strong>NOTE:</strong> Objects should only be recompiled for SQL Server databases created for the project. Objects may need to be recompiled a few times. If the recompile fails after three attempts, submit an issue to BackOffice Support.</p>
<p><strong>NOTE:</strong> When recompiling a data source, SQL inline Table-Valued functions are not supported.</p></td>
</tr>
<tr class="even">
<td><p>DATA SOURCE NAME</p></td>
<td><p>Displays name of the data source.</p></td>
</tr>
<tr class="odd">
<td><p>DATA SOURCE TYPE</p></td>
<td><p>Displays the type of data source. The default value is SqlServer. Options are:</p>
<ul>
<li>Local File</li>
<li>ODBC</li>
<li>OleDB</li>
<li>Oracle</li>
<li>Remote File (FTP)</li>
<li>Remote File (HTTP)</li>
<li>Remote File (UNC)</li>
<li>SqlServer</li>
</ul></td>
</tr>
<tr class="even">
<td><p>DATABASE</p></td>
<td><p>Displays the database name exactly as it appears in the database. For Oracle databases, the Database name appears in the TNS name file.</p></td>
</tr>
<tr class="odd">
<td><p>Audit</p></td>
<td><p>Click to open the <em><a href="Audit_Configuration">Audit Configuration</a></em> page to enable auditing for specific tables in the database. This icon is only enabled for SQL Server data sources if the data source is protected (if the Protected check box on the <em>Vertical</em> View of this page is checked).</p></td>
</tr>
<tr class="even">
<td><p>Index</p></td>
<td><p>Click to open the <a href="Index%20Specification%20H"><em>Index (Specification)</em></a> page to configure index tables for the database. This icon is disabled if the data source is not Microsoft SQL Server and it is not protected (if the Protected check box on the <em>Vertical</em> View of this page is unchecked).</p></td>
</tr>
<tr class="odd">
<td><p>Instances</p></td>
<td><p>Click to open the <em>Data Source Instances</em> page to add, edit and delete instances for the data source.</p></td>
</tr>
<tr class="even">
<td><p>Encryption</p></td>
<td><p>Click to open the <em><a href="Data_Source_Column_Encryption">Data Source Column Encryption</a></em> page to enable or disable encryption for a specific field within a database table. This icon is disabled if the data source is not Microsoft SQL Server and it is not protected (if the Protected check box on the <em>Vertical</em> View of this page is unchecked).</p></td>
</tr>
</tbody>
</table>

## <span id="Data_Sources_V_All_Tabs"></span>Data Sources V

[Data Sources H](Data_Sources_HSysAdmi)

<div class="use">

Use this page to [Register a Data
Source](../Use_Cases/Register_a_Data_Source).

</div>

The configuration of the Vertical View depends on the Data Source Type.
Options are:

  - [SQL Server](#Data_Sources_V:_SQL_Server)
  - [ODBC](#Data_Sources_V:_ODBC)
  - [Local File](#Data_Sources_V:_Local_File)
  - [OleDB](#Data_Sources_V:_OleDB)
  - [Oracle](#Data_Sources_V:_Oracle)
  - [Remote File (FTP)](#Data_Sources_V:_Remote_File__FTP_)
  - [Remote File (HTTP)](#Data_Sources_V:_Remote_File__HTTP_)
  - [Remote File
(UNC)](#Data_Sources_V:_Remote_File__UNC_)

## <span id="Data_Sources_V:_SQL_Server"></span>Data Sources V: SQL Server

This page contains the following tabs:

  - [General tab](#General_Tab)
  - [Advanced Properties tab](#Advanced_Properties_Tab)

## <span id="General_Tab"></span>General tab

Field

Description

Test Connection

Click to test the connection to the data source, which verifies that the
user ID and password are valid.

Recompile Objects

Click to verify the data is available in the database. Objects may need
to be recompiled a few times. If the recompile fails after three
attempts, submit an issue to BackOffice Support:

[https://support.boaweb.com/](http://support.boaweb.com/).

Append Columns

Click to append the BackOffice reserved columns to all tables in the
data source that do not already contain them. The following are
BackOffice reserved columns:

  - boaStatus
  - AddedOn
  - AddedBy
  - AddedVia
  - ChangedBy
  - ChangedOn
  - ChangedVia

Refer to [Append BOA Reserved Columns to
Tables](../../WebApp_Dev/Append_BOA_Reserved_Columns_to_Tables) for
more information.

**NOTE** This feature is used for local SQL data sources only.

Data Source Type

Displays the type of data source: SqlServer.

Connection Settings

Server Address

Displays address of the server this data source connects to. The
database name must be the host name of the database instance and cannot
be the IP address. Although the IP address may test successfully, if the
IP address is used for the CranSoft data source, then Collect downloads
do not return the Record Count and the rules registered to Collect
tables will not execute.

Database

Displays the database name exactly as it appears in the database.

User ID

Displays the user ID used to connect to the database.

Password

Displays asterisks representing the password associated with the user ID
used to connect to the database.

## <span id="Advanced_Properties_Tab"></span>Advanced Properties tab

Field

Description

Active

If checked, the data source is active. If unchecked, the data source is
inactive, and system views cannot be created for the data source.

Protected

If checked, the data source is protected (read only) and no schema
changes will be performed by DSP®.

Features that make changes to the data source are hidden/disabled (for
example, Recompile Objects, Append System Columns, building System
Views, indexing, auditing, encryption, and building WebApps).

System Views

If checked, Systems Views are created in the data source by DSP®. System
Views are views that are installed by the Platform in a data source that
links back to certain tables or views in the CranSoft database.

This feature is often used for more advanced WebApp development.

If unchecked, Systems Views are not created in the data source by DSP®.

Connection Properties

Port

Displays the TCP/IP Port to use when connecting to the data source. FTP,
HTTP, and databases can use non-default ports for security and
management.

Trusted Connection

If checked, if the Server is configured to connect using Windows
Authentication, the connection uses the hosting machine’s information to
authenticate the connection and bypass the usage of the User ID and
Password fields.

Connection Timeout

Displays the number of seconds until the connection times out and the
DSP displays an error message stating that the connection failed.
Generally, this value does not need to be changed to a value higher than
30 seconds, and adjustment to values above that should be made after
checking with BackOffice Product Support.

Command Timeout

Displays the number of seconds until the command times out, the
execution of the command fails, and the DSP displays a notification
about the error. Insufficient command timeouts are the main cause of
timeout errors in DSP and this parameter may be increased to a high
value to accommodate long running processes.

 

## <span id="Data_Sources_V:_ODBC"></span>Data Sources V: ODBC

[Data Sources H](Data_Sources_HSysAdmi)

This page contains the following tabs:

  - [General tab](#Data_Sources_ODBC_General_tab)
  - [Advanced Properties
    tab](#Data_Sources_ODBC_Advanced_Properties_tab)

## <span id="Data_Sources_ODBC_General_tab"></span>General tab

Field

Description

Test Connection

Click to test the connection to the data source, which verifies that the
user ID and password are valid.

Recompile Objects

*This feature is not supported for ODBC data sources.*

Append Columns

*This feature is not supported for ODBC data sources.*

Data Source Type

Displays the type of data source: ODBC.

Connection Settings

Database Type

Displays the type of database.

Server Address

Displays address of a non-DSP server used to connect to the current
system. The database name must be the host name of the database instance
and cannot be the IP address. Although the IP address may test
successfully, if the IP address is used for the CranSoft data source,
then Collect downloads do not return the Record Count and the rules
registered to Collect tables will not execute.

Database

Displays the database name exactly as it appears in the database.

Connection String

Displays the OLE database connection string.

DSN

Displays the Data Source Name (DSN) parameter, which can be used when
the connection to the data source is not a SQL server connection. It is
used primarily when defined by the web server control panel, or if the
SQL server connection requires additional special parameters not
supplied by the DSP standard connection.

User ID

Displays the user name used to connect to the database.

Password

Displays asterisks representing the password associated with the User ID
used to connect to the
database.

## <span id="Data_Sources_ODBC_Advanced_Properties_tab"></span>Advanced Properties tab

Field

Description

Active

If checked, the data source is active. If unchecked, the data source is
inactive and system views cannot be created for the data source.

Protected

If checked, the data source is protected (read only) and no schema
changes will be performed by DSP.

Features that make changes to the data source are hidden/disabled (for
example, Recompile Objects, Append System Columns, building System
Views, indexing, auditing, encryption, and building WebApps).

System Views

If checked, Systems Views are created in the data source by DSP®. System
Views are views that are installed by the Platform in a data source that
links back to certain tables or views in the CranSoft database.

This feature is often used for advanced WebApp development.

If unchecked, Systems Views are not created in the data source by DSP®.

Connection Properties

Connection Timeout

Displays the number of seconds until the connection times out and the
DSP displays an error message stating that the connection failed.
Generally, this value does not need to be changed to a value higher than
30 seconds, and adjustment to values above that should be made after
checking with BackOffice Product Support.

Command Timeout

Displays the number of seconds until the command times out, the
execution of the command fails, and the DSP displays a notification
about the error. Insufficient command timeouts are the main cause of
timeout errors in DSP and this parameter may be increased to a high
value to accommodate long running processes.

Schema Properties

Procedure Parameter Name Prefix

Displays the parameter prefix used for the data source. Parameters are
usually prefixed to not conflict with table/view column names when
writing a stored procedure. By registering this prefix at the data
source level, the Platform adds the prefix to the column name when
passing parameters to stored
procedures.

 

## <span id="Data_Sources_V:_Local_File"></span>Data Sources V: Local File

[Data Sources H](Data_Sources_HSysAdmi)

This page contains the following tabs:

  - [General tab](#Data_Sources_Local_File_General_tab)
  - [Permissions tab](#Data_Sources_Local_File_Permissions_tab)

## <span id="Data_Sources_Local_File_General_tab"></span>General tab

Field

Description

Test Connection

Click to test the connection to the file system. This process:

  - Verifies the User ID and Password are valid and/or verifies
    permissions have been granted to access the specified path in the
    file system.
  - Updates the permissions on the Permissions tab.

Data Source Type

Displays the type of data source: Local File.

Path Settings

Path

Displays the path where the local file is
stored.

## <span id="Data_Sources_Local_File_Permissions_tab"></span>Permissions tab

|            |                                                                                                                                                                                                                                            |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field      | Description                                                                                                                                                                                                                                |
| Can Read   | If checked, users have Read permissions to the local file. This field is set based on the permissions granted by the file system given the file path and credentials specified, and is updated when the Test Connection icon is clicked.   |
| Can Write  | If checked, users have Write permissions to the local file. This field is set based on the permissions granted by the file system given the file path and credentials specified, and is updated when the Test Connection icon is clicked.  |
| Can Delete | If checked, users have Delete permissions to the local file. This field is set based on the permissions granted by the file system given the file path and credentials specified, and is updated when the Test Connection icon is clicked. |

## <span id="Data_Sources_V:_OleDB"></span>Data Sources V: OleDB

[Data Sources H](Data_Sources_HSysAdmi)

This page contains the following tabs:

  - [General tab](#Data_Sources_OleDB_General_tab)
  - [Advanced Properties
    tab](#Data_Sources_OleDB_Advanced_Properties_tab)

## <span id="Data_Sources_OleDB_General_tab"></span>General tab

Field

Description

Test Connection

Click to test the connection to the Data Source by verifying that the
User ID and Password are valid.

Recompile Objects

*This feature is not supported for OleDB data source types.*

Append Columns

*This feature is not supported for OleDB data source types.*

Data Source Type

Displays the type of data source: OleDB.

Connection Settings

Database Type

Displays the type of database.

Server Address

Displays address of a non-DSP server used to connect to the current
system. The database name must be the host name of the database instance
and cannot be the IP address. Although the IP address may test
successfully, if the IP address is used for the CranSoft data source,
then Collect downloads do not return the Record Count and the rules
registered to Collect tables will not execute.

Database

Displays the database name exactly as it appears in the database.

Connection String

Displays the OLE database connection string.

DSN

Displays the Data Source Name (DSN) parameter, which can be used when
the connection to the data source is not a SQL server connection. It is
used primarily when defined by the web server control panel, or if the
SQL server connection requires additional special parameters not
supplied by the DSP standard connection.

User ID

Displays the user name used to connect to the database.

Password

Displays asterisks representing the password associated with the User ID
used to connect to the
database.

## <span id="Data_Sources_OleDB_Advanced_Properties_tab"></span>Advanced Properties tab

Field

Description

Active

If checked, the data source is active. If unchecked, the data source is
inactive and system views cannot be created for the data source.

Protected

If checked, the Data Source is protected (read only) and features that
make changes to the Data Source will be hidden/disabled (e.g., Recompile
Objects, Append System Columns, building System Views, indexing,
auditing, encryption, and building WebApps).

System Views

If checked, Systems Views are created in the data source by DSP®. System
Views are views that are installed by the Platform in a data source that
links back to certain tables or views in the CranSoft database.

This feature is often used for advanced WebApp development.

If unchecked, Systems Views are not created in the data source by DSP®.

Connection Properties

Connection Timeout

Displays the number of seconds until the connection times out and the
DSP displays an error message stating that the connection failed.
Generally, this value does not need to be changed to a value higher than
30 seconds, and adjustment to values above that should be made after
checking with BackOffice Product Support.

Command Timeout

Displays the number of seconds until the command times out, the
execution of the command fails, and the DSP displays a notification
about the error. Insufficient command timeouts are the main cause of
timeout errors in DSP and this parameter may be increased to a high
value to accommodate long running processes.

Schema Properties

Procedure Parameter Name Prefix

Displays the parameter prefix used for the data source. Parameters are
usually prefixed to not conflict with table/view column names when
writing a stored procedure. By registering this prefix at the data
source level, the Platform adds the prefix to the column name when
passing parameters to stored procedures.

## <span id="Data_Sources_V:_Oracle"></span>Data Sources V: Oracle

[Data Sources H](Data_Sources_HSysAdmi)

This page contains the following tabs:

  - [General tab](#Data_Sources_Oracle_General_tab)
  - [Advanced Properties
    tab](#Data_Sources_Oracle_Advanced_Properties_tab)

## <span id="Data_Sources_Oracle_General_tab"></span>General tab

Field

Description

Test Connection

Click to test the connection to the Data Source, which verifies that the
user ID and password are valid..

Recompile Objects

Click to verify the data is available in the database. Objects may need
to be recompiled a few times. If the recompile fails after three
attempts, submit an issue to BackOffice Support:

<http://support.boaweb.com/>.

Append Columns

*This feature is not supported for Oracle data source types.*

Click to append the BackOffice reserved columns to all tables in the
data source that do not already contain them. The following are
BackOffice reserved columns:

  - boaStatus
  - AddedOn
  - AddedBy
  - AddedVia
  - ChangedBy
  - ChangedOn
  - ChangedVia

Refer to [Append BoA Reserved Columns to
Tables](../../WebApp_Dev/Append_BOA_Reserved_Columns_to_Tables) for
more information.

Data Source Type

Displays the type of data source.

Connection Settings

Server Address

Displays address of a non-DSP server used to connect to the current
system. The database name must be the host name of the database instance
and cannot be the IP address. Although the IP address may test
successfully, if the IP address is used for the CranSoft data source,
then Collect downloads do not return the Record Count and the rules
registered to Collect tables will not execute.

Database

Displays the database name exactly as it appears in the database.

**NOTE**: If this field is populated, the Database Instance Name on the
Advanced Properties tab must be blank.

User ID

Displays the user name used to connect to the database.

Password

Displays asterisks representing the password associated with the User ID
used to connect to the
database.

## <span id="Data_Sources_Oracle_Advanced_Properties_tab"></span>Advanced Properties tab

Field

Description

Active

If checked, the data source is active. If unchecked, the data source is
inactive and system views cannot be created for the data source.

Protected

If checked, the Data Source is protected (i.e., read only) and features
that make changes to the Data Source will be hidden/disabled (e.g.,
Recompile Objects, Append System Columns, building System Views,
indexing, auditing, encryption, and building WebApps).

Connection Properties

Database Instance Name

Displays the Oracle instance name. This field is not required if using
the Database Instance Name listed in the TNSNames.ora file for
connection. If using the Database field on the General tab, this field
should be empty.

Port

Displays the TCP/IP Port to use when connecting to this Oracle data
source. This field is not required if using the Port listed in the
TNSNames.ora file for the connection.

Trusted Connection

If checked, if the Server is configured to connect using Windows
Authentication, the connection uses the hosting machine’s information to
authenticate the connection and does not use the User ID and Password
fields.

Connection Timeout

Displays the number of seconds until the connection times out and the
DSP displays an error message stating that the connection failed.
Generally, this value does not need to be changed to a value higher than
30 seconds, and adjustment to values above that should be made after
checking with BackOffice Product Support.

Command Timeout

Displays the number of seconds until the command times out, the
execution of the command fails, and the DSP displays a notification
about the error. Insufficient command timeouts are the main cause of
timeout errors in DSP and this parameter may be increased to a high
value to accommodate long running processes.

Schema Properties

Procedure Parameter Name Prefix

Displays the parameter prefix used for the data source. Parameters are
usually prefixed to not conflict with table/view column names when
writing a stored procedure. By registering this prefix at the data
source level, the Platform adds the prefix to the column name when
passing parameters to stored procedures.

Sequences

This feature is not
used.

## <span id="Data_Sources_V:_Remote_File__FTP_"></span>Data Sources V: Remote File (FTP)

This page contains the following tabs:

  - [General tab](#Data_Sources_Remote_File__FTP_General_tab)
  - [Permissions
tab](#Data_Sources_Remote_File__FTP_Permissions_tab)

## <span id="Data_Sources_Remote_File__FTP_General_tab"></span>General tab

Field

Description

Test Connection

Click to test the connection to the file system. This process:

  - Verifies the User ID and Password are valid and permissions have
    been granted to access the specified path in the file system
  - Updates the permissions on the Permissions tab

Data Source Type

Displays the type of data source: Remote File (FTP).

Path Settings

Server Address

Displays address of a non-DSP server used to connect to the current
system.

Path

Displays the path where the remote file is stored.

Port

Displays the TCP/IP Port to use when connecting to the data source. FTP,
HTTP, and databases can use non-default port for security and
management.

User ID

Displays the user name used to connect to the file system.

Password

Displays asterisks representing the password associated with the User ID
used to connect to the file
system.

## <span id="Data_Sources_Remote_File__FTP_Permissions_tab"></span>Permissions tab

|            |                                                                                                                                                                                                                                             |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field      | Description                                                                                                                                                                                                                                 |
| Can Read   | If checked, users have Read permissions to the remote file. This field is set based on the permissions granted by the file system given the file path and credentials specified, and is updated when the Test Connection icon is clicked.   |
| Can Write  | If checked, users have Write permissions to the remote file. This field is set based on the permissions granted by the file system given the file path and credentials specified, and is updated when the Test Connection icon is clicked.  |
| Can Delete | If checked, users have Delete permissions to the remote file. This field is set based on the permissions granted by the file system given the file path and credentials specified, and is updated when the Test Connection icon is clicked. |

## <span id="Data_Sources_V:_Remote_File__HTTP_"></span>Data Sources V: Remote File (HTTP)

This page contains the following tabs:

  - [General tab](#Data_Sources_Remote_File__HTTP_General_tab)
  - [Permissions
tab](#Data_Sources_Remote_File__HTTP_Permissions_tab)

## <span id="Data_Sources_Remote_File__HTTP_General_tab"></span>General tab

Field

Description

Test Connection

Click to test the connection to the file system. This process:

  - Verifies the User ID and Password are valid and permissions have
    been granted to access the specified path in the file system
  - Updates the permissions on the Permissions tab

Data Source Type

Displays the type of data source: Remote File (HTTP).

Path Settings

Server Address

Displays address of a non-DSP server used to connect to the current
system..

Path

Displays the path where the data source is stored.

User ID

Displays the user name used to connect to the file system.

Password

Displays asterisks representing the password associated with the User ID
used to connect to the file
system.

## <span id="Data_Sources_Remote_File__HTTP_Permissions_tab"></span>Permissions tab

|            |                                                                                                                                                                                                                                             |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field      | Description                                                                                                                                                                                                                                 |
| Can Read   | If checked, users have Read permissions to the remote file. This field is set based on the permissions granted by the file system given the file path and credentials specified, and is updated when the Test Connection icon is clicked.   |
| Can Write  | If checked, users have Write permissions to the remote file. This field is set based on the permissions granted by the file system given the file path and credentials specified, and is updated when the Test Connection icon is clicked.  |
| Can Delete | If checked, users have Delete permissions to the remote file. This field is set based on the permissions granted by the file system given the file path and credentials specified, and is updated when the Test Connection icon is clicked. |

## <span id="Data_Sources_V:_Remote_File__UNC_"></span>Data Sources V: Remote File (UNC)

This page contains the following tabs:

  - [General tab](#Data_Sources_Remote_File__UNC_General_tab)
  - [Permissions
tab](#Data_Sources_Remote_File__UNC_Permissions_tab)

## <span id="Data_Sources_Remote_File__UNC_General_tab"></span>General tab

Field

Description

Test Connection

Click to test the connection to the file system. This process:

  - Verifies the User ID and Password are valid and permissions have
    been granted to access the specified path in the file system
  - Updates the permissions on the Permissions tab

Data Source Type

Displays the type of data source: Remote File (UNC).

Path Settings

Path

Displays the path where the remote file is stored.

User ID

Displays the user name used to connect to the file system.

Password

Displays asterisks representing the password associated with the User ID
used to connect to the file
system.

### <span id="Data_Sources_Remote_File__UNC_Permissions_tab"></span>Permissions tab

|            |                                                                                                                                                                                                                                             |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field      | Description                                                                                                                                                                                                                                 |
| Can Read   | If checked, users have Read permissions to the remote file. This field is set based on the permissions granted by the file system given the file path and credentials specified, and is updated when the Test Connection icon is clicked.   |
| Can Write  | If checked, users have Write permissions to the remote file. This field is set based on the permissions granted by the file system given the file path and credentials specified, and is updated when the Test Connection icon is clicked.  |
| Can Delete | If checked, users have Delete permissions to the remote file. This field is set based on the permissions granted by the file system given the file path and credentials specified, and is updated when the Test Connection icon is clicked. |
