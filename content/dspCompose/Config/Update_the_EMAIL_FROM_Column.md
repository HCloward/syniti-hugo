+++
title = 'Update the EMAIL FROM Column'
solution = 'Data Quality'
+++

# Update the EMAIL FROM Column

Prior to setting up external data role processing, update the address in
the **EMAIL FROM** column for the **ExternalData** and
**EmailValidation** events on the *Workflow Language Message* page. The
address should be the same as the external email account saved on the
*External Data Email Accounts* page in the **USERNAME** column.

**NOTE:** The address in the **EMAIL FROM** column for the
**EmailValidation** event and the **ExternalData** event are identical
by default. These addresses must be configured on site and should
contain the same email address.

Refer to [Set up External Email
Accounts](Set_up_an_External_Data_Email_Account.htm) for more
information.

This setup configures dspCompose™ to send a workflow email and any
emails about email validation failures to an external contact from the
external data email account address. The external contact then replies
to the correct email address when submitting data for a request.

To update the **EMAIL FROM** column on the *WorkFlow Language Message*
page:

1.  Select **Configuration \> Workflow Message** on the *Navigation*
    pane.

2.  Click **Messages** for the **English LANGUAGE ID** field.

3.  Click **Edit** for the **ExternalData EVENT** field.
    
    *[View the field descriptions for the Workflow Language Message
    page's Vertical
    View.](../Page_Desc/Workflow_Language_Message_H.htm)*

4.  Update the **EMAIL FROM** field to match the **USERNAME** saved on
    the *External Data Email Accounts* page.

5.  Click **Save**.
    
    **NOTE**: Update the **EMAIL FROM** field for all languages that use
    Workflow Language Messages.
