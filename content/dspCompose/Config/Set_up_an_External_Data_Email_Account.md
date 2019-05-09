+++
title = 'Set Up an External Data Email Account'
solution = 'Data Quality'
+++

# Set Up an External Data Email Account

The External Data Email Account is used for both [External Request
Scenarios](../Use_Cases/Use_External_Request_Scenarios) and for
[External Data Processing with an External Data
role](../Use_Cases/Use_External_Data_Roles_in_Request_Processing).

On the *External Data Email Accounts* page, a record is added with a
previously created external email account. dspCompose™ will poll that
account for emails from users who are assigned the External Data role.
This account will send a spreadsheet to an External Data role designated
as an external contact for the template. The external contact will then
email the spreadsheet containing data for a request to this external
email account.

The external data email account is also used for external request
scenarios. Once the scenario has been configured, a valid user will send
an email to this address to add a request.

To set up an external data email account:

1.  Select **Configuration \> External Data Email Accounts** on the
    *Navigation* pane.

2.  Click **Add**.
    
    *[View the field descriptions for the External Data Email Accounts
    page.](../Page_Desc/External_Data_Email_Accounts)*

3.  Enter the host name for the external email account in **HOST**
    field.

4.  Enter the email address in **USERNAME** field.
    
    **NOTE:** This address must be dedicated to receiving external
    emails for the purposes of external data processing and external
    request scenarios.
    
    **NOTE:** The email address entered in **USERNAME** must be polled
    by only one server and the dspCompose™ instance. For example, if
    there are multiple dspCompose™ instances (development, QA,
    production), each should reference a different email address in the
    **USERNAME** field.
    
    **NOTE:** This email address should also be configured as the
    **EMAIL FROM** on the *Workflow Language Message* page. Refer to
    [Update the EMAIL FROM
    Column](Update_the_EMAIL_FROM_Column)<span> </span>for more
    information.

5.  Enter the email password in **PASSWORD** field.

6.  Click the **USE SSL** check box to enable it to use this standard
    security technology.
    
    **NOTE:**SSL is used to encrypt sensitive information sent across
    the Internet so that only the intended recipient can receive it.

7.  Enter the port number on the email server for email in the **PORT**
    field.

8.  Enter the path where attachments from emails, in the form of Excel
    spreadsheets containing data for a request, should be stored in the
    **ATTACHMENT FOLDER PATH** field.

9.  Click **Test Connection** to verify that dspCompose™ can access the
    external email account to poll it.

10. Click **Save**.
