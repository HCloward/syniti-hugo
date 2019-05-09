+++
title = 'Indices H'
solution = 'Platform'
+++

# Indices H

[Indices V](#Indices)

<div class="use">

Use this page to:

  - [Populate an index](../Use_Cases/Populate%20an%20Index)
  - [Stop a Running Index](../Use_Cases/Stop%20a%20Running%20Index)

</div>

To access this page, select **Admin \> Resources \> Indices** in the
*Navigation*
pane.

|               |                                                                                                          |
| ------------- | -------------------------------------------------------------------------------------------------------- |
| Field         | Description                                                                                              |
| DATABASE      | Displays the name of the database that stores the table that is indexed.                                 |
| TABLE         | Displays the name of the table that is indexed.                                                          |
| PREVIOUS TIME | Displays the amount of time in seconds that it took the last indexing process to complete for the table. |
| ACTIVE        | If enabled, the table index is active and is fully indexed.                                              |
| START         | Click to start the index process.                                                                        |
| STOP          | Click to stop the running index.                                                                         |
| Failed Log    | Click to view a log of indexing failures.                                                                |
| All Jobs      | Click to view all indexing jobs that have run.                                                           |

## <span id="Indices"></span>Indices V

[Indices H](#top)

This page has the following tabs:

  - [General](#General)
  - [Search Options](#Search)

### <span id="General"></span>General tab

Field

Description

Index Information

Database

Displays the name of the database that stores the table that is indexed.

Table

Displays the name of the table that is indexed.

Duplicate Detection Batch Size

Displays number of records queued in the duplicate detection process.
This field allows a subset of large files to be processed and at the
same time, limits the resources required.

Duplicate Detection Status

Displays current status of the bulk duplicate detection process. Values
are: Not Running, Processing and Process Complete.

Duplicate Detection Records

Displays the total number of records in the \[tablename\]\#Duplicate
table.

Duplicate Detection Processed

Displays number of records in the table that have been processed for
bulk duplicate detection.

Duplicate Detection Queued

Displays the number of records queued. Initially, this is the Duplicate
Detection Batch Size. As the process runs, this number decreases and the
Duplicate Detection Processed number increases.

Duplicate Detection Duplicates

Displays the number of duplicate records detected in the table.

### <span id="Search"></span>Search Options tab

<table>
<tbody>
<tr class="odd">
<td><p>Fields</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Search ID</p></td>
<td><p>Displays the table containing the index used for the search.</p></td>
</tr>
<tr class="odd">
<td><p>Duplicate Detection Search ID</p></td>
<td><p>Displays the table containing the index used for bulk duplicate detection.</p></td>
</tr>
<tr class="even">
<td><p>Duplicate Detection Binding Field Names</p></td>
<td><p>Displays the Binding Fields used for Bulk Duplicate Detection.</p>
<p>This field is similar to the Binding Fields when defining a Link To another page on a column.</p>
<p>By default the DSP® joins the page's view to the page's duplicate detection table using primary keys. It is possible to override this default and use custom joining fields by configuring this setting (e.g. TableColumnName=IndexColumnName). This featere is typically used when using a Request page, but enabling search against an SAP data set. The Duplicate Detection process checks against a different table than the current page's table to avoid duplicating data in the target.</p></td>
</tr>
</tbody>
</table>
