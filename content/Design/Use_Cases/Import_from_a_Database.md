# Import From a Database

The design of a Target can be imported from one or multiple tables in a
database.

Import is also allowed from a System Type or from an Excel file (using a
provided template). Refer to [Import Target Design from a System
Type](Import_from_a_System_Type.htm) and [Import Target Design from an
Excel File](Import_from_an_Excel_File.htm) for more information.

When initially importing from a database, the table(s) and fields are
imported. When importing a table that has already been imported for the
Target, only updates are applied.

After a successful import, the table displays on the
*[Targets](../Page_Desc/Targets_H_Design.htm)* page in Target Design,
with 'tt' appended to the front of the table name. When a user selects
the Target on the *Targets* page, the fields in the Target table display
on the *[Target Fields](../Page_Desc/Target_Fields_H_Target_Design.htm)*
page.

**NOTE:** Ordering of columns is lost when a table is reimported.
Whenever a table is imported, the column order is set using the ordinal
position in the database. Any changes in column order made after import
will be lost when the table is imported again.

To import a database table in Target Design:

1.  Click **Target Import** in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the **Database Import** icon for an OBJECT ID in the parent
    pane.

3.  Click the **Import** icon for a DATA SOURCE ID in the child pane.
    
    **NOTE:** These data sources are registered in Common  and have the
    data source type of SqlServer. Refer to [Register a Data Source in
    Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
    for more information.

4.  Click the **IMPORT** check box to include a table in the import.
    
    **NOTE:** Import can be checked for multiple tables at once. To
    select a contiguous range of records, hold down the **Shift** key
    and select the first and last records in the range. To select a
    non-contiguous range of records, hold down the **Ctrl** key and
    select each record. Click the **Mark for Import**. To exclude
    multiple tables from import, repeat these steps but click the
    **Clear Import Flag** icon.

5.  Click the **Execute Import** icon; a confirmation message displays.

6.  Click **OK**.

During the import, new records are added to the tables, fields, and look
up tables. If the records have been imported into the Target previously,
updates are applied to existing tables, fields and lookup tables.
