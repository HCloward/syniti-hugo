+++
title = 'Submit an Email for an External Request Scenario'
solution = 'Data Quality'
+++

# Submit an Email for an External Request Scenario

Once a scenario has been configured, a user sends an email to add a
request for the template.

To submit an email:

1.  Send the email from the address configured for the scenario.
    
    **NOTE**: Refer to [Add Email Addresses for a
    Scenario](Add_Email_Addresses_for_a_Scenario.htm) for more
    information.

2.  Enter the email address configured as the external date email
    account in the **To** field.
    
    **NOTE**: Refer to [Set up External Email
    Accounts](../Config/Set_up_an_External_Data_Email_Account.htm) for
    more information.

3.  Enter the alias for the scenario in the **Subject** field.
    
    **NOTE**: T<span>he subject line of the email submitted for an
    external request scenario</span> must
    
      - Contain this alias
    
      - Match the alias exactly
    
      - Contain no other characters
        
        Refer to [Create the
        Scenario](Create_an_External_Request_Scenario.htm) for more
        information.

4.  Leave the email body blank.

5.  Send the email.

If there are errors processing the scenario, the sender will receive a
message from the external data email account. Refer to [Set up Email
Validations Including Custom Validation
Rules](Set_up_Email_Validations.htm) for more information. Correct the
errors and resubmit the email.

Once the email has been submitted successfully, the first role in the
request receives an email and notification that the request is ready to
be processed, if the user(s) for that role have **SENDWORKFLOW** check
box enabled on the *Users* page.

If the scenario’s first role is an External Data role, dspCompose™ sends
the spreadsheet with request data to the External Data role. Otherwise,
the initial data role is notified that work is ready to be completed.

The newly created request displays on the *Requests* page. In the
**DESCRIPTION** field, the description included with the scenario
displays.
