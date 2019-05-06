# Audit Tables H

[Audit Tables V](#Audit)

<div class="use">

Use this page to:

  - [Enable Audit Trail on a
    Page](../../WebApp_Dev/Enable_Audit_Trail_on_a_Page.htm)
  - [Drop Audit Tables](../../WebApp_Dev/Drop_Audit_Tables.htm)

</div>

To access this page in System Administration:

1.  Click **Data Sources** in the *Navigation* pane.
2.  Click the **Audit** icon for a data source.
3.  Click the **Tables** icon.

<table>
<thead>
<tr class="header">
<th style="text-align: left;"><p>Field</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="text-align: left;">TABLE NAME</td>
<td><p>Displays the name of the audited data source table.</p></td>
</tr>
<tr class="even">
<td style="text-align: left;"><p>ENABLE AUDITING</p></td>
<td><p>If checked, an audit trail is enabled for the table.</p></td>
</tr>
<tr class="odd">
<td style="text-align: left;"><p>AUDIT PROCEDURES</p></td>
<td><p>If checked, a record of every stored procedure that runs against a record as part of a DSP Page Event is maintained in the audit tables.</p></td>
</tr>
<tr class="even">
<td style="text-align: left;"><p>BUILD AUDIT TABLES</p></td>
<td><p>Click to create audit tables in the specified Data Source to track changes to the selected user table.</p>
<p><strong>NOTE:</strong> Once the tables are built, the Snapshot Data button is active.</p></td>
</tr>
<tr class="odd">
<td style="text-align: left;"><p>SNAPSHOT DATA</p></td>
<td><p>Click to create a copy of the tables with a snapshot of the data currently in the table. This process must be run after creating the audit tables. When a record is edited, the audit trail records both the before and the after values. However, the trail only shows values that are edited. Snapshot Data can be viewed as an insert for existing records. If the audit is enabled after the table has values in it, the trail has no way of telling where the data came from, so the snapshot is a way of verifying that some data existed prior to auditing.</p></td>
</tr>
<tr class="even">
<td style="text-align: left;"><p>CHECK COLUMNS</p></td>
<td><p>Click to report any differences between the columns in the table and the audit table. When the audit tables are built, all the columns from the table that are being audited are included. However, it is possible to have a case where the columns in the table and the audit tables do not match. There can be two reasons for the misalignment:</p>
<ul>
<li>The Designer deliberately removed some columns from the audit table because those values should not be audited.</li>
<li>The Designer added columns to the table after the audit tables were built and forgot to manually update the audit tables.</li>
</ul></td>
</tr>
</tbody>
</table>

## <span id="Audit"></span>Audit Tables V

[Audit Tables H](#)

Field

Description

Table Name

Displays the name of the audited data source table.

Drop Tables

Request Drop

Click to request that the audit tables be dropped. Another user with
Administrator rights must confirm within 24 hours before the audit
tables can actually be dropped.

Drop Requested By

Displays the name of the user who requested that the audit tables be
dropped.

Drop Requested On

Displays the date on which a user requested that the audit tables be
dropped.

Drop Audit Tables

Click to drop the audit tables. This button is enabled after another
user with Administrator rights requests that the audit tables be
dropped.
