+++
title = 'Packages H'
solution = 'Platform'
+++

# Packages H

[Packages V](#Packages_V)

<div class="use">

Use this page to [Create Packages](Create_Packages.htm).

</div>

To access this page, click <span style="font-weight: bold;">Assemble \>
Packages</span> in the
<span style="font-style: italic;">Navigation</span> pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PACKAGE NAME</p></td>
<td><p>Displays the package name.</p>
<p>The naming convention for packages is #Database#%#Source#%, for example dswBRAZIL.stKNA1_QALegacyData_Customer.imp for an import or dswBRAZIL.stKNA1_QALegacyData_Customer.exp for an export.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE DATA SOURCE ID</p></td>
<td><p>Displays the Assemble data source to be used for source data.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE TYPE</p></td>
<td><p>Displays the source type. Options include:</p>
<ul>
<li>SQL Server</li>
<li>Table</li>
<li>ODBC</li>
<li>Fixed File</li>
<li>Delimited File</li>
<li>Excel File</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>TARGET DATA SOURCE ID</p></td>
<td><p>Displays the Assemble data source to be used for target data.</p></td>
</tr>
<tr class="even">
<td><p>TARGET TYPE</p></td>
<td><p>Displays the Target Type. Options include:</p>
<ul>
<li>SQL Server</li>
<li>Table</li>
<li>ODBC</li>
<li>Fixed File</li>
<li>Delimited File</li>
<li>Excel File</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>SC</p></td>
<td><p>Click to open the <span style="font-weight: bold;">Source Columns</span> page of the selected package.</p></td>
</tr>
<tr class="even">
<td><p>TC</p></td>
<td><p>Click to open the <span style="font-weight: bold;">Target Columns</span> page of the selected package.</p></td>
</tr>
<tr class="odd">
<td><p>Map</p></td>
<td><p>Click to open the <span style="font-weight: bold;">Package (Mapping)</span> page which displays the selected package's column mapping.</p></td>
</tr>
<tr class="even">
<td><p>SUM</p></td>
<td><p>Click to open the package summary page of the selected package.</p></td>
</tr>
<tr class="odd">
<td><p>Run</p></td>
<td><p>Click to open the <span style="font-weight: bold;">Packages (Run)</span> page, from which the selected package can be executed.</p></td>
</tr>
<tr class="even">
<td><p>Log</p></td>
<td><p>Click to open the <span style="font-weight: bold;">Log</span> page, where the selected package's execution history, number of records, Time duration, etc. can be seen.</p></td>
</tr>
</tbody>
</table>

## <span id="Packages_V"></span>Packages V

[Packages H](#Packages_H)

<div class="use">

Use this page to [Create Packages](Create_Packages.htm).

</div>

### <span id="Source_Types:"></span>Source Types:

  - [Table (General tab)](#Table_-_General_Tab)
  - [Table (Advanced Properties tab)](#Table_-_Advanced_Properties_Tab)
  - [SQL (General tab)](#SQL_-_General_Tab)
  - [SQL (Advanced Properties tab)](#SQL_-_Advanced_Properties_Tab)
  - [File Delimited (General tab)](#File_Delimited_-_General_Tab)
  - [File Delimited( Advanced Properties
    tab)](#File_Delimited_-_Advanced_Properties_Tab)
  - [Excel (General tab)](#Excel_-_General_Tab)
  - [Excel (Advanced Properties tab)](#Excel_-_Advanced_Properties_Tab)
  - [File Start-End (General tab)](#File_Start-End_-_General_Tab)
  - [File Start-End (Advanced Properties
    tab)](#File_Start-End_-_Advanced_Properties_Tab)
  - [File Width (General tab)](#File_Width_-_General_Tab)
  - [File Width (Advanced Properties
    tab)](#File_Width_-_Advanced_Properties_Tab)

### <span id="Table_-_General_Tab"></span>Table - General tab

Field

Description

Source Information

Source Table Name

Displays the name of the table to extract data from. This name must be
unique.

Target Information

Target Table Name

Displays the name of the database table used as the target for this
package. This name must be unique.

**NOTE:** If spaces or special characters are required in the table
name, the name must be enclosed in square brackets (\[ and \]).

Target Table Exists

If enabled, the Target Table already exists in the database.

Create Target Table

Click to create the table in the target database in accordance with the
target column specifications, and the column
map.

### <span id="Table_-_Advanced_Properties_Tab"></span>Table - Advanced Properties tab

Field

Description

Time Out

Displays the SQL command timeout used for database commands. This
applies only to Assemble execution. It controls the time out for a
database command when a CranPort package runs. Database commands include
creating a table, truncating an existing table, selecting data and
writing data. If the Time Out is not specified for a package, the
Parameter Time Out value automatically defaults.

Batch Size

Displays the number of records moved to the target database in each
transaction. The default batch size is 10,000.

This option is useful for dense datasets which can lead to performance
degradation on the system running the package.

Execution Option

Displays the option for executing the package. The values are:

  - Stop on Error – Execution will cease execution if an error is
    encountered.
  - Continue On Error - Assemble will log the error, and then try to
    continue transferring data.

Queue ID

Displays which service queue will be used to process this package.

Source Options

Source Segment Field

Displays the field used to divide the package up into smaller execution
segments or blank if no field is to be used. For example, if Source
Segment Field is "Country", a package will be run for each country in
the source query. In this way, the package can be multi-threaded to
increase performance.

**NOTE**: For tables, it will break up the execution of the CranPort
package based on whichever field in the table the user chooses.  This is
an execution optimization option.

Segment Threshold

Displays the minimum percentage of the total records a segment must have
to be run in its own thread. Segments that are below the threshold are
run together.

**NOTE**: This field is used in conjunction with Source Segment Field
and indicates the percentage of which a source segment can be its own
partition. The default value is 5. If any of the source segment field
values breakup is less than 5 percent of the total record set it will be
included in a single segment reserved for other partitions that do not
exceed this threshold.

Segment Preview

When clicked, it opens a page with the first 15 records from the source.

Target Options

Target Delete Records

If enabled, records will be deleted from the target table before package
execution. This may be used in conjunction with Target Delete Where
Clause.

Target Delete Where Clause

If Target Delete Where Clause is not blank and Target Delete Records is
checked, the where clause will be used when deleting records from the
target table. "WHERE" should not be entered.

### <span id="SQL_-_General_Tab"></span>SQL - General tab

Field

Description

Source Information

Source SQL

Displays the SQL statement used to query the Source database.

Target Information

Target Table Name

Displays the name of the database table used as the target for this
package. This name must be unique.

**NOTE:** If spaces or special characters are required in the table
name, the name must be enclosed in square brackets (\[ and \]).

Target Table Exists

If enabled, the Target Table already exists in the database.

Create Target Table

Click to create the table in the target database in accordance with the
target column specifications, and the column
map.

### <span id="SQL_-_Advanced_Properties_Tab"></span>SQL - Advanced Properties tab

Field

Description

Time Out

Displays the SQL command timeout used for database commands. This
applies only to Assemble execution. It controls the time out for a
database command when a CranPort package runs. Database commands include
creating a table, truncating an existing table, selecting data and
writing data. If the Time Out is not specified for a package, the
Parameter Time Out value automatically defaults.

Batch Size

Displays the number of records moved to the target database in each
transaction. The default batch size is 10,000. This option is useful for
dense datasets which can lead to performance degradation on the system
running the package.

Execution Option

Displays the option for executing the package. The values are:

  - Stop on Error – Execution will cease execution if an error is
    encountered.
  - Continue On Error – Assemble will log the error, and then try to
    continue transferring data.

Queue ID

Displays which service queue will be used to process this package.

Source Options

Source Order By

When using SQL typed source, it will order the result set by this value.
Order by should not be explicitly defined within the SQL itself. ORDER
BY should also not be used in the value provided.

Source Segment Field

If Source Segment Field is not blank, it will be used to divide the
package up into smaller execution segments. For example, if Source
Segment Field is "Country", a package will be run for each country in
the source query. In this way, the package can be multi-threaded to
increase performance.

Segment Threshold

If Source Segment Field is used, the Segment Threshold specifies the
minimum percentage of the total records a segment must have to be run in
its own thread. Segments that are below the threshold are run together.

Segment Preview

Displays a dataset of each segment value along with the record count.
This is based on the Source Segment Field chosen for this package.

Target Options

Target Delete Records

If enabled, records will be deleted from the target table before package
execution. This may be used in conjunction with Target Delete Where
Clause.

Target Delete Where Clause

If Target Delete Where Clause is not blank and Target Delete Records is
checked, the where clause will be used when deleting records from the
target table. "WHERE" should not be
entered.

### <span id="File_Delimited_-_General_Tab"></span>File Delimited - General tab

Field

Description

Source Information

Source Path

Displays thefile path specified by the Source Data Source.

Source Subdirectory

Displays the subdirectory within the data source where the source file
is located.

Source File Name

Displays the name of the file to be used for source data. This name will
be appended to the data source file path and the Source Subdirectory if
it exists, so it should not include drive specifications (i.e. c:\\).

Source File Upload

Click to upload a package source file to the web server form their local
machine.

Source Contains Header

If enabled, the first row in the source file will be interpreted as a
column header and not imported as data.

Source Start Row

If populated, allows for skipping unnecessary data at the beginning of
the Source file. The default is 1.

Source Delimiter

Displays the delimiter used to parse the Source file.

Target Information

Target Table Name

Displays the name of the database table used as the target for this
package. This name must be unique.

**NOTE:** If spaces or special characters are required in the table
name, the name must be enclosed in square brackets (\[ and \]).

Target Table Exists

If enabled, the Target Table already exists in the database.

Create Target Table

Click to create the table in the target database in accordance with the
target column specifications, and the column
map.

### <span id="File_Delimited_-_Advanced_Properties_Tab"></span>File Delimited - Advanced Properties tab

Field

Description

Time Out

Displays the SQL command timeout used for database commands. This
applies only to Assemble execution. It controls the time out for a
database command when a CranPort package runs. Database commands include
creating a table, truncating an existing table, selecting data and
writing data. If the Time Out is not specified for a package, the
Parameter Time Out value automatically defaults.

Batch Size

Displays the number of records moved to the target database in each
transaction. The default batch size is 10,000.

This option is useful for dense datasets which can lead to performance
degradation on the system running the package.

Execution Option

Displays the option for executing the package. The values are:

  - Stop on Error – Execution will cease execution if an error is
    encountered.
  - Continue On Error - Assemble will log the error, and then try to
    continue transferring data.

Queue ID

Displays which service queue will be used to process this package.

Source Options

Source Code Page

Displays the encoding of the source file. Allows text files with
different character sets to be imported.

Segment Treat Consecutive Delimiters As One

Determines the way consecutive delimiters are handled. For instance, if
this value is checked, a line reading "A,,B" will be split into 2
columns. . If unchecked (default behavior) the line will be split into
3.

Source Text Qualifier

If specified, it is stripped from the Source data file. For example *A
"B" C* will be exported as *A B C*, if " is specified as the Source Text
Qualifier.

Source File Delete

If checked, the source file will be deleted after the package completes
a successful execution. If the package errors they will see it as failed
in the log for that package. Their Service light will also turn Yellow
(If it’s not already) to indicate there was a failed job.

Target Options

Target Delete Records

If enabled, records will be deleted from the target table before package
execution. This may be used in conjunction with Target Delete Where
Clause.

Target Delete Where Clause

If Target Delete Where Clause is not blank and Target Delete Records is
checked, the where clause will be used when deleting records from the
target table. "WHERE" should not be entered.

### <span id="Excel_-_General_Tab"></span>Excel - General tab

Field

Description

Source Information

Source Path

Displays thefile path specified by the Source Data Source.

Source Subdirectory

Displays the subdirectory of the data source where the source file is
located.

Source File Name

Displays the name of the file to be used for source data. This name will
be appended to the data source file path, so it should not include drive
specifications (i.e. c:\\).

Source File Upload

Click to upload a package source file to the web server form their local
machine.

Source Contains Header

If checked, the first row in the source file will be interpreted as a
column header and not imported as data.

Source Start Row

If populated, allows for skipping unnecessary data at the beginning of
the Source file. The default is 1.

Source Delimiter

Displays the delimiter used to parse the Source file.

Target Information

Target Table Name

Displays the name of the database table used as the target for this
package. This name must be unique.

**NOTE:** If spaces or special characters are required in the table
name, the name must be enclosed in square brackets (\[ and \]).

Target Table Exists

If enabled, the Target Table already exists in the database.

Create Target Table

Click to create the table in the target database in accordance with the
target column specifications, and the column
map.

### <span id="Excel_-_Advanced_Properties_Tab"></span>Excel - Advanced Properties tab

Field

Description

Time Out

Displays the SQL command timeout used for database commands. This
applies only to Assemble execution. It controls the time out for a
database command when a CranPort package runs. Database commands include
creating a table, truncating an existing table, selecting data and
writing data. If the Time Out is not specified for a package, the
Parameter Time Out value automatically defaults.

Batch Size

Displays the number of records moved to the target database in each
transaction. The default batch size is 10,000. This option is useful for
dense datasets which can lead to performance degradation on the system
running the package.

Execution Option

Displays options for executing package?

Values are:

  - Stop on Error - Assemble will cease execution if an error is
    encountered.
  - Continue On Error - Assemble will log the error, and then try to
    continue transferring data.

Queue ID

Displays which service queue will be used to process this package.

Source Options

Source Excel Worksheet

Displays the name of the Excel worksheet containing the data to be
imported.

Source Excel Skip Empty Rows

If enabled, empty rows will be skipped, meaning empty records will not
be written to the target.

Source File Delete

If enabled, the source file will be deleted after the package completes
a successful execution.

Target Options

Target Delete Records

If enabled, records will be deleted from the target table before package
execution. This may be used in conjunction with Target Delete Where
Clause.

Target Delete Where Clause

If Target Delete Where Clause is not blank and Target Delete Records is
checked, the where clause will be used when deleting records from the
target table. "WHERE" should not be
entered.

### <span id="File_Start-End_-_General_Tab"></span>File Start-End - General tab

Field

Description

Source Information

Source Path

Displays the file path specified by the Source Data Source.

Source Subdirectory

Displays the subdirectory of the data source where the source file is
located.

Source File Name

Displays the name of the file to be used for source data. This name will
be appended to the data source file path, so it should not include drive
specifications (i.e. c:\\).

Source File Upload

Click to upload a package source file to the web server form their local
machine.

Source Contains Header

If enabled, the first row in the source file will be interpreted as a
column header and not imported as data.

Source Start Row

If populated, allows for skipping unnecessary data at the beginning of
the Source file. The default is 1.

Source Delimiter

Displays the delimiter used to parse the Source file.

Target Information

Target Table Name

Displays the name of the database table used as the target for this
package. This name must be unique.

**NOTE:** If spaces or special characters are required in the table
name, the name must be enclosed in square brackets (\[ and \]).

Target Table Exists

If enabled, the Target Table already exists in the database.

Create Target Table

Click to create the table in the target database in accordance with the
target column specifications, and the column
map.

### <span id="File_Start-End_-_Advanced_Properties_Tab"></span>File Start-End - Advanced Properties tab

Field

Description

Time Out

Displays the SQL command timeout used for database commands. This
applies only to Assemble execution. It controls the time out for a
database command when a CranPort package runs. Database commands include
creating a table, truncating an existing table, selecting data and
writing data. If the Time Out is not specified for a package, the
Parameter Time Out value automatically defaults.

Batch Size

Displays the number of records moved to the target database in each
transaction. The default batch size is 10,000.

This option is useful for dense datasets which can lead to performance
degradation on the system running the package.

Execution Option

Displays the option for executing the package. The values are:

  - Stop on Error – Execution will cease execution if an error is
    encountered.
  - Continue On Error - Assemble will log the error, and then try to
    continue transferring data.

Queue ID

Displays which service queue will be used to process this package.

Source Options

Source Code Page

Displays the encoding of the source file. Allows text files with
different character sets to be imported.

Source File Delete

If enabled, the source file will be deleted after the package completes
a successful execution.

Target Options

Target Delete Records

If enabled, records will be deleted from the target table before package
execution. This may be used in conjunction with Target Delete Where
Clause.

Target Delete Where Clause

If Target Delete Where Clause is not blank and Target Delete Records is
checked, the where clause will be used when deleting records from the
target table. "WHERE" should not be entered.

### <span id="File_Width_-_General_Tab"></span>File Width - General tab

Field

Description

Source Information

Source Path

Displays the file path specified by the Source Data Source.

Source Subdirectory

Displays the subdirectory of the data source where the source file is
located.

Source File Name

Displays the name of the file to be used for source data. This name will
be appended to the data source file path, so it should not include drive
specifications (i.e. c:\\).

Source File Upload

Click to upload a package source file to the web server form their local
machine.

Source Contains Header

If enabled, the first row in the source file will be interpreted as a
column header and not imported as data.

Source Start Row

If populated, allows for skipping unnecessary data at the beginning of
the Source file. The default is 1.

Source Delimiter

Displays the delimiter used to parse the Source file.

Target Information

Target Table Name

Displays the name of the database table used as the target for this
package. This name must be unique.

**NOTE:** If spaces or special characters are required in the table
name, the name must be enclosed in square brackets (\[ and \]).

Target Table Exists

If enabled, the Target Table already exists in the database.

Create Target Table

Click to create the table in the target database in accordance with the
target column specifications, and the column
map.

### <span id="File_Width_-_Advanced_Properties_Tab"></span>File Width - Advanced Properties tab

Field

Description

Time Out

Displays the SQL command timeout used for database commands. This
applies only to Assemble execution. It controls the time out for a
database command when a CranPort package runs. Database commands include
creating a table, truncating an existing table, selecting data and
writing data. If the Time Out is not specified for a package, the
Parameter Time Out value automatically defaults.

Batch Size

Displays the number of records moved to the target database in each
transaction. The default batch size is 10,000. This option is useful for
dense datasets which can lead to performance degradation on the system
running the package.

Execution Option

Displays the option for executing the package. The values are:

  - Stop on Error – Execution will cease execution if an error is
    encountered.
  - Continue On Error - Assemble will log the error, and then try to
    continue transferring data.

Queue ID

Displays which service queue will be used to process this package.

Source Options

Source Code Page

Displays the encoding of the source file. Allows text files with
different character sets to be imported.

Source File Delete

If enabled, the source file will be deleted after the package completes
a successful execution.

Target Options

Target Delete Records

If enabled, records will be deleted from the target table before package
execution. This may be used in conjunction with Target Delete Where
Clause.

Target Delete Where Clause

If Target Delete Where Clause is not blank and Target Delete Records is
checked, the where clause will be used when deleting records from the
target table. "WHERE" should not be entered.
