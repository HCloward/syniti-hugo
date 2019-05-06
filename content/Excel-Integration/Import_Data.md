# Import Data

Users have the ability to import data into the DSP® from an Excel
spreadsheet created by the user (based on the current DSP® page) or from
a spreadsheet previously downloaded from the DSP®. If the imported
spreadsheet has multiple worksheets, the user will be able to choose
which worksheet data to import. If multiple worksheets are to be
imported, a separate import process must be performed for each
worksheet.

**NOTE:** When importing data via Excel, records that are locked by
another user are listed as failed on the Import Results tab. The user
has the ability to download the failed record(s) and upload the data
later when the record has been unlocked.

**NOTE:** DSP® will calculate functions in an Excel spreadsheet before
importing the results.  It is the result of the calculations that will
be imported.

**NOTE:** If a column is a check box, and the user enters “Y”, “True”,
"true", or “1” in the column in the template, the check box is checked
during the import process. If the user enters “N”, “False”, "false", or
“0”, the check box is unchecked during the import process.

**NOTE:** When importing records via Excel Integration, if a cell in the
Excel file is left blank, the default values from the page are applied.
Default values can be defined either on the page column property, the
page’s defaults view or a database default. To insert a null value in a
column that has a default, the special keyword, {NULL}, can be placed in
the cell in the Excel file.

**NOTE:** When importing records using Excel Integration, the
PreValidation tab on the Excel Integration panel displays a message
indicating which columns contain default values. 

To import data: 

1.  Navigate to the page where the data is to be imported in the DSP®.

2.  Select **Excel Integration** from the page gear menu; the *Excel
    Integration* panel displays.

3.  Click the **Import Data** tab.

4.  Click the **Click here to browse for your Excel file** button.

5.  In the **Choose File to Upload** window, navigate to the desired
    file.

6.  Select the file.

7.  Click **Open**; the *Import Option* tab displays along with a
    confirmation message informing the user the file chosen is valid
    
    **NOTE:** If the file is invalid, an error message displays
    indicating the file is invalid.
    
    **NOTE:** The worksheet name appears in the **Choose Worksheet**
    list box. If there is more than one worksheet in the template, click
    the down arrow to select the worksheet to import.

8.  Modify the value in the **Data Starts on Row** field if necessary.
    
    **NOTE:** The default value for the Data Starts on Row field is the
    first row containing the data to be imported after the column
    heading rows in the Excel template.

9.  Modify the value in the **Column Names on Row** field if necessary.
    
    **NOTE:** The value entered in the **Column Names on Row** field is
    the starting row of the column names in the Excel template. The
    default value for the **Column Names on Row** field is 1.

10. Click the **Import Records** button.
    
    **NOTE:** The import process performs pre-check validations. Results
    are either of type Info, Warning or Error and then separated into
    categories. Hover a cursor over each category to view explanations
    and remediation information of the various pre-validation messages.
    For errors, the reason the user cannot continue is also specified.
    The following pre-check validations are
    performed:
    
    |                                        |                                                                                                                                                                                                                               |
    | -------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
    | Validation                             | Description                                                                                                                                                                                                                   |
    | Missing Optional Columns (Information) | Columns configured for Excel import are missing from the template. These columns are not required. The spreadsheet will be imported.                                                                                          |
    | Extra Columns (information)            | Columns exist in the spreadsheet, but are not configured for import on the DSP page. The spreadsheet will not import data from the columns listed.                                                                            |
    | Drill Criteria (Warning)               | The template contains drill criteria for the current page. These values will override any found in the template. The spreadsheet will be imported but drill criteria on the page will override any values in the template.    |
    | Identity Field (Warning)               | A column included in the template is an identity field for the underlying table. Values in this column in the spreadsheet will be overridden by auto-incrementing identity value on import. The spreadsheet will be imported. |
    | Shared Criteria (Warning)              | The template contains shared fields on the current page that belong to the primary key. These values will be auto-inserted on import and will override any values found in the template.                                      |
    | Missing Required Columns (Error)       | These are required columns that are missing from the template. The import stops. These columns and values must be added to the template to continue.                                                                          |
    | Duplicate Columns (Error)              | Columns appear more than once in the template. The import stops. The user must edit the template and remove the duplicate column (s) before continuing.                                                                       |
    

    **NOTE:** While the Excel import is processing, a process bar and a
    Stop Import button appears. Click the **Stop Import** button to
    cancel the process.

Once the process is complete, the Import Results tab displays. After
data has been imported, a list of inserted, updated, failed and skipped
records displays and is grouped with error summaries based on reasons
for failure:

  - **Inserted** — These records were successfully imported into DSP®.
  - **Updated** — These records were successfully updated in the DSP.
  - **Skipped** — These records were skipped. Blank rows in the
    spreadsheet are skipped. Click the row listed to view the reason it
    was not inserted.
  - **Failed** — These records were not imported. Expand the list to
    display the reason(s) and row number of the failed record. Click the
    failed row to display the details of the failure. Reasons for
    failure include but are not limited to:
      - **Locked records** — An attempt was made to import a record that
        is locked. Refer to [Lock Records](Lock_Records.htm) for more
        information.
    
      - **Incorrect data type** — The data type of the imported data
        does not match the data type of the corresponding data in the
        DSP.
    
      - **Data length exceeded** — The length of the data for the
        imported value was exceeded.
    
      - **Foreign key constraint violation** — An attempt was made to
        insert a record with a value whose column references a foreign
        key constraint. The value was not found in the foreign key
        table.
    
      - **Duplicate primary key** — An attempt was made to insert a
        record whose primary key already exists in the table.
        
        **NOTE:** A record can fail for a duplicate primary key when the
        record is initially imported, if there are no records on the
        page and if the import file contains duplicate records. If the
        record already exists on a page, it is updated on import, and
        does not fail for duplicate primary keys.
    
      - **Data Volume Limitations** — The data volume limitation on
        imported spreadsheets cannot exceed the **Excel Import Record
        Limit**. The default for this parameter is 100k rows. Refer to
        the
         [Parameters](../Sys_Admin/Page_Desc/Parameters_All_TabsSysAdmin.htm)
        page for more information.

If records fail to import, a button appears in the upper right corner of
the Import Results window.

To download an Excel spreadsheet of records that fail to insert:

1.  Click the **Download Excel Sheet of Records that Fail to Insert**
    button.
2.  Follow the browser specific instructions that are presented to open
    or save the file.

**NOTE:** If errors occur, modify the worksheet accordingly and perform
the import again.

**NOTE:** If the data is encrypted in the DSP®, then the data is
encrypted on import.

**NOTE:** After performing an Excel Import, a Bulk Execution icon
displays in the top right area of the Results tab. When this icon is
clicked, the Bulk Execution panel opens and is filtered on the records
which were successfully inserted. The user can then proceed to perform
the Bulk Execution process, which allows the user to validate the
records that were inserted or updated. Refer to the [Bulk
Execution](../Sys_Admin/Use_Cases/Configure_Bulk_Execution_Overview.htm)
topic for more information.

**NOTE:** If Audit is turned on for the table when the Excel import is
performed, an audit is conducted to show which fields have changed. To
view the results of the audit, select **Admin \> Data Sources \> Audit
Report** in the *Navigation* pane. The Data Source Audit Report
displays. In the table, the field names are listed along with the data
type and data length in the source table and audit table. If the Audit
Table column is populated, that means the corresponding field was
changed.
