# Import From an Excel File

The design of a Target can be imported from an Excel file. A user must
download a formatted template, add data and import the Excel file.

Import is also allowed from a System Type or database tables. Refer to
[Import Target Design from a System Type](Import_from_a_System_Type.htm)
and [Import Target Design from a Database](Import_from_a_Database.htm)
for more information.

After a successful import, the table displays on the
*[Targets](../Page_Desc/Targets_H_Design.htm)* page in Target Design,
with 'tt' appended to the front of the table name. When a user selects
the Target on the *Targets* page, the fields in the Target table (i.e.,
the fields entered in the Excel file) display on the *[Target
Fields](../Page_Desc/Target_Fields_H_Target_Design.htm)* page.

When an Excel file is imported, the fields marked as key in the Excel
file have the KEY FIELD, VERIFY POST LOAD and the ACTIVE check box
enabled by default. Additionally, the REQUIRED field is set to Technical
Required and the CRITICALITY is set to High. Other fields must be made
active to be used in the Target. Refer to [Activate and Deactivate
Target Fields for Mapping](Activate_Fields_for_Map.htm) for more
information.

**NOTE:** The uploaded Excel file is saved to the import file data
source path before it is imported. The default import file data source
is cMap\_Design\_File Path which can be configured and edited by an
Administrator if another data source should be used.

To edit the import path in Target Design:

1.  Select **Configuration** \> **Import Setup** in the *Navigation*
    pane.

2.  Click **Edit**.
    
    *[View the field descriptions for the Target Import Configuration
    page](../Page_Desc/Target_Import_Configuration.htm)*

3.  Select a path in the **IMPORT FILE DATASOURCE** list box.

4.  Click **Save**.

To import an Excel file in Target Design:

1.  Click **Target Import** in the *Navigation* pane.

2.  Click the **Excel Import** icon in the parent pane.

3.  Click the **Download a File** icon in the **EXCEL TEMPLATE** column
    in the child pane to download the template.
    
    **NOTE:** The template contains instructions for data entry. Refer
    to [Complete the Excel File](#Complete) for more information.
    
    **NOTE:** The template is downloaded as read only. Save a copy to
    enter data.

4.  Click the **Upload a File** icon in the **EXCEL FILE PATH** column
    to upload the completed Excel file.

5.  Click the **Import** icon in the child pane.

6.  Click **OK**.

During the import, new records are added to the tables, fields, and look
up tables. If the records have been imported into the Target previously,
updates are applied to existing tables, fields and lookup tables.

## <span id="Complete"></span>Complete the Excel File

After downloading the Excel file, enter data in it to be imported into
the Target.

The template includes instructions on the Instructions tab.

To complete the Excel file in Target Design:

1.  Click the **Targets** tab to access the Targets worksheet.

2.  Complete a row for each Target to be imported.
    
    **NOTE:** All columns are required in the template for the Target
    except Instructions and Comments.

3.  Click **Save**.

4.  Click the **x\_FIELDS** tab to access the worksheet.
    
    **NOTE:** If the Excel file contains multiple Targets, make a copy
    of the fields worksheet for each Target and name it after the
    Target.

5.  Complete a row for each field on the Target.
    
    **NOTE:** Required fields are Name, Field Order, and Usage. If a
    field is marked as a key field in the Excel file, the KEY FIELD
    check box and the VERIFY POST LOAD check box will be checked for the
    field on import. Additionally, the REQUIRED field is set to
    Technical Required and the CRITICALITY is set to High.

6.  Click the **Targets** tab.

7.  Enter the name of the worksheet that contains the Target fields in
    the **Field Worksheet** column.

8.  Click **Save**.

Certain fields have restricted values. In this case, when the user
clicks in the field, a down pointing arrow displays to the right of the
field. Click the arrow to view the list of options. The user must select
a value from a list box to complete the field.

Fields on the **Targets** worksheet should be completed as instructed in
the following table.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Enter</p></td>
</tr>
<tr class="even">
<td><p>Target Name</p></td>
<td><p>Enter the name of the Target, usually a table name.</p></td>
</tr>
<tr class="odd">
<td><p>Field Worksheet</p></td>
<td><p>Enter the name of the worksheet that has been added to the Excel file that stores the field data for the Target.</p></td>
</tr>
<tr class="even">
<td><p>Usage</p></td>
<td><p>Select how the Target table is used.</p>
<p>Values are:</p>
<ul>
<li><strong>Natural</strong> – A field that exists in the Target system.</li>
<li><strong>Utility</strong> – A field that does not exist in the Target system, but is used to register rules and reports to in Transform. Fields of this type should be captured in Target Design but should not be mapped and will not display in Map. A utility field is added to the Target table to be used by Auto Generation.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Target Table Name</p></td>
<td><p>Enter the name of the Target table starting with tt (as in, ttMARA).</p></td>
</tr>
<tr class="even">
<td><p>Priority</p></td>
<td><p>Enter a number for the order that the table should be processed and the order the table displays on the <em><a href="../Page_Desc/Targets_H_Design.htm">Targets</a></em> page in Target Design.</p></td>
</tr>
<tr class="odd">
<td><p>Description</p></td>
<td><p>Enter a brief description of the Target table.</p></td>
</tr>
<tr class="even">
<td><p>Comments</p></td>
<td><p>Enter a comment about the Target.</p>
<p><strong>NOTE:</strong> This field is not required.</p></td>
</tr>
<tr class="odd">
<td><p>Instructions</p></td>
<td><p>Enter instructions about how to use the Target in mapping or other functions.</p>
<p><strong>NOTE:</strong> This field is not required.</p></td>
</tr>
<tr class="even">
<td><p>Status</p></td>
<td><p>Select the status of the Target design.</p>
<p>Values are:</p>
<ul>
<li><strong>In Design</strong> – A Target is in this Design Status when it has been added and while the Target is being configured. All functionality that can be performed on a Target is available.</li>
<li><strong>Design Finished</strong> – When a Target is in this status, the design is locked down, and no changes are allowed. A Target can only move to this status if it is in sync with Map. Auto-generation in Data Services and in SQL is allowed.</li>
<li><strong>Completed</strong> – When a Target is in this status, the design is locked down, and no changes are allowed.</li>
</ul></td>
</tr>
</tbody>
</table>

 

Fields on the x\_FIELDS worksheet should be completed as instructed in
the following table.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Enter</p></td>
</tr>
<tr class="even">
<td><p>Name</p></td>
<td><p>Enter the name of the Target field.</p></td>
</tr>
<tr class="odd">
<td><p>FieldOrder</p></td>
<td><p>Enter the order the field appears on the screen in the Target system.</p></td>
</tr>
<tr class="even">
<td><p>Active</p></td>
<td><p>Select an option to indicate whether this is an active or inactive field. If the field is active, it can be used for mapping. If inactive, the field cannot be used in mapping, and will not be pushed to Map when the Target design is loaded or synced.</p></td>
</tr>
<tr class="odd">
<td><p>Label</p></td>
<td><p>Enter then name of field as it appears on the screen.</p>
<p><strong>NOTE:</strong> This field is not required.</p></td>
</tr>
<tr class="even">
<td><p>Description</p></td>
<td><p>Enter a brief description of the field.</p></td>
</tr>
<tr class="odd">
<td><p>HelpText</p></td>
<td><p>Enter help text from the ERP system.</p></td>
</tr>
<tr class="even">
<td><p>KeyField</p></td>
<td><p>Select an option to indicate if the field is a key field on the table. If a field is marked as a key field in the Excel file, the KEY FIELD check box and the VERIFY POST LOAD check box will be enabled for the field on import. Additionally, the REQUIRED field is set to Technical Required and the CRITICALITY is set to High.</p></td>
</tr>
<tr class="odd">
<td><p>Required</p></td>
<td><p>Select the field’s requirement status.</p>
<p>Values are:</p>
<ul>
<li><strong>Business Required</strong> – Required to meet a business rule or otherwise meet a business need.</li>
<li><strong>Technical Required</strong> – Required by the system</li>
<li><strong>Conditional</strong> – Required depending on certain conditions</li>
<li><strong>Optional</strong> – Not required.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>DataType</p></td>
<td><p>Select the field’s data type, such as NVARCHAR or DECIMAL.</p></td>
</tr>
<tr class="odd">
<td><p>Length</p></td>
<td><p>Enter the field length, or the maximum allowable characters/numbers that the field can store.</p>
<p><strong>NOTE:</strong> If the field is a data type of DECIMAL, the length cannot exceed 38.</p></td>
</tr>
<tr class="even">
<td><p>Decimals</p></td>
<td><p>Enter the number of decimal places allowed in the Target field.</p></td>
</tr>
<tr class="odd">
<td><p>Criticality</p></td>
<td><p>Select an option to indicate the criticality level, used for reporting. Values are High, Medium and Low.</p></td>
</tr>
<tr class="even">
<td><p>Comments</p></td>
<td><p>Enter a comment about the Target.</p>
<p><strong>NOTE:</strong> This field is not required.</p></td>
</tr>
<tr class="odd">
<td><p>Instructions</p></td>
<td><p>Enter instructions about how to use the Target in mapping or other functions.</p>
<p><strong>NOTE</strong>: This field is not required.</p></td>
</tr>
<tr class="even">
<td><p>Usage</p></td>
<td><p>Select how the Target table is used.</p>
<p>Values are:</p>
<ul>
<li><strong>Natural</strong> – A field that exists in the Target system.</li>
<li><strong>Utility</strong> – A field that does not exist in the Target system, but is used to register rules and reports to in Transform. Fields of this type should be captured in Target Design but should not be mapped and will not display in Map. A utility field is added to the Target table to be used by Auto Generation.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>VerifyPostLoad</p></td>
<td><p>Select an option to indicate if data should be verified after it is loaded into the Target system. This option is used with Natural fields only.</p></td>
</tr>
<tr class="even">
<td><p>ApplicationScreen</p></td>
<td><p>Enter the name of the screen in the ERP system that contains the field.</p></td>
</tr>
</tbody>
</table>
