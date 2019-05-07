+++
title = 'External Request Scenarios that Create Excel-Initiated Requests'
solution = 'Data Quality'
+++

# External Request Scenarios that Create Excel-Initiated Requests

While an external request scenario can be configured to simply create a
request when an email is received, templates may also be configured to
accept an Excel file attached to the email. The Excel file provides data
for the first Data Entry role in the workflow. In this case, not only
will the request be created, but the worksheet data from the Excel file
will be inserted into the table used by the first Data Entry role (after
certain conditions are met).

This type of request is called an Excel-initiated request.

<span style="font-weight: bold;">NOTE</span>: For templates that use
scenarios that create Excel-initiated requests, emails can have an Excel
file attached that contains more than one worksheet so that more than
one template external request scenario can be processed with one email.
The subject line for external emails for Excel-initiated requests must
include the text entered in the SUBJECT ALIAS field for at least one of
the Sheet Names that match a worksheet in the email. dspCompose creates
a request for every worksheet name that matches a sheet name for an
External Request Scenario.

An external request scenario that creates an Excel-initiated request
requires the same configuration as an external request scenario. Refer
to [Configure settings for an External Request
Scenario](Configure_Settings_External_Rqst_Scenarios_that_Create_Excel.htm)
for more information.

This type of scenario also requires additional configuration. Refer to
[Configure settings for an External Request Scenario that creates
Excel-initiated
Requests](Configure_Settings_External_Rqst_Scenarios_that_Create_Excel.htm)
for more information.

To use an external request scenario that creates an Excel-initiated
request:

1.  An external contact sends a request by email to an external data
    email account set up in dspCompose™. Refer to [Set up an External
    Data Email
    Account](../Config/Set_up_an_External_Data_Email_Account.htm) for
    more information.

2.  The email poller runs, locates the email, and checks the email for
    an alias in the subject line that corresponds to a subject alias
    saved for an external request scenario that creates Excel-initiate
    requests. Refer to [Create an External Request Scenario for an
    Excel-initiated
    Request](Create_an_External_Request_Scenario_for_an_Excel_Initiated_Requestel.htm)
    for more information about aliases.
    
    **NOTE:** If the email’s subject line does not contain the alias,
    processing stops and the external contact receives a message that
    the email’s subject line is not valid. The external contact must
    correct the error and resubmit the email.

3.  If an email’s subject line contains an alias that has been
    configured for an external request scenario, dspCompose™ compares
    the sender’s email address to the list of email addresses on the
    *Template (External Request Scenario Email Address)* page for the
    scenario. Refer to [Add Email Addresses for a
    Scenario](Add_Email_Addresses_for_a_Scenario.htm) for more
    information.
    
    **NOTE:** If the email’s subject line does not contain a valid
    alias, processing stops and the external contact receives a message
    that the email’s alias is not valid. The external contact must
    correct the error and resubmit the email.

4.  If the sender’s email address has been added to the external request
    scenario, the name of the worksheet in the Excel file is compared to
    the Sheet Name (entered on the *Template (External Request
    Scenario)* page’s *Vertical* View on the Advanced tab) for the
    external request scenario.
    
    **NOTE:** If the sender’s email address has not been added to the
    external request scenario, processing stops and the external contact
    receives a message that the email address is not valid. The external
    contact must resubmit the email from a valid email address.

5.  If there is a match between the worksheet name in the Excel file and
    the name entered in Sheet Name, dspCompose™ copies the request data
    to a staging table for the external request scenario’s template.
    
    **NOTE:** If the Excel file contains worksheets for which no
    matching Sheet Name is found, those worksheets are ignored. Other
    worksheets with valid names are processed.

6.  dspCompose™ maps the data in the columns in the worksheet to the
    template columns according to mappings created on the *Template
    (External Request Scenario Columns)* page. Refer to [Map Columns
    from the Template to Columns from the
    Spreadsheet](../../../Migration/Map/Use_Cases/Map_Columns_Template_to_Sprdsht.htm)
     for more information.

7.  If custom rules have been registered as template-level events,
    dspCompose™ runs those rules on the data. Refer to [Create Custom
    Rules for Excel-initiated
    Requests](Create_Custom_Rules_for_Excel_Initiated_Requests.htm)  for
    more information.

8.  Once the mapping and rules are complete, the request data is moved
    from the staging table to the data entry table for the lowest
    priority Data Entry role for that template.

**NOTE:** When an External Contact for an external request scenario that
creates an Excel-initiated request submits an Excel file as an
attachment to an email, if any of the worksheets fail an email
validation, none of the worksheets in the Excel file will be processed.
The external contact will receive a message from the first validation
that fails.<span> </span> The external contact must correct and resubmit
the Excel file. Refer to [Set Up Email
Validations](Set_up_Email_Validations.htm) for more information.

**NOTE:** The email poller is scheduled to run every 10 minutes. This
value is configurable in System Administration.

**NOTE:** Once the request is created, the workflow for processing the
request is the same as any other request. Refer to [Process
Requests](Process_Requests.htm) for more information.

This section includes:

  - [Configure Settings for External Request Scenarios that Create
    Excel-initiated
    Requests](Configure_Settings_External_Rqst_Scenarios_that_Create_Excel.htm)
  - [Configure an External Request Scenario for an Excel-initiated
    Request](Configure_External_Rqst_Scenario_for_Excel_Initiated_Request.htm)
  - [Submit an Email for an External Request Scenario that Creates an
    Excel-initiated request](Submit_Email_External_Reqst_Scenario.htm)
