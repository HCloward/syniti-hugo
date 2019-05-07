+++
title = 'Bulk Duplicate Detection H'
solution = 'Platform'
+++

# Bulk Duplicate Detection H

[Bulk Duplicate Detection
V](Bulk_Duplicate_Detection_H.htm#Bulk_Duplicate_Detection_V)

<div class="use">

Use this page while [Finding
Duplicates](../../Common/Use_Cases/Find_Duplicates_Overview.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Common \></span>**Analyze**
    in the *Navigation* pane.
2.  Click **Duplicates** for Data Source ID.
3.  Select an object.
4.  Click **BDD** on Page
toolbar.

|                               |                                                                                                                                                                                    |
| ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                         | Description                                                                                                                                                                        |
| DATA SOURCE NAME              | Displays name of data source that contains data being inspected for duplicates.                                                                                                    |
| TABLE                         | Displays name of table within data source on which bulk duplicate detection is run.                                                                                                |
| DUPLICATE DETECTION STATUS    | Displays current status of bulk duplicate detection process. Values are: Not Running, Processing and Process Complete.                                                             |
| DUPLICATE DETECTION RECORDS   | Displays total number of records in the table.                                                                                                                                     |
| DUPLICATE DETECTION PROCESSED | Displays number of records in the table that have been processed for bulk duplicate detection.                                                                                     |
| DUPLICATE DETECTION SUSPEND   | If enabled, the bulk duplicate detection process is suspended for the table.                                                                                                       |
| START                         | Click to run the bulk duplicate detection process for the table. This process runs in the background.                                                                              |
| CANCEL                        | Click to cancel a running bulk duplicate detection process. Cancelling a process can take up to 60 seconds. Button is only active if duplicate detection is running for the table. |
| VIEW                          | Click to view the results of the bulk duplicate detection process. Button is only active once the process successfully completes.                                                  |

## <span id="Bulk_Duplicate_Detection_V"></span>Bulk Duplicate Detection V

[Bulk Duplicate Detection H](Bulk_Duplicate_Detection_H.htm)

Field

Description

Table Info

Data Source Name

Displays name of data source that contains data being inspected for
duplicates.

Table

Displays name of table within data source on which bulk duplicate
detection is run.

Statistics

Duplicate Detection Batch Size

Displays the number of records within the table to be processed for bulk
duplicate detection at a given time.

Duplicate Detection Status

Displays current status of bulk duplicate detection process. Values are:
Not Running, Processing and Process Complete.

Duplicate Detection Records

Displays total number of records in the table.

Duplicate Detection Processed

Displays number of records in the table that have been processed for
bulk duplicate detection.

Duplicate Detection Queued

Displays the number of records queued. Initially, this is the Duplicate
Detection Batch Size. As the process runs, this number decreases and the
Duplicate Detection Processed number increases.

Duplicate Detection Duplicates

Displays the number of duplicate records detected in the table.

Duplicate Detection Execution Time

Displays the number of seconds that the bulk duplicate detection process
took to run.

Debug Actions

Clear Duplicates

Click to empty the contents of the table that contains the bulk
duplicate detection information for the table.

Process Batch

Click to queue up a single batch of records and look for duplicates for
each record. Once all the records in the batch have been processed, the
operation terminates.<span> </span>
