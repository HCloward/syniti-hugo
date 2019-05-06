# Download an Excel Spreadsheet

The downloaded Excel spreadsheet contains those columns in the
*Horizontal* View that are not hidden or disabled via the “Excel” or
“All Views” View Types. Refer to [Exclude Columns from Excel
Integration](../Sys_Admin/Use_Cases/Exclude%20Columns%20Excel%20Integration.htm)
for more information.

In the Excel template, the cell’s comment as well as column highlighting
indicate if the column is required. Users can also include the Data Type
in the header.

  - varchar, nvarchar, char, nchar will show the data type and length,
    for example nvarchar (50), when the field has maximum length it will
    show (-1) as the length, for example nvarchar (-1), ntext will show
    always (-1)
  - decimal, numeric, money and smallmoney will show the data type and
    the number of whole digits and decimals, for example decimal (10,4)
  - bit, int, smallint, bigint, double, float, real, datetime,
    datetime2, time and uniqueidentifier will show only the data type

Users can add new records or can update existing records using the
template. If users are updating records, those records are locked until
the template is uploaded. Refer to [Lock Records](Lock_Records.htm) and
[Unlock Records](Unlock_Records.htm) for more information.

**NOTE:** Columns with the following defined column properties do not
apply to Excel and are not downloaded via Excel Integration:

  - Button
  - File
  - HTML Area
  - Image
  - Label
  - Tab
  - Toolbar

**NOTE:** When a column has data disabled via a Data Control View (DCV)
and a spreadsheet is downloaded using that existing data, the data is
disabled in the spreadsheet as well. When a column has data hidden via a
DCV, the data is hidden in the spreadsheet as well. Columns controlled
via a DCV should be unaffected during Excel insert.

**NOTE:** Columns disabled or hidden by a Page Control View (PCV) or
User Control View (UCV) are not included in a downloaded spreadsheet.

To download an Excel spreadsheet:

1.  Navigate to the page where the Excel spreadsheet is to be
    downloaded.

2.  Select **Excel Integration** from the page gear menu; the *Excel
    Integration* panel displays.

3.  Update the **Workbook Filename** field if desired.
    
    **NOTE:** The filename format is limited to the standards of the
    user’s operating system. Unallowed characters are converted to
    underscores.
    
    **NOTE:** If no filename is entered, the page name is used as the
    default.

4.  Update the **Worksheet Name** field if desired.
    
    **NOTE:** The worksheet name format is limited to 31 characters and
    is filtered for characters not allowed in an Excel worksheet name.
    Unallowed characters are converted to underscores. If the name
    entered is longer than 31 characters, it is truncated to 31
    characters. If no worksheet name is entered, the page name is used
    as the default.

5.  Check the **Include Existing Data** check box if records on the page
    must be edited in the spreadsheet.
    
    **NOTE:** If this check box is checked, the records on the page are
    locked until the spreadsheet is uploaded if the reserved columns
    LockedOn, LockedBy, and boaLockType have been added to the
    underlying table(s) for the page. Refer to [Lock
    Records](Lock_Records.htm) for more information.
    
    **NOTE:** If records on the page are already locked, they are not
    downloaded. To unlock records, refer to [Unlock
    Records](Unlock_Records.htm) for more information.

6.  On the **Download Template** tab, click the **Download** button.

7.  Follow the browser specific instructions that are presented to open
    the file.
