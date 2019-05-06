# Excel Integration Panel

<div class="use">

Use this page to:

  - [Download an Excel
    Spreadsheet](../../Excel_Int/Download_an_Excel_Spreadsheet.htm)
  - [Import Data](../../Excel_Int/Import_Data.htm)
  - [Unlock Records](../../Excel_Int/Unlock_Records.htm)

</div>

This panel contains the following tabs:

  - [Download Template](#Download_Template_tab)
  - [Import Data](#Import_Data_tab)

To access this page:

1.  Navigate to the page where the data is to be imported in the DSP®.  
    OR  
    Navigate to the page where the Excel template is to be downloaded.
2.  Select **Excel Integration** from the page gear menu.

### <span id="Download_Template_tab"></span>Download Template tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Unlock Records</p></td>
<td><p>Click to unlock the records on the current page that have been locked by another user. Refer to <a href="../../Excel_Int/Lock_Records.htm">Lock Records</a> for more information.</p>
<p><strong>NOTE:</strong> This icon only displays if there are locked records on the page.</p></td>
</tr>
<tr class="odd">
<td><p>Workbook Filename</p></td>
<td><p>Displays the filename of the Excel workbook that is downloaded.</p>
<p><strong>NOTE:</strong> The filename format is limited to the standards of the user’s operating system. Unallowed characters are converted to underscores.</p>
<p><strong>NOTE:</strong> If no file name is entered, the page name is used as the default.</p></td>
</tr>
<tr class="even">
<td><p>Worksheet Name</p></td>
<td><p>Displays the name of the worksheet (in the Excel file indicated in the Workbook Filename field) that is downloaded.</p>
<p><strong>NOTE:</strong> The worksheet name format is limited to 31 characters and is filtered for characters not allowed in an Excel worksheet name. Unallowed characters are converted to underscores. If the name entered is longer than 31 characters, it is truncated to 31 characters.</p>
<p><strong>NOTE:</strong> If no worksheet name is entered, the page name is used as the default.</p></td>
</tr>
<tr class="odd">
<td><p>Include Existing Data</p></td>
<td><p>If checked, unlocked records are included in the downloaded spreadsheet, which can then be edited.</p>
<p>If unchecked, an empty Excel spreadsheet (based on the current DSP® page) is downloaded.</p></td>
</tr>
<tr class="even">
<td><p>Download</p></td>
<td><p>Click to download the Excel file indicated in the <strong>Workbook Filename</strong> field.</p>
<p><strong>NOTE:</strong> This creates a template file for the user to enter data.</p></td>
</tr>
</tbody>
</table>

### <span id="Import_Data_tab"></span>Import Data tab

### Choose an Excel File

|                                           |                                                             |
| ----------------------------------------- | ----------------------------------------------------------- |
| Field                                     | Description                                                 |
| Click here to browse for your Excel file. | Click to choose the file to upload for importing into DSP®. |

### Import Options

On this tab, a message indicating whether or not the file chosen is a
valid Excel file displays.

If the file is valid, the filename and its size display.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Choose Worksheet</p></td>
<td><p>Displays the worksheet name containing the data that will be imported.</p>
<p><strong>NOTE:</strong> If there is more than one worksheet in the template, click the down arrow to select the worksheet to import.</p></td>
</tr>
<tr class="odd">
<td><p>Data Starts on Row</p></td>
<td><p>Displays the starting row of the data in the Excel template that will be imported.</p>
<p><strong>NOTE:</strong> The default value for the Data Starts on Row field is the first row containing data after the column heading rows in the Excel template.</p></td>
</tr>
<tr class="even">
<td><p>Column Names on Row</p></td>
<td><p>Displays the starting row of the column names in the Excel template.</p>
<p><strong>NOTE:</strong> The default value for the <strong>Column Names on Row</strong> field is 1.</p></td>
</tr>
<tr class="odd">
<td><p>Insert Records</p></td>
<td><p>Click to import records in the worksheet indicated in the Choose Worksheet field.</p></td>
</tr>
</tbody>
</table>

### Import Results

After data has been imported, a list of inserted, updated, failed and
skipped records displays and is grouped with error summaries based on
reasons for failure. See [Import Data](../../Excel_Int/Import_Data.htm)
for more
information.

|                       |                                                                                                         |
| --------------------- | ------------------------------------------------------------------------------------------------------- |
| Field                 | Description                                                                                             |
| Expand All            | Click to expand the lists (Inserted, Updated, Failed, and Skipped) to display the records.              |
| Collapse All          | Click to collapse the lists (Inserted, Updated, Failed, and Skipped).                                   |
| Import Another File   | Click to import another file into DSP®.                                                                 |
| Bulk Execution button | Click to open the Bulk Execution panel to validate the records added and updated via Excel Integration. |
