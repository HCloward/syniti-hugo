+++
title = 'Source Connection Types H'
solution = 'Platform'
+++

# Source Connection Types H

[Source Connection Types V](#Source_Connection_Types_V)

<div class="use">

Use this page to [Set up Connection
Types](../Config/Set_up_Connection_Types.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Collect \> Administrative \>
    Connection Types</span> in
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Sources</span> for a Target
    Connection Type of SQLSERVER.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>SOURCE CONNECTION TYPE</p></td>
<td><p>Displays database connection type for the source.</p>
<p><strong>NOTE:</strong> Collect only supports SQL Server Source databases. SQL 2012 and 2014 connection types are supported.</p></td>
</tr>
<tr class="odd">
<td><p>OLE PROVIDER</p></td>
<td><p>Displays name of OLE settings.</p></td>
</tr>
<tr class="even">
<td><p>ODBC DRIVER</p></td>
<td><p>Displays name of driver used in the Windows ODBC setup for the DSN.</p></td>
</tr>
<tr class="odd">
<td><p>Data Type Conversions</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Connection_Types_H.htm">Connection Type Data Conversion</a></span> page to manage data type conversions for the source.</p></td>
</tr>
</tbody>
</table>

## <span id="Source_Connection_Types_V"></span>Source Connection Types V

[Source Connection Types H](Source_Connection_Types_H.htm)

<div class="use">

Use this page to [Set up Connection
Types](../Config/Set_up_Connection_Types.htm).

</div>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Source Connection Type</p></td>
<td><p>Displays database connection type for the source.</p>
<p><strong>NOTE:</strong> Collect only supports SQL Server Source databases. SQL 2012 and 2014 connection types are supported.</p></td>
</tr>
<tr class="odd">
<td><p>Fetchsize</p></td>
<td><p>Displays number of records put into a buffer (i.e., the number of records to load into memory to run faster) on the Windows server.</p></td>
</tr>
<tr class="even">
<td><p>Download SQL</p></td>
<td><p>Displays the SQL command used to read non-SAP databases to download table and column information from the source during the Build Package process. The data type conversions are performed during this load process and are followed by the Create Table and Create Keys/Indices process.</p></td>
</tr>
<tr class="odd">
<td><p>Download Table SQL</p></td>
<td><p>Displays the SQL called during Fetch Table process. When the Fetch Table icon on the <span style="font-style: italic;">Target Sources</span><span>page is clicked, Collect uses the SQL entered in the Download Table SQL field to download a list of tables.</span></p></td>
</tr>
<tr class="even">
<td><p>Download Primary Key SQL</p></td>
<td><p>Displays the SQL called during Build Package process. SQL verifies table built from SQL has a primary key. This field is only used for non-SAP sources.</p></td>
</tr>
<tr class="odd">
<td><p>Download Index SQL</p></td>
<td><p>Displays the SQL called during Build Package process. SQL verifies table built from SQL has indices. This field is only used for non-SAP sources.</p></td>
</tr>
<tr class="even">
<td><p>SAP Table Check SQL</p></td>
<td><p>Displays the SQL called during the Build Package process to verify if the table is Transparent, Pooled, Clustered or Other. Tables are not created for objects (views, structures, etc.) marked as “other.”</p></td>
</tr>
<tr class="odd">
<td><p>SAP Column Download SQL</p></td>
<td><p>Displays the SQL called during the Build Package process to download all column information from SAP DD03L table, which is an SAP table that contains column information.</p></td>
</tr>
<tr class="even">
<td><p>SAP Primary Key SQL</p></td>
<td><p>Displays the SQL called during the Build Package process to download all primary key information from SAP DD03L table, which is an SAP table that contains column information.</p></td>
</tr>
<tr class="odd">
<td><p>ODBC Driver</p></td>
<td><p>Displays name of the driver used in the Windows ODBC setup for the DSN.</p></td>
</tr>
<tr class="even">
<td><p>OLE Provider</p></td>
<td><p>Displays name of OLE settings.</p></td>
</tr>
<tr class="odd">
<td><p>Connection String Example</p></td>
<td><p>Displays an example of a connection string for reference.</p></td>
</tr>
<tr class="even">
<td><p>Left Column Delimiter</p></td>
<td><p>Displays character that wraps around special characters in field and table names.</p></td>
</tr>
<tr class="odd">
<td><p>Right Column Delimiter</p></td>
<td><p>Displays character that wraps around special characters in field and table names.</p></td>
</tr>
</tbody>
</table>
