+++
title = 'Targets H'
solution = 'Platform'
+++

# Targets H

[Targets V](#Targets_V)

<div class="use">

Use this page to [Register
Targets](../Use_Cases/Register_and_Use_Targets.htm#Register_Targets).

</div>

To access this page, click <span style="font-weight: bold;">Collect \>
Targets</span> in <span style="font-style: italic;">Navigation</span>
pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Test Connection</p></td>
<td><p>Click to test the connectivity to a data source, which verifies the database User ID and Password login is connected to the target database. Does not test the validity of the SAP login credentials or DSN connection.</p></td>
</tr>
<tr class="odd">
<td><p>Refresh</p></td>
<td><p>Click to manually extract a copy of data from all registered sources and load into target. </p>
<p><strong>NOTE</strong>: If the data in the target has been purged manually, or the retention expiration date for that object has passed, it cannot be refreshed and this icon is inactive. Refer to <a href="../Use_Cases/Support_Regulatory_Compliance.htm#Purge_Data">Purge Data</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>TARGET</p></td>
<td><p>Displays database target where tables are refreshed with source data.</p></td>
</tr>
<tr class="odd">
<td><p>CONNECTION TYPE</p></td>
<td><p>Displays valid database connection type from source to target. Connection Types are configured under Configuration &gt; Connection Types.</p></td>
</tr>
<tr class="even">
<td><p>SCHEMA OWNER</p></td>
<td><p>Displays the schema of the target database that contains the tables. The SCHEMA OWNER doesn’t have to match database user ID.</p></td>
</tr>
<tr class="odd">
<td><p>Sources</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Target_Sources_H_Collect.htm">Target Sources</a></span> page to register source database where data is refreshed from and stored in the target.</p></td>
</tr>
<tr class="even">
<td><p>Metrics</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Target_Source_Metric_Charts.htm">Target Source Metric Charts</a></span> page to view monthly, weekly and daily download results for target/source combination.</p></td>
</tr>
</tbody>
</table>

## <span id="Targets_V"></span>Targets V

[Targets H](Targets_H_Collect.htm)

This page has two tabs:

  - [General](#General)
  - [Data Protection](#Data)

<span id="General_Tab"></span>

## <span id="General"></span>General tab

<div class="use">

Use this tab to [Register
Targets](../Use_Cases/Register_and_Use_Targets.htm#Register_Targets).

</div>

Field

Description

Target

Displays database where tables are refreshed with source data.

Connection Type

Displays valid database connection type from source to target.
Connection Types are configured under Configuration \> Connection Types.

Schema Owner

Displays the schema of the target database that contains the tables. The
Schema Owner doesn’t have to match database user ID.

Collation Type

Displays language option for text data in the target  database.

Values are: General Latin Case-insensitive, General Latin Case-sensitive

Default value is **General Latin Case-insensitive**, which means the
collation uses Latin characters and is case insensitive.

Refresh Index Option

Displays the options to build indices or the primary key of registered
tables. Select an option to increase download and network performance.

Values are: Build Indices and Primary Keys, Build Indices only, Do Not
Build Indices and Primary Keys. Default value is **Do Not Build Indices
and Primary Keys**.

Description

Displays additional information about the target, e.g., DBA or business
contact information, or when the target can be deleted from server.

Data Services ID

Displays the Data Services repository instance assigned to the target,
which instructs Collect to use the Data Services instance for the
creation and execution of packages. Click the link to view data service
configuration, which is managed in Common \> Configuration \> Data
Source Registry.

Sources

Click to open the <span style="font-style: italic;">[Target
Sources](Target_Sources_H_Collect.htm)</span> page to register source
database where data is refreshed from and stored in the target.

General Information

Refresh Started On

Displays date and time when the manual refresh started.

Refresh Completed On

Displays date and time when the manual refresh completed.

Test Connection Status

Displays results from the most recent test connection, either from the
Service page or when the Test Connection icon was clicked

Test Connection On

Displays date and time of most recent test connection.

Action

Build Index

Click to schedule the rebuild process for all indices in the Target
Source Table index. Only registered indices and keys are rebuilt.

Reset

Click to reset a running refresh. This process activates the Refresh
icon and triggers the batch job schedule to calculate new run dates for
next scheduled refresh. Reset doesn’t impact processes currently
running. Reset the target if download process backs up due to network
problems.

<span id="Data_Protection"></span>

## <span id="Data"></span>Data Protection

<div class="use">

Use this tab to:

  - [Configure Data
    Protection](../Use_Cases/Support_Regulatory_Compliance.htm#Configure_Data_Protection)
  - [Update the Retention Expiration
    Date](../Use_Cases/Support_Regulatory_Compliance.htm#Update_the_Retention_Expiration_Date)
  - [Purge
    Data](../Use_Cases/Support_Regulatory_Compliance.htm#Purge_Data)

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Data Controller</p></td>
<td><p>Displays the user responsible for the processing of personal data in the target.</p>
<p>Any user or group who is assigned the Data Controller role must have a user account in the DSP. Data Controller must have access to the target based on their assigned security role and security key.</p>
<p><strong>NOTE:</strong> The Collect Administrator must check the WORK FLOW SUMMARY check box for the target and Data Controller on the <em><a href="Workflow_Summary_User_Settings.htm">Workflow Summary User Settings</a></em> page. The Data Controller is added to this page automatically. If the check box is not checked, the Data Controller will not receive a warning email that data is going to be purged.</p></td>
</tr>
<tr class="odd">
<td><p>Data Classification</p></td>
<td><p>Displays the nature of the data in the target, identifying whether a target contains personal data and so must be purged.</p>
<p>Options included with the DSP are:</p>
<ul>
<li><strong>Personal</strong> — This object contains data that must be purged by a certain date. The Retention Expiration Date field must be completed for this object (for example, Customer Addresses, Employee Records, Business Partner Tax IDs).</li>
<li><strong>Public</strong> —This object contains data that does not need to be purged (for example, Units of Measure, Material Descriptions, Country Codes).</li>
<li><strong>Restricted</strong> — This data does not need to be purged, but is marked as restricted access (for example, Company Chart of Accounts, Recipes, Work Orders).</li>
</ul>
<p><strong>NOTE</strong>: These options are delivered with the DSP and cannot be updated; however, a Common Administrator can create custom classifications on the Data Classification page in Common. Refer to <a href="../../Common/Use_Cases/Add%20Custom%20Data%20Classifications%20and%20Information%20Types.htm">Add Custom Data Classifications and Information Types</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Retention Expiration Date</p></td>
<td><p>Displays the date when the data in the target, target sources, and tables will be automatically purged when a Service page runs.</p>
<p>A Collect Administrator must enter a date for a target with a data classification of Personal or for any custom classification with the Retention Period Warning feature enabled.</p>
<p>A different retention expiration date can be set at the target source and table level.</p>
<p>If no date is set for the object, the data is not purged.</p>
<p><strong>NOTE:</strong> Updates to this field are audited. An e-signature is required.</p>
<p><strong>NOTE:</strong> Once this data has passed, the Refresh and Build and Refresh icons on the this page, and the <em><a href="Target_Sources_H_Collect.htm">Target Sources</a></em>, and <em><a href="Tables_H.htm">Tables</a></em> pages are inactive. The target can no longer be refreshed either manually or automatically.</p></td>
</tr>
<tr class="odd">
<td><p>Data Collection Reason</p></td>
<td><p>Displays reason for extracting the data. Any time the target is processed, the data should only be used for the reason identified in this field.</p></td>
</tr>
<tr class="even">
<td><p>Purge Data</p></td>
<td><p>Click to manually delete all data in all tables (including check tables) at the target, target source, and table levels.</p>
<p><strong>NOTE:</strong> Data is automatically purged on the Retention Expiration Date when a Service page runs once daily.</p>
<p><strong>NOTE:</strong> After data is purged, the table(s) cannot be downloaded again for the target, and the Collect refresh will not pull data into the table. The Refresh and Build and Refresh icons on the <em>Targets</em>, <em>Target Sources</em>, and <em>Tables</em> pages are inactive.</p></td>
</tr>
</tbody>
</table>
