# Create rt Tables From the tt Tables and Create Views for the Custom WebApp

Once each **tt** table is created, use it as a script to create an
**rt** table. Add the following columns to each table.

**NOTE:** The tt table has the ID column as an IDENTITY.  When using the
tt table as a basis for the rt table, the rt table will then also have
the ID column as an IDENTITY when the rt table is created.  In the rt
table,<span> </span> the ArchiveID should be added as IDENTITY. Since a
table can only have one IDENTITY column, the definition of the ID column
has to be changed to not be IDENTITY. These updates to the rt table must
be performed manually.

**NOTE:** ArchiveID column must be set as the PrimaryKey of the rt
Table.

<table>
<tbody>
<tr class="odd">
<td><p>Column Name</p></td>
<td><p>Data Type</p></td>
<td><p>Value</p></td>
</tr>
<tr class="even">
<td><p>ArchiveID</p>
<p>This should be the first column in the table.</p></td>
<td><p>int</p></td>
<td><p>IDENTITY(1,1) NOT NULL</p>
<p> </p></td>
</tr>
<tr class="odd">
<td><p>ID column must have its IDENTITY property removed.</p></td>
<td><p>Int</p></td>
<td><p>NOT NULL</p></td>
</tr>
<tr class="even">
<td><p>PostedOn</p></td>
<td><p>smalldatetime</p></td>
<td><p><span style="font-size: 12.0pt;font-family: Arial, sans-serif;">NULL DEFAULT (getdate())</span></p></td>
</tr>
<tr class="odd">
<td><p>PostedBy</p></td>
<td><p>nvarchar (50)</p></td>
<td><p>NULL</p></td>
</tr>
<tr class="even">
<td><p>Connection</p></td>
<td><p>nvarchar (50)</p></td>
<td><p>NULL</p></td>
</tr>
</tbody>
</table>

For each Data Entry table, create a **tx** view. The **tx** view should
contain all columns from the **tt** table, the WebAppID where the view
resides, and a WHERE clause 'WHERE \[PostError\] \>= 1'.
