# Manage Duplicate Detection

Duplicate Detection is a validation rule included with the DSP® that
uses search engine indexes to find possible duplicate records. Unlike
most validation rules, which are hard coded views residing in the
database, DSP® dynamically builds a derived table at runtime to perform
Duplicate Detection. The derived table is treated much the same way as
any user-defined validation rule. The results of the query display the
same as any other validation results.

The Duplicate Detection validation rule runs as a foreground event,
triggered when:

  - A record is created or modified on a page where Duplicate Detection
    is enabled for a column(s)

**NOTE**: If both search and duplicate detection are used, the user can
enable a validation as a page event that runs in the foreground to check
for duplicates when a single record is added. Refer to [Configure an
Index,](Configure%20an%20Index.htm) [Add a Column to an
Index](Add%20a%20Column%20to%20an%20Index.htm) and [Register a
Validation Rule to a Page](../../WebApp_Dev/ValidationRules.htm) for
more information.

  - A user manually triggers an event that contains the validation rule

**NOTE**: The validation can be assigned to any event, with any severity
or priority. Add a Duplicate Detection validation rule to the OnValidate
event as a warning. Refer to [Create
Events](../../WebApp_Dev/Create_Events.htm) for more information.

The Duplicate Detection validation rule is available for use on a page
if the following criteria have been met:

  - The page must be indexed.
  - Duplicate detection must be enabled on one or more index columns.

Refer to [Build indices for a Data Source for Search and Duplicate
Detection](Build%20Indices%20for%20a%20Data%20Source%20for%20Search%20and%20Duplicate%20Detection.htm)
and [Enable Duplicate Detection](Enable%20Duplicate%20Detection.htm) for
more information.

**NOTE**: There is a distinction between Duplicate Detection, configured
in System Administration, and Bulk Duplicate Detection performed in
Common. Bulk Duplicate Detection is an extension of the Duplicate
Detection capability. Bulk Duplicate Detection is a background event
that detects duplicates for each record in a table. An Administrator or
Designer runs the Bulk Duplicate Detection process in Common. The
results are stored in a DSP®-created table where a client can use them.

This section contains these topics:

  - [Enable Duplicate Detection](Enable%20Duplicate%20Detection.htm)
  - [Search for Duplicates](Search%20for%20Duplicates.htm)
  - [Determine the Duplicate Detection
    Threshold](Determine%20the%20Duplicate%20Detection%20Threshold.htm)
  - [Define an Index for Duplicate
    Detection](Define%20an%20Index%20for%20Duplicate%20Detection.htm)
  - [Control Display and Limit Possible
    Candidates](../Page_Desc/Control%20Display%20and%20Limit%20Possible%20Candidates.htm)
