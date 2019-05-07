+++
title = 'Data Source Registry H'
solution = 'Platform'
+++

# Data Source Registry H

<span lang="EN">[Data Source Registry V](#Data_Source_Registry_V)</span>

<div class="use">

Use this page to [Register a Data Source in
Common](../Use_Cases/Register_a_Data_Source_in_Common.htm).

</div>

To access this page, select <span style="font-weight: bold;">Common \>
Configuration \> Data Source Registry</span> in the
<span style="font-style: italic;">Navigation</span> pane.

**NOTE:** Bulk Execution has been enabled on this page. Refer to [Use
Bulk Execution](../../Bulk_Exec/Use_Bulk_Execution.htm) for more
information.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Test Connection</p></td>
<td><p>Click to test the connection to the data source, which verifies the user ID and password.</p></td>
</tr>
<tr class="odd">
<td><p>NAME</p></td>
<td><p>Displays the name of the data source.</p></td>
</tr>
<tr class="even">
<td><p>APPLICATION DATA SOURCE TYPE</p></td>
<td><p>Displays the type of data source (for example, an Oracle Database or a Local File). Refer to the Knowledge Base article &quot;<a href="https://support.boaweb.com/hc/en-us/articles/115015120927--DSP-Common-SysAdmin-Data-Sources#C2">How DSP Applications Use Different Data Source Types</a>&quot; on the BackOffice Associates support site (https://support.boaweb.com) for more information.</p></td>
</tr>
<tr class="odd">
<td><p>OUT OF SYNC</p></td>
<td><p>Displays an icon if there was a change made to the data source on the System Administration <span lang="EN" style="font-style: italic;">Data Sources</span> page.</p>
<p>The user can either:</p>
<ul>
<li>Apply the updates made to the data source in Common to the data source in System Administration by validating or saving the record in Common</li>
</ul>
<ul>
<li>Apply the updates made to the data source in System Administration to the data source in Common manually</li>
</ul>
<p>Refer to <a href="../Use_Cases/Sync_Data_Sources_in_Common_and_System_Administration.htm">Sync Data Sources in Common and System Administration</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Admin Data Source</p></td>
<td><p>Click to open the <span style="font-style: italic;">Data Sources</span> page in System Administration to view changes entered in System Administration for the selected data source.</p>
<p><strong>NOTE:</strong> A user must have permission to access the <em>Data Sources</em> page in System Administration.</p></td>
</tr>
</tbody>
</table>

## <span id="Data_Source_Registry_V"></span>Data Source Registry V

[Data Source Registry H](#Data_Source_Registry_H)

<div class="use">

Use this page to [Register a Data Source in
Common](../Use_Cases/Register_a_Data_Source_in_Common.htm).

</div>

Application Data Source Types

Data Services Repository (%)

  - [General](#data_service_rep_gen)
  - [Advanced Settings](#Data_Services_Repository_Advanced_Settings)

External System Connection (%)

  - [General](#External_System_Connection_____-_General)
  - [Advanced
    Settings](#External_System_Connection_______Advanced_Settings)

IG Universal Connect (%)

  - [General](#IG)
  - [Advanced Settings](#IG2)

Local Utility Database (%)

  - [General](#Local_Utility_Database_____-_General)
  - [Advanced Settings](#Local_Utility_Database_______Advanced_Settings)

Migration Object Database (dsw%)

  - [General](#Migration_Object_Database__dsw_____General)
  - [Advanced
    Settings](#Migration_Object_Database__dsw_____Advanced_Settings)

Migration Source Database (sdb%)

  - [General](#Migration_Source_Database__sdb_____General)
  - [Advanced
    Settings](#Migration_Source_Database__sdb_____Advanced_Settings)

SAP Application Server (%)

  - [General](#SAP_Application_Server_____-_General)
  - [Advanced Settings](#SAP_Application_Server_____-_Advanced_Settings)

Target System Database (dg%)

  - [General](#Target_System_Database__dg_____General)
  - [Advanced
    Settings](#Target_System_Database__dg_____Advanced_Settings)

## **<span id="data_service_rep_gen"></span>Data Services Repository (%) - General**

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Test Connection</p></td>
<td><p>Click to test the connection to the data source, which verifies the user ID and password.</p></td>
</tr>
<tr class="odd">
<td><p>Name</p></td>
<td><p>Displays the name of the data source registry.</p></td>
</tr>
<tr class="even">
<td><p>Application Data Source Type</p></td>
<td><p>Displays the type of data source (for example, an Oracle Database or a Local File). Refer to the Knowledge Base article &quot;How DSP Applications Use Different Data Source Types&quot; on the BackOffice Associates support site (https://support.boaweb.com) for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Description</p></td>
<td><p>Displays a description of the data source.</p></td>
</tr>
<tr class="even">
<td><p>DS Default Connection</p></td>
<td><p>If checked, the selected Data Services repository is the default Data Services connection for various automated processes. There is only one default Data Services connection.</p></td>
</tr>
<tr class="odd">
<td><p>System</p></td>
<td><p>Displays the server address of the Data Services server.</p></td>
</tr>
<tr class="even">
<td><p>Web Services URL</p></td>
<td><p>Displays the URL to the Data Services web service.</p>
<p><strong>NOTE:</strong> URL supports both http and https.</p></td>
</tr>
<tr class="odd">
<td><p>Repository Name</p></td>
<td><p>Displays the name of the Data Services repository.</p></td>
</tr>
<tr class="even">
<td><p>Authentication</p></td>
<td><p>Displays the type of Authentication used to connect to Data Services.</p></td>
</tr>
<tr class="odd">
<td><p>DS User Name</p></td>
<td><p>Displays the user name used to connect to Data Services.</p></td>
</tr>
<tr class="even">
<td><p>DS Password</p></td>
<td><p>Displays the password used to connect to Data Services.</p></td>
</tr>
<tr class="odd">
<td><p>Requires Web Service Authentication</p></td>
<td><p>If checked, Web Services Authentication is required to connect to this Instance of Data Services. If unchecked, Web Services Authentication is not required.</p></td>
</tr>
</tbody>
</table>

## **<span id="Data_Services_Repository_Advanced_Settings"></span>Data Services Repository (%) – Advanced Settings**

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Command Timeout</p></td>
<td><p>Displays the length of time in seconds that a command can run before timing out. This value is configured via a Data Source registry entry for the Data Services calls for RFC Download Packages. If the field is blank, the timeout is set to 300 seconds.</p>
<p><strong>NOTE:</strong> The recommended setting for the Command Timeout field is 600.</p></td>
</tr>
</tbody>
</table>

## **<span id="External_System_Connection_____-_General"></span>External System Connection (%) - General**

**NOTE:** The Advanced Settings for the External System Connection type
only need to be populated if the data source type is OleDb or ODBC.

Field

Description

Test Connection

Click to test the connection to the data source, which verifies the user
ID and password.

Recompile Data Sources

Click to verify the data is available in the database.

**NOTE:** Objects should only be recompiled for SQL Server databases
created for the project. Objects may need to be recompiled a few times.
If the recompile fails after three attempts, submit an issue to
BackOffice Support.

**NOTE:** This feature is not used for OleDb and ODBC data source types.

Append Columns

This feature is used for local SQL data sources only.

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
Tables](../../WebApp_Dev/Add%20Reserved%20Columns%20%20to%20Tables.htm)
in System Administration for more information.

**NOTE:** This feature is not used for OleDb and ODBC data source types.

Name

Displays the name of the data source.

Application Data Source Type

Displays the type of data source (for example, an Oracle Database or a
Local File). Refer to the Knowledge Base article "How DSP Applications
Use Different Data Source Types" on the BackOffice Associates support
site (https://support.boaweb.com) for more information.

Active

If checked, the data source is active. If unchecked, the data source is
inactive, and system views are not created for the data source.

Data Source Type

Displays the database type of the data source.

Values are:

  - ODBC

  - OleDB
    
    **NOTE:** The fields on the Advanced tab are required for the two
    data source types above.

  - Oracle

  - SqlServer

Server Address

Displays the server address of the data source.

The Server Address combo box contains the server address from data
sources registered in the Platform and in Common.

To add a new server address, type the address in this field and click
**Use this value**.

Database

Displays the database name of the data source.

The Database name must be the name of the database exactly as it appears
in the database. For Oracle databases, the Database name appears in the
TNS name file.

If this field is populated, the Database Instance Name on the Advanced
Settings tab must be blank.

User ID

Displays the User ID used to connect to the data source.

Password

Displays asterisks representing the password used to connect to the data
source.

Database Settings

**NOTE:** A user must have access to System Administration to access the
pages in this section.

Audit

Click to open the *Audit Configuration* page in System Administration to
enable auditing for specific tables in the database. This icon is only
enabled for SQL Server data sources if the data source is protected
(i.e., if the Protected check box on the *Vertical* View of the *Data
Sources* page is checked)

Index

Click to open the *Index (Specification)* page in System Administration
for this data source. This icon is disabled if the data source is not
Microsoft SQL Server and it is not protected (i.e., if the Protected
check box on the *Vertical* View of the *Data Sources* page is
unchecked).

Instances

Click to open the *Data Source Instances* page in System Administration
to add, edit and delete instances for the data source

Encryption

Click to open the *Data Source Column Encryption* page in System
Administration to enable or disable encryption for a specific field
within a database table. This icon is disabled if the data source is not
Microsoft SQL Server and it is not protected (i.e., if the Protected
check box on the *Vertical* View of the Data Sources page is
unchecked).

## **<span id="External_System_Connection_______Advanced_Settings"></span>External System Connection (%) – Advanced Settings**

**NOTE:** The Advanced Settings for the External System Connection type
only need to be populated if the data source type is OleDb or ODBC.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Connection Timeout</p></td>
<td><p>Displays the number of seconds until the connection times out and the DSP® displays an error message stating that to wait before considering the connection failed. Generally, this value does not need to be changed to a value higher than 30 seconds, and adjustment to values above that should be made after checking with BackOffice Product Support.</p></td>
</tr>
<tr class="odd">
<td><p>Command Timeout</p></td>
<td><p>Displays the number of seconds until the command times out, the execution of the command fails, and the DSP displays a notification about the error. Insufficient command timeouts are the main cause of timeout errors in DSP and this parameter may be increased to a high value to accommodate long running processes.</p></td>
</tr>
<tr class="even">
<td><p>Database Type</p></td>
<td><p>Displays the type of database to connect to. This is required if the database type is ODBC or OleDB.</p></td>
</tr>
<tr class="odd">
<td><p>Trusted Connection</p></td>
<td><p>If checked, if the Server is configured to connect using Windows Authentication, the connection will use the hosting machine’s information to authenticate the connection and bypass the usage of the User ID and Password fields.</p></td>
</tr>
<tr class="even">
<td><p>DSN</p></td>
<td><p>Displays the Data Source Name (DSN) parameter, which can be used when the connection to the data source is not a SQL server connection. It is used primarily when defined by the web server control panel, or if the SQL server connection requires additional special parameters not supplied by the DSP standard connection.</p></td>
</tr>
<tr class="odd">
<td><p>Driver</p></td>
<td><p>This field is not used.</p></td>
</tr>
<tr class="even">
<td><p>DBQ</p></td>
<td><p>This field is not used.</p></td>
</tr>
<tr class="odd">
<td><p>Connection String</p></td>
<td><p>Displays the connection string for this data source.</p></td>
</tr>
<tr class="even">
<td><p>Audit Data Source ID</p></td>
<td><p>Displays the DataSourceID used for auditing.</p></td>
</tr>
<tr class="odd">
<td><p>Port</p></td>
<td><p>Displays the port number of the connection.</p>
<p>Some databases can be configured to run on the non-default port. The Port field allows users to enter the server that uses a different port. Also, the Port field is used for FTP connections to define the target port.</p></td>
</tr>
<tr class="even">
<td><p>Protected</p></td>
<td><p>If checked, the Data Source is protected (as in, read only) and features that make changes to the Data Source are hidden/disabled (e.g., Recompile Objects, Append System Columns, building System Views, indexing, auditing, encryption, and building WebApps).</p></td>
</tr>
<tr class="odd">
<td><p>Database Instance Name</p></td>
<td><p>Displays the name of the database instance. For Oracle it's the SID. If this field is populated, the Database field on the General tab must be blank.</p></td>
</tr>
<tr class="even">
<td><p>Procedure Parameter Name Prefix</p></td>
<td><p>Displays the prefix for the procedure parameter name. To prevent conflicts with table/view column names when writing a stored procedure, parameters are usually prefixed. By registering this prefix at the data source level, DSP will add the prefix to the column name when passing parameters to a stored procedures.</p></td>
</tr>
<tr class="odd">
<td><p>System Views</p></td>
<td><p>If checked, Systems Views are created in the data source by DSP. System Views are views that are installed by the Platform in a data source that links back to certain tables or views in the CranSoft database.</p>
<p>This feature is often used for advanced WebApp development.</p>
<p>If unchecked, Systems Views are not created in the data source by DSP®.</p></td>
</tr>
<tr class="even">
<td><p>Net Connection String</p></td>
<td><p>This field is not used.</p></td>
</tr>
</tbody>
</table>

<span id="IG_Universal_Connect_(%)_—_General_Tab"></span>

## <span id="IG"></span>IG Universal Connect (%) — General tab

Field

Description

Test Connection

Click to test the connection to Boomi using the credentials supplied
below. The Boomi Account Name is populated if it does not already exist
in the field.

Name

Displays the name of the data source.

Application Data Source Type

Displays the data source type for the application. The naming convention
indicated by (%) means that any character can be used in the name.

Boomi API Configuration

Boomi Account Name

Displays the name of the Boomi account.

Click the Test Connection icon in the Page toolbar to populate this
field if it is blank.

Boomi Api End Point

Displays the endpoint URL used to call the Boomi AtomSphere API.

Boomi Account ID

Displays the unique identifier for the account.

**NOTE:**This information can be found in Boomi by clicking the active
account name \> Setup \> Account Information.

Boomi User ID

Displays the user ID tied to the Boomi account.

Boomi Password

Displays asterisks representing the password for the Boomi account.

Boomi Default Atom

Displays the atom, the default execution environment where the Process
runs.

Each DSP Server has its own atom.

Optional Proxy Settings

Boomi Proxy Server

Displays the URI of the proxy server, if one is used.

Boomi Proxy User Name

Displays the user name for the proxy server account.

Boomi Proxy Password

Displays asterisks representing the password for the proxy server
account.

<span id="IG_Universal_Connect_(%)_—_Advanced_Settings_Tab"></span>

## <span id="IG2"></span>IG Universal Connect (%) — Advanced Settings tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Connection Timeout</p></td>
<td><p>Displays the maximum time in seconds that the Boomi Process can run before returning a status. After this time passes with no response, a timeout error occurs and the Process stops.</p>
<p>The default value is 100 seconds.</p></td>
</tr>
<tr class="odd">
<td><p>Command Timeout</p></td>
<td><p>Displays the maximum time in seconds that:</p>
<ul>
<li>The API call waits to get a response from Boomi</li>
<li>The first step in the IG Universal Connect template has started (as indicated by a status message returned to the ttBoomiStatus table)</li>
</ul>
<p>If there is no response, a timeout error occurs. The default value is 86400 seconds (24 hours).</p></td>
</tr>
</tbody>
</table>

## **<span id="Local_Utility_Database_____-_General"></span>Local Utility Database (%) - General**

## **<span id="Migration_Object_Database__dsw_____General"></span>Migration Object Database (dsw%) – General**

## **<span id="Migration_Source_Database__sdb_____General"></span>Migration Source Database (sdb%) – General**

## **<span id="Target_System_Database__dg_____General"></span>Target System Database (dg%) – General**

Field

Description

Test Connection

Click to test the connection to the data source, which verifies the user
ID and password.

Recompile Data Source

Click to verify the data is available in the database.

**NOTE:** Objects should only be recompiled for SQL Server databases
created for the project. Objects may need to be recompiled a few times.
If the recompile fails after three attempts, submit an issue to
BackOffice Support.

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

Refer to Append BOA Reserved Columns to Tables for more information.

**NOTE:** This feature is used for local SQL data sources only.

Name

Displays the name of the datasource.

Application Data Source Type

Displays the type of data source (for example, an Oracle Database or a
Local File). Refer to the Knowledge Base article "How DSP Applications
Use Different Data Source Types" on the BackOffice Associates support
site (https://support.boaweb.com) for more information.

Server Address

Displays the server address of the data source.

The Server Address combo box contains the server address from data
sources registered in the Platform and in Common. This list can be used
as suggestions where an existing server address can be selected. To add
a new server address, type the address in tthis field and click **Use
this value**.

Database

Displays the database name of the data source.

The Database name must be the name of the database exactly as it appears
in the database. For Oracle databases, the Database name appears in the
TNS name file.

If this field is populated, the Database Instance Name on the Advanced
Settings tab must be blank.

User ID

Displays the User ID used to connect to the data source.

Password

Displays asterisks representing the password used to connect to the data
source.

System Type

Displays the System Type, which includes the data dictionary, schema and
relationship information about external systems used by DSP®.
Information captured for System Types includes table and field
descriptions, field properties, primary keys, lookup tables, and join
relationships.

**NOTE:** This field displays for the Migration Source Database (.sdb)
only.

Database Settings

**NOTE:** A user must have access to System Administration to access the
pages in this section.

Audit

Click to open the *Audit Configuration* page in System Administration to
enable auditing for specific tables in the database. This icon is only
enabled for SQL Server data sources if the data source is protected
(i.e., if the Protected check box on the Vertical View of the Data
Sources page is checked).

Index

Click to open the *Index (Specification)* page in System Administration
for this data source in System Administration. This icon is disabled if
the data source is not Microsoft SQL Server and it is not protected
(i.e., if the Protected check box on the Vertical View of the Data
Sources page is unchecked).

Instances

Click to open the *Data Source Instances* page in System Administration
to add, edit and delete instances for the data source.

Encryption

Click to open the *Data Source Column Encryption* page in System
Administration to enable or disable encryption for a specific field
within a database table. This icon is disabled if the data source is not
Microsoft SQL Server and it is not protected (i.e., if the Protected
check box on the *Vertical* View of the *Data Sources* page is
unchecked).

## **<span id="Local_Utility_Database_______Advanced_Settings"></span>Local Utility Database (%) – Advanced Settings**

## **<span id="Migration_Object_Database__dsw_____Advanced_Settings"></span>Migration Object Database (dsw%) – Advanced Settings**

## **<span id="Migration_Source_Database__sdb_____Advanced_Settings"></span>Migration Source Database (sdb%) – Advanced Settings**

## **<span id="Target_System_Database__dg_____Advanced_Settings"></span>Target System Database (dg%) – Advanced Settings**

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Connection Timeout</p></td>
<td><p>Displays the number of seconds until the connection times out and the DSP displays an error message stating that the connection failed. Generally, this value does not need to be changed to a value higher than 30 seconds, and adjustment to values above that should be made after checking with BackOffice Product Support.</p></td>
</tr>
<tr class="odd">
<td><p>Command Timeout</p></td>
<td><p>Displays the number of seconds until the command times out, the execution of the command fails, and the DSP displays a notification about the error. Insufficient command timeouts are the main cause of timeout errors in DSP and this parameter may be increased to a high value to accommodate long running processes.</p></td>
</tr>
<tr class="even">
<td><p>Trusted Connection</p></td>
<td><p>If checked, if the Server is configured to connect using Windows Authentication, the connection uses the hosting machine’s information to authenticate the connection and bypass the usage of the User ID and Password fields.</p></td>
</tr>
<tr class="odd">
<td><p>DSN</p></td>
<td><p>Displays the Data Source Name (DSN) parameter which can be used when the connection to the data source is not a SQL server connection. It is used primarily when defined by the web server control panel, or if the SQL server connection requires additional special parameters not supplied by the DSP standard connection.</p></td>
</tr>
<tr class="even">
<td><p>Database Instance Name</p></td>
<td><p>Displays the name of the database instance. For Oracle it's the SID. You must leave the Database field blank to use this feature.</p>
<p>If this field is populated, the Database field on the General tab must be blank.</p></td>
</tr>
<tr class="odd">
<td><p>System Views</p></td>
<td><p>If checked, the Platform injects specific system views into the database. This feature is often used for advanced WebApp development.</p>
<p>System Views are views that are installed by the Platform in a data source that link back to certain tables or views in the CranSoft database.</p></td>
</tr>
</tbody>
</table>

## <span id="SAP_Application_Server_____-_General"></span>SAP Application Server (%) - General

Use this tab to [Establish a Connection to a Target
System](../Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm).

Field

Description

Test Connection

Click to test the connection to the data source, which verifies the
database User ID and Password are connected to the database.

Name

Displays the name of the data source.

Application Data Source Type

Displays the type of data source (for example, an Oracle Database or a
Local File). Refer to the Knowledge Base article "How DSP Applications
Use Different Data Source Types" on the BackOffice Associates support
site (https://support.boaweb.com) for more information.

SAP System ID

Displays a three-character alpha-numeric identifier for the SAP System.

Application Server

SAP Application Server

Displays the name of the server where SAP is installed.

**NOTE:** An Administrator can connect directly to the Application
Server using this method. Alternatively, an Administrator can use a
Message Server to connect dynamically to the Application Server based on
Server resources. Only one type of connection, direct or through a
Message Server, can be created for an SAP connection.

Refer to [Establish a Connection via a Direct Connection to the
Application
Server](../Use_Cases/Establish_a_Connection_Direct_Connection.htm)  for
more information.

SAP System Number

Displays a two character integer that identifies the SAP instance, used
as a parameter in the SAP GUI Logon client when configuring the SAP
connection. The SAP System Number displays in SAP on the *SAP GUI Change
Item* screen.

Message Server

SAP Message Server

Displays the name of the message server.

**NOTE:** Connecting to SAP via a Message Server uses load balancing to
manage Server resources. Load Balancing dynamically distribute the SAP
users to application server instances when connecting to the Application
Server. Only one type of connection, direct or through a Message Server,
can be created for an SAP connection.

**NOTE:** Refer to [Establish a Connection via a Message
Server](../Use_Cases/Establish_a_Connection_via_a_Message_Server.htm)
 for more information.

SAP Logon Group

Displays the logon group name for the message server if SAP Load
Balancing is used to download SAP tables from the source via RFC. Refer
to SAP documentation for details about Load Balancing.

Default Credentials

SAP Client

Displays the SAP client number.

SAP Language

Displays the language of the SAP instance and the SAP Language Code.

The language is used when SAP interfaces with the platform and is used
when logging in to SAP.

SAP User ID

Displays the user name the connection uses when logging in to SAP.

SAP Password

Displays asterisks to represent the user password the connection uses
when logging in to SAP.

User Credentials

Click to open the <span style="font-style: italic;">[Data Source
Registry User
Credentials](Data_Source_Registry_User_Credentials_H.htm)</span> page to
add user credentials to log in to SAP to specific user accounts.

Refer to [Add User Credentials to an SAP Connection for a Specific
User](../Use_Cases/Add_User_Credentials_to_an_SAP_Connection_for_a_Specific_Use.htm)
for more information.

RFC

RFC Functions

Click to open the <span style="font-style: italic;">[SAP Connections:
RFCs](SAP_RFC.htm)</span> page to view a list of RFCs enabled in the SAP
System and a description of each.

The list displays after a user clicks the RFC Extracts icon.

RFC Extract

Click to retrieve a list of all RFCs enabled in the SAP system.

After the extract is complete, click the RFC Functions icon to view the
extracted RFCs.

**NOTE:** RFCs must be extracted before the first BAPI/RFC template type
can be created.

Other

SAP Default Connection

If checked, this SAP connection is used by default when posting using
the Application Data Source Type of <span style="color: #333333;">SAP
Application Sever (%).</span>

SAP Max Pool Size

Displays a value to specify how many RFC connections are left open for
the current user, even if the connections are not being used actively. A
pooled RFC connection is allocated much faster than a new connection.
Therefore, increasing the pool size minimizes the time needed to get a
new connection.

However, if a connection is pooled, it is not available for other users.
Typically, ABAP backend systems define an upper limit for the number of
RFC connections. If this number has been fully allocated by pooled
connections, then new users requesting a new connection may not succeed
because the maximum number of connections allowed by the ABAP system has
already been allocated.

Typically, the maximum pool size is kept very low and may even be set to
0. If there are substantially fewer concurrent users than the number of
concurrent RFC connections to an ABAP system, then increase the pool
size to improve performance.

The recommended setting for Max Pool Size is 10 in highly parallel
environments.

## <span id="SAP_Application_Server_____-_Advanced_Settings"></span>SAP Application Server (%) - Advanced Settings

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>SAP File Data Source ID</p></td>
<td><p>Displays the data source remote file type that must be used for asynchronous postings for user defined templates. Files must be physically transferred to the SAP system via FTP, UNC or HTTP for these posting types.</p></td>
</tr>
<tr class="odd">
<td><p>SAP Use Namespace</p></td>
<td><p>If checked, the platform uses the namespace version of the BOA Function Module. If unchecked, the platform uses the non-namespace version of the BOA Function Module.</p>
<p><strong>NOTE:</strong> The namespace concept describes how customers and partners name their development objects to avoid overlapping when SAP software is upgraded. BDC Function Modules and BAPI Function Modules can be namespace or non-namespace objects.</p></td>
</tr>
<tr class="even">
<td><p>SAP All Clients</p></td>
<td><p>If checked, data is downloaded in Collect for all clients in the SAP instance. This setting is used for RFC and SAP Text data downloads when more than one SAP client is required to download data.</p>
<p>If unchecked, data is downloaded for the client associated with this data source only.</p></td>
</tr>
<tr class="odd">
<td><p>SAP Remove Client From Key</p></td>
<td><p>If checked, builds primary keys without the client field (usually MANDT). This feature can be used if only 1 client is downloaded (as in, the All Clients check box is unchecked) for RFC and SAP Text data downloads.</p></td>
</tr>
</tbody>
</table>
