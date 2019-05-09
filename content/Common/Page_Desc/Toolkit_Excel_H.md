+++
title = 'Toolkit: Excel H'
solution = 'Platform'
+++

# Toolkit: Excel H

[Toolkit: Excel V](#Toolkit_Excel_V)

<div class="use">

Use this page to:

  - [Import Excel Files](../Use_Cases/Import_Excel_Files)
  - [Export Excel Files](../Use_Cases/Export_Excel_Files)

</div>

To access this page, select <span style="font-weight: bold;">Common \>
Toolkit \> Excel</span> in
<span style="font-style: italic;">Navigation</span>
pane.

|                         |                                                                                                                                           |
| ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| Field                   | Description                                                                                                                               |
| ID                      | Displays the unique identifier of the Excel record.                                                                                       |
| EXCEL EXPORT TABLE NAME | Displays the table name of the calling component’s database into which exports from Excel file are processed. Only required for Export.   |
| EXCEL IMPORT TABLE NAME | Displays the table name of the calling application’s database into which imports from Excel file are processed. Only required for Import. |

## <span id="Toolkit_Excel_V"></span>Toolkit: Excel V

[Toolkit: Excel H](Toolkit_Excel_H)

<div class="use">

Use this page to:

  - [Import Excel Files](../Use_Cases/Import_Excel_Files)
  - [Export Excel Files](../Use_Cases/Export_Excel_Files)

</div>

Field

Description

ID

Displays the unique identifier of the Excel record.

General

 

Excel Use Excel2007

If enabled, Excel 2007 or 2010 (i.e., .xlsx) is used. If disabled, Excel
97-2003 (i.e., .xls) is used.

Excel Where Clause

Displays where clause to limit data extracted.

Import

Excel Import Table Name

Displays table name of the calling component’s database into which
imports from Excel file is processed. Only required for Import.

Excel Upload File Name

Displays location (name and path on the application server) of file to
use for the import.

Excel Delete On Import

Click to delete all data from the Excel Import Table Name before data
from the Excel file is imported.

**NOTE:** If an Excel Where clause is entered, the delete function will
be limited by the where clause.

Excel Import Sheet Name

Displays name of worksheet in the Excel workbook that contains data for
the import.

Excel Import Default Column

Displays column name on the Excel Import Table Name to default a value
for each record imported.

Excel Import Default Value

Displays value to write to the Excel Import Default Column for each
record imported.

Excel Import Batch Size

Displays number of records to write to database from the Excel file at
one time during the import process.

Excel Create Table For Import If Not Exists

Click to create a table named for the Excel Import Table Name containing
all of the imported data. The table also contains an Identity column set
as the primary key of the table.

Excel Import Data Source ID

Displays data source name if the Excel file is being imported from one
data source and written to another. By default, Excel is written to the
same data source.

Import From Spreadsheet

Click to upload an Excel file to import.

File To Import

Click to download a copy of the Excel file being imported.

Export

Excel Export Table Name

Displays table name of  the calling component’s database into which
exports from Excel file is processed. Only required for Exports.

Excel Export File Name

Displays location (name and path on the application server) of the Excel
file to create.

Excel Include Data In Export

Click to include data from the Excel Export Table Name in the created
Excel file. If disabled, the generated Excel file will only contain
column names.

Excel Export Sheet Name

Displays name of the worksheet to create in the generated Excel file.

Excel Export Field List

Displays a comma-separated list of fields in include/exclude from the
Excel Export Table Name when generating the export Excel file.

Excel Export Field List Option

Displays “Include” or “Exclude” to determine whether the Excel Export
Field List includes a list of columns from the Excel Export Table Name
to include in the export or a list of columns to exclude.

Excel Export Order By

Displays an Order By clause to apply to the exported data.

Excel Export Data Source ID

Displays the data source name if Excel file is being exported to one
data source and written from another. By default, Excel is written to
the same data source.

Excel Export Create Directory

Click to create the output directory.

Export To Excel

Displays name of Excel file to export.

Excel File

Click to download an Excel file to export.
