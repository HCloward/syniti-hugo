+++
title = 'Submit an Email for an External Request Scenario that Creates an Excel-initiated Request'
solution = 'Data Quality'
+++

# Submit an Email for an External Request Scenario that Creates an Excel-initiated Request

Once an external request scenario that creates an Excel-initiated
request has been configured, a user sends an email with an Excel file
attached to add a request for the template using the data in the Excel
file; any erroneous data in the file should be corrected before sending
the email.

**NOTE**: The email must pass all validations. Refer to [Set up Email
Validations](Set_up_Email_Validations.htm) for more information.

The Excel file provides data for the first Data Entry role in the
workflow.

To submit an email:

1.  Send the email from the address configured for the scenario.
    
    **NOTE**: Refer to [Add Email Addresses for a
    Scenario](Add_Email_Addresses_for_a_Scenario.htm) for more
    information.

2.  Enter the email address configured as the external date email
    account in the **To** field.
    
    **NOTE**: Refer to [Set up External Data Email
    Accounts](../Config/Set_up_an_External_Data_Email_Account.htm) for
    more information.

3.  Enter the alias for the scenario in the **Subject** field.
    
    **NOTE**: The subject line of the email submitted for an external
    request scenario must contain this alias. Refer to [Create an
    External Request <span> </span>Scenario that Creates Excel-initiated
    Requests](Create_an_External_Request_Scenario_for_an_Excel_Initiated_Requestel.htm)
    for more information.

4.  Leave the email body blank.

5.  Attach the spreadsheet that contains the data.

6.  Send the email.

If there are errors processing the scenario, the sender will receive a
message from the external data email account. Refer to [Set up Email
Validations](Set_up_Email_Validations.htm) for more information. Correct
the errors and resubmit the email.

Once the email has been submitted successfully, the Data Entry role with
the lowest priority receives a workflow message that the role is ready
(if the user(s) for that role have the
<span>SEND</span><span>WORKFLOW</span> check box enabled on the *Users*
page).

**NOTE**: If the Finish First Role check box is enabled for the external
request scenario, the Data Entry role with the lowest priority is
finished once the data from the Excel file has passed validations and
been written to the Data Entry table. In this case, the request moves to
the next role in the workflow, either the next Data role or a Review
role, and a user assigned to this next role receives a workflow message
that the role is ready. <span> </span>Refer to [Create an External
Request Scenario for an Excel-initiated
Request](Create_an_External_Request_Scenario_for_an_Excel_Initiated_Requestel.htm)
for more information.

The newly created request displays on the *Requests* page. In the
<span>DESCRIPTION</span> field, the description included with the
scenario displays and the first data entry role has data from the Excel
file submitted for the scenario.
