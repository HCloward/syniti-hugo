# Import Excel Files

When the Excel Import Adapter is used to import Excel files, the
following format must be used:

  - Row 1 – Technical column name

  - Row 2 – Friendly column name put through DSP® translation

  - Row 3 – n: Data

When the import runs, the adapter matches the technical column names
from the worksheet (row 1) with the column names in the Excel Import
Table Name field and only imports data for columns where the column
names match. This configuration allows for columns to be added to the
Excel worksheet for calculations, formulas, etc. without affecting the
import.

To use the Excel Import Adapter to import an Excel file:

1.  Select **Toolkit \> Excel** in *Navigation* pane.

2.  Click **Add.**
    
    [View the field descriptions for the Toolkit: Excel
    page](../Page_Desc/Toolkit_Excel_H.htm)

3.    Enter the table name to import in the **EXCEL IMPORT TABLE NAME**
    field.

4.  Click **Save**; *Vertical* View displays.
    
    [View the field descriptions for the Toolkit: Excel
    page](../Page_Desc/Toolkit_Excel_H.htm)

5.  Click **Excel Use Excel2007** check box to use Excel 2007 or 2010
    (i.e., .xlsx). If disabled, Excel 97-2003 (i.e., .xls) is used.

6.  Enter a value in **Excel Where Clause** field to limit data when
    extracting data.

7.  Enter a table name of the calling component's database into which
    import from the Excel file is processed in **Excel Import Table
    Name** field.

8.  Enter a location (name and path on the application server) of file
    to use for import in **Excel Upload File Name** field.
    
    **NOTE:** It is recommended to use the full physical path to the
    file. If a virtual path is used, the navigation of the virtual path
    begins at the **\[DSP® Installation
    Directory\]\\web\\UserArea\\\[Calling application’s WebAppID\]\\**
    folder.

9.  Click **Excel Delete On Import** check box to enable it, deleting
    all data from the Excel Import Table Name before data from the Excel
    file is imported.

**NOTE:** If an Excel Where Clause is entered, the delete function will
be limited by the where clause.

1.  Enter a name of worksheet in Excel workbook that contains data for
    the import in **Excel Import Sheet Name** field.
2.  Enter a column name on Excel Import Table Name to default a value
    for each record imported in **Excel Import Default Column** field,
    if a default value is used.
3.  Enter a value to write to Excel Import Default Column for each
    record imported in **Excel Import Default Value** field, if a
    default value is used.
4.  Enter a number of records to write to the database from the Excel
    file at one time during the import process in **Excel Import Batch
    Size** field.
5.  Click **Excel Create Table For Import If Not Exists** check box to
    enable it, creating a table named for the Excel Import Table Name,
    which contains all the imported data.
6.  Select a data source from **Excel Import Data Source ID** list box
    if Excel writes to a data source other than current data source. The
    default is to write to the same data source.
7.  Click **Save<span style="font-weight: normal;">.</span>**
8.  Click **Import From Spreadsheet** and browse to Excel file to
    upload; a confirmation message displays.
9.  Click **Ok**.
10. Click **File To Import** to download the file to import.
