+++
title = 'Automatically Set Settings when Creating an External Request Scenario that Creates an Excel-initiated Request'
solution = 'Data Quality'
+++

# Automatically Set Settings when Creating an External Request Scenario that Creates an Excel-initiated Request

Certain settings, such as the Staging Table Name and the Sheet Name, can
be populated automatically when a user uploads an Excel file for an
external request scenario that creates an Excel-initiated request.

To populate values automatically:

1.  Select **Team** from *Navigation*<span>pane</span>.

2.  Click **Templates** for a team.

3.  Click **Vertical View** for a template.

4.  Click **Configuration** tab.

5.  Click **External Request Scenarios**.
    
    **NOTE**: This icon is disabled if the template has not been
    generated. If the template is active, the *Template (External
    Request Scenario)*<span>page opens in display mode.</span>
    
    **NOTE**: If conditions allow a scenario to be added and no records
    exist, the page displays in add mode. Otherwise, click **Add**.
    
    *[View the field descriptions for the Template (External Request
    Scenario)
    page](../Page_Desc/Template_External_Request_Scenario)*

6.  Enter a value in the **SUBJECT ALIAS** field.
    
    **NOTE**: When dspCompose™ receives an external email and the
    subject line of the email contains this text, dspCompose™ uses this
    external request scenario for the template to create a request.

7.  Enter the name or a brief description of the scenario in the
    **SCENARIO** **DESCRIPTION** field.
    
    **NOTE**: Use this field to identify the scenario, and, if the
    template has multiple scenarios, to distinguish it from others
    attached to the template.

8.  Enter a description in the **REQUEST DESCRIPTION FORMAT** field.
    
    **NOTE**: The text entered in this field displays on the *Request*
    page in the DESCRIPTION field for a request created from this
    external request scenario. <span style="color: #000000;">The field
    defaults
    to</span><span style="font-size: 10.5pt;color: #333333;">Request
    from \#RequesterEmailAddress\# -
    \#Date\#</span><span style="color: #000000;">where the
    RequesterEmailAddress is the address of the user who submitted the
    email to create the request, and the Date is the date that the email
    was received at the External Data Email Account.</span>

9.  Select the connection ID from the **REQUEST CONNECTION ID** list
    box.
    
    **NOTE**: The REQUEST CONNECTION ID is the connection ID to use for
    the created request. Refer to [Establish a Target System
    Connection](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview)
    for more information.

10. Click **Save**; the *Vertical* View displays.

11. Click **Save** again.

12. Click the **Advanced** tab.
    
    **NOTE**: The page is in display mode.

13. Click **Upload Sample Sheet**.

14. Navigate to the Excel file that contains the worksheet.

15. Click **Open**.
    
    **NOTE**: The spreadsheet must be in the following format:
    
      - The first row contains the column names of the table that will
        be created for the lowest priority Data Entry role for the
        request.
      - The second row is ignored, and could contain column descriptions
        to assist users when entering data.
      - The third row is the first data record imported into the staging
        table.
    
    **NOTE**: The only files that can be uploaded are Excel files (with
    an .xls or .xlsx extension).
    
    **NOTE**: When the Excel file has completed uploading,
    
      - The Excel Allowed check box is enabled
      - The name of the first worksheet in the Excel file displays in
        the Sheet Name field
    
    **NOTE**: After the external request scenario that creates an
    Excel-initiated request is configured, a version of this worksheet
    with request-ready data will be mailed to the external data email
    account to create requests for this template. Refer to [Map Columns
    from the Template to Columns from the Excel
    File](../../../Migration/Map/Use_Cases/Map_Columns_Template_to_Sprdsht)
    for more information.
    
      - The Staging Table Name field displays st\[Template
        name\]\_\[Subject
    Alias\]\_ExcelStaging.
    
    **<span style="font-size: 10.5pt;color: #333333;">NOTE</span>**<span style="font-size: 10.5pt;color: #333333;">:</span>
    The Staging Table Name is the name of the table that will be used to
    import Excel attachment spreadsheet data. Once the data has passed
    validations, it will be written to the data entry table for the Data
    role with the lowest priority for the request.
    
    **NOTE**: If another sheet other than the first sheet in the Excel
    file should be used for this scenario, click
    <span style="font-weight: bold;">Edit</span>, select the sheet name
    in the Sheet Name list box and click
    <span style="font-weight: bold;">Save</span>.

16. Click **Build Staging Area**; a confirmation message displays.

17. Click **Ok**.

**NOTE**: dspCompose™ creates a staging table in the cMass\_Data
database. The column names in the table match the column headers in the
Excel file.

**NOTE**: In some cases, the table may need to be rebuilt if the sheet
in the Sheet Name field is uploaded again. Clear the staging table by
clicking Clear Staging Area, then click Build Staging
Area.<span> </span>

Refer to [Map Columns from the Scenario to Columns from the
Spreadsheet](../../../Migration/Map/Use_Cases/Map_Columns_Template_to_Sprdsht)
for more information to continue configuring the external request
scenario.
