+++
title = 'Create an External Request Scenario for an Excel-initiated Request'
solution = 'Data Quality'
+++

# Create an External Request Scenario for an Excel-initiated Request

An external request scenario allows dspCompose™ to create a request when
an external contact sends an email to an email address designated to
receive dspCompose™ workflows. Refer to [Use External Request
Scenarios](Use_External_Request_Scenarios) for more information.

**NOTE**: If the template associated with the external request scenario
is active, no external request scenarios can be added, edited or deleted
for that template. Updates are restricted. Refer to [Edit an Active
template with an external request scenario that uses an Excel-initiated
request](Edit_Active_Template_External_Rqst_Scnario) for more
information.

In an external request scenario that creates an Excel-initiated request,
an external contact sends an email with an Excel file (with one or
multiple worksheets) attached to an external data email account
configured for dspCompose™.

**NOTE**: The Excel file must be in the following format.

The first row contains the column names of the table that will be
created for the lowest priority Data Entry role for the request.

The second row is ignored, and could contain column descriptions to
assist users when entering data.

The third row is the first data record imported into the staging table.

Before creating this type of scenario, some configuration is required.
Refer to [Configure Settings for External Request Scenarios that Create
Excel-initiated
Requests](Configure_Settings_External_Rqst_Scenarios_that_Create_Excel)
for more information.

To understand the external request scenario process, refer to [External
Request Scenarios that Create Excel-initiated
Requests](External_Request_Scenarios_that_Create_Excel_Initiated_Requests)
for more information.

Some settings for an external request scenario that creates an
Excel-initialed request can be automatically populated when a
spreadsheet is uploaded. Refer to [Automatically Set Settings when
Creating an External Request Scenario that Creates an Excel-initiated
Request](Automatically_Set__Settings_When_Createng_an_External) for
more information.

To create an external request scenario for an Excel-initiated request:

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
    
    **NOTE**: When dspCompose™ receives an external email, if the
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

9.  Click the **EXCEL ALLOWED** check box to enable it.
    
    **NOTE**: This check box cannot be disabled if:
    
      - The template has been activated, even if the template is in
        Developer mode
    
      - The template has not yet been activated, but an Excel file has
        been added to the external request scenario.
    
      - The check box can be disabled if the template has not yet been
        activated, an Excel file has been added to the external request
        scenario, but the user clears data from all fields on the
        <span style="font-style: italic;">Template (External Request
        Scenario)</span> page's
        <span style="font-style: italic;">Vertical</span> View on the
        Advanced tab.

10. Select the SAP connection ID from the
    <span style="font-weight: bold;">TARGET ERP SYSTEM</span> list box.
    
    **NOTE**: The TARGET ERP SYSTEM is the connection ID to use for the
    created request. SAP connections are added in Common. Refer to
    [Establish an SAP
    Connection](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview)
    for more information.

11. Click **Save**; the *Vertical* View displays.

12. Click the **Advanced** tab.
    
    **NOTE**: The Request Excel Initiate check box is enabled.

13. Click the **Finish First Role** check box to enable it if the Data
    Entry role with the lowest priority is to be finished once the data
    from the spreadsheet has passed validations and been written to the
    Data Entry table.
    
    **NOTE**: In this case, the request moves to the next role in the
    workflow, either the next Data role or a Review role, and a user
    assigned to this next role receives a workflow message that the role
    is ready. The FINISHED BY column on the *Request (Roles)* page
    displays the email of the user who submitted the Excel file. The
    FINISHED ON column displays the date the email was received. If the
    Finish First Role check box is disabled, the Data Entry role with
    the lowest priority receives a workflow message that the role is
    ready after the data from the Excel file has passed validations and
    been written to the Data Entry table. The Data Entry role will not
    be finished until the user assigned to this role clicks the Finish
    button.

14. Enter a name in the **Sheet Name** field.
    
    **NOTE**: The Sheet Name is the name of the worksheet in the sample
    Excel file that will be uploaded in step 19 below. A version of this
    worksheet with request-ready data will be mailed to the external
    data email account to create requests for this template.
    
    **NOTE**: This name is case sensitive.

15. Press the **Enter** key.

16. Select an option from the **Staging Data Source ID** list box.
    
    **NOTE:** The dspCompose\_Data data source is the recommended
    selection and is where the staging table will be created and stored.

17. Enter a name in the **Staging Table Name** field.
    
    **NOTE:**  The Staging Table Name is the name of the table that will
    be used to import Excel attachment spreadsheet data. Once the data
    has passed validations, it will be written to the data entry table
    for the Data role with the lowest priority for the request.

18. Click **Save**.

19. Click **Upload Sample Sheet**.

20. Navigate to the Excel file that contains the worksheet entered in
    step 14 and select it.

21. Click **Open**.
    
    **NOTE**: The spreadsheet must be in the following format.
    
      - The first row contains the column names of the table that will
        be created for the lowest priority Data Entry role for the
        request.
      - The second row is ignored, and could contain column descriptions
        to assist users when entering data.
      - The third row is the first data record imported into the staging
        table.
    
    **NOTE**: The only files that can be uploaded are Excel files (with
    an .xls or .xlsx extension).

22. Click **Build Staging Area**; a confirmation message displays.

23. Click **Ok**.

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
