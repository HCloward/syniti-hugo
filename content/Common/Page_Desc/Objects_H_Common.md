+++
title = 'Objects H'
solution = 'Platform'
+++

# Objects H

[Objects V All Tabs](#Objects_V__All_Tabs_)

<div class="use">

Use this page to [Register Objects](../Use_Cases/Register_Objects).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Common \> Analyze</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Duplicates</span> icon
    for a data source.

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
<td><p>Columns</p></td>
<td><p>Click to specify columns to be analyzed for duplicate records.</p></td>
</tr>
<tr class="odd">
<td><p>Results</p></td>
<td><p>Click to view duplicate results for the object.</p></td>
</tr>
<tr class="even">
<td><p>BDD</p></td>
<td><p>Click to open the <em>Bulk Duplicate Detection</em> page in System Administration to view details about the search tables used in duplicate detection.</p>
<p><strong>NOTE</strong>: A user must have access to System Administration to access this page.</p></td>
</tr>
<tr class="odd">
<td><p>OBJECT</p></td>
<td><p>Displays name of object being analyzed for duplicate records.</p></td>
</tr>
<tr class="even">
<td><p>Build</p></td>
<td><p>Click to find duplicate records.</p></td>
</tr>
<tr class="odd">
<td><p>RECORD COUNT</p></td>
<td><p>Displays number of records returned by the duplicate detection process.</p></td>
</tr>
<tr class="even">
<td><p>CANDIDATES</p></td>
<td><p>Displays count of potential duplicate records in the data source.</p></td>
</tr>
<tr class="odd">
<td><p>Unresolved Candidates</p></td>
<td><p>Displays count of duplicate candidates that are not yet resolved. Click to resolve duplicate candidates.</p></td>
</tr>
<tr class="even">
<td><p>RESOLVED CANDIDATES</p></td>
<td><p>Displays count of resolved duplicates in the data source.</p></td>
</tr>
<tr class="odd">
<td><p>PERCENT RESOLVED</p></td>
<td><p>Displays percent of total duplicate candidates that have been resolved.</p></td>
</tr>
</tbody>
</table>

## <span id="Objects_V__All_Tabs_"></span>Objects V (All Tabs)

[Objects H](Objects_H_Common)

<div class="use">

Use this page to [Register Objects](../Use_Cases/Register_Objects).

</div>

This page contains the following tabs:

  - [General tab](#General_Tab)
  - [Actions tab](#Actions_Tab)
  - [Duplicate Detection Results tab](#Duplicate_Detection_Results_Tab)

## <span id="General_Tab"></span>General tab

Field

Description

Dictionaries

Click to open the *Dictionaries* page in System Administration to add,
edit and delete dictionary entries. Users must have access to System
Administration to manage dictionaries.

Stop List

Click to open the *Stop Lists* page in System Administration to add,
edit and delete stop list entries. Users must have access to System
Administration to manage stop lists.

BDD

Click to open the *Bulk Duplicate Detection* page in System
Administration to run the bulk duplicate detection administration
process for the object.

**NOTE:** Users must have access to System Administration to run
duplicate detection.

Object Settings

Object

Displays name of object being analyzed for duplicate records.

View Name

Displays name of object. Click to view details about the object.

View

Click to open the Objects page to view object’s data.

Advanced Settings

Search ID

Displays ID of the search table that controls which record pairs in the
source data are stored as a duplicate. The DSP® is delivered with a
default search table, DSPCommon.ttDuplcate, that has been set up for the
BDD process.

**NOTE**: If a search table other than DSPCommon.ttDuplicate is to be
used, it must be set up in System Administration.

Non Searchable Characters

Displays characters excluded from the duplicate detection search.

Stop List ID

Displays ID for list of words ignored during the duplicate detection
search. Default value is managed in Configuration \> Modules \>
Parameters-Duplicates.

Search Threshold

Displays level to ignore false positives.

Duplicate Detection Threshold

Displays weight percent of the calculated value for matched words. Words
that match carry more weight than words that sound alike. Default value
is managed in Configuration \> Modules \> Parameters-Duplicates.

Synonym Weight

Displays weight value of synonym matches.

Sound Ex Weight

Displays percentage of combined calculated value for words found within
the search (number of words found plus the number of words that sound
alike divided by the total number of words). Words that match carry more
weight than words that sound alike.

Custom Sound Ex Function ID

Displays ID for custom SQL Server Sound Ex function. Selecting a custom
function improves accuracy of duplicate detection, but consequently,
decreases performance.

Index Batch Size

Displays number of records to process in one pass through the data.
Default valus is **1000**.

Duplicate Detection Batch Size

Displays number of records queued up in the duplicate detection process.
This field allows a subset of large files to be processed and at the
same time, limits the resources required.

Word Ratio Threshold

Displays number of words in each duplicate pair. A value less than 50%
marks a duplicate value for removal. For example, if A has 10 words and
B has 1 word, which matches on one of A’s words, then A-B matches 10%,
but B-A matches 100%. This 100% is the false positive; the Word Ratio
will remove this as a potential match. Default value is managed in
Configuration \> Modules \> Parameters-Duplicates.

Remove Blank Lines

Click to remove blank lines from the HTML formatted output in the
*[Candidates](Candidates)* page. This action makes each object block
smaller because white space is removed. When comparing objects with
multiple lines, such as address data, multiple lines may cause the data
to not line up on the page. If needed, the Remove Blank Lines check box
can be disabled and the object can be re-built. Default value is managed
in Configuration \> Modules \> Parameters-Duplicates.

Unicode Separate Characters

If enabled, Unicode characters (double-byte) are included in the
duplicate detection
process.

## <span id="Actions_Tab"></span>Actions tab

|               |                                                                                                                                                                                                                                                                                                                              |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field         | Description                                                                                                                                                                                                                                                                                                                  |
| Build         | Click to find duplicates.                                                                                                                                                                                                                                                                                                    |
| History       | Click to open the <span style="font-style: italic;">[Object History](Object_History_H)</span> page to view details on previous builds (i.e., duplicate searches) for the object.                                                                                                                                         |
| Reset Status  | Click to change the status of the build from Processing to Procedures Completed. Only reset status if the build process is aborted and the status is still processing                                                                                                                                                        |
| Reset Results | Click to remove all previous duplicates and non-duplicate results for the object. Button is only available for objects that returned duplicates (which display on the *[Results](Results)* page). This action is not reversible; it is recommended to back up the drResultsDuplicate table before the results are reset. |
| Post Process  | Click to continue running a stopped process.                                                                                                                                                                                                                                                                                 |

## <span id="Duplicate_Detection_Results_Tab"></span>Duplicate Detection Results tab

|                                    |                                                                                                     |
| ---------------------------------- | --------------------------------------------------------------------------------------------------- |
| Field                              | Description                                                                                         |
| Duplicate Detection Status         | Displays current status of the duplicate detection build process.                                   |
| Duplicate Detection Records        | Displays number of records to be processed.                                                         |
| Duplicate Detection Processed      | Displays actual number of records processed at this point in time; value changes during processing. |
| Duplicate Detection Queued         | Displays number of records that still need to be processed.                                         |
| Duplicate Detection Duplicates     | Displays number of records marked as duplicates.                                                    |
| Duplicate Detection Execution Time | Displays time to run the duplicate detection process.                                               |
