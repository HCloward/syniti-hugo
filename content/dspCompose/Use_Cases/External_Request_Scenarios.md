+++
title = 'External Request Scenarios'
solution = 'Data Quality'
+++

# External Request Scenarios

A Template Administrator configures one or multiple external request
scenarios for a template.

Once an external request scenario is configured, a user can submit an
email to an external data email account set up in dspCompose™ to begin
request processing by creating a request. This user must:

  - Use an alias set up for the external request scenario in the subject
    line of the email
  - Have an email address that has been saved for the external request
    scenario

Set up of alias and email address are part of external request scenario
configuration.

<span style="font-weight: bold;">NOTE</span>: Request data can also be
sent to dspCompose™ by an External Data role. Refer to [Use External
Data Roles in Request
Processing](Use_External_Data_Roles_in_Request_Processing) for more
information. An external request scenario can use an External Date role
as the initial role, but is not required to do so.

For example, a Template Administrator could create a scenario called
Create Customer. Its alias is also Create Customer. The email addresses
for members of the Sales team have been added to the scenario. A member
of the sales team can then send an email to the external data email
account with the subject line “Create Customer.” dspCompose™
automatically creates a request for that template.

Before setting up external request scenarios, other settings must be
configured. Refer to [Configure Settings for External Data Processing
and External Request
Scenarios](../Config/Configure_Settings_for_External_Data_Processing)
for more information.

To use an external request scenario to process a request:

1.  An external user sends a request by email to an external data email
    account set up in dspCompose™. Refer to [Set up an External Data
    Email Account](../Config/Set_up_an_External_Data_Email_Account)
    for more information.
2.  The dspCompose™ Email Poller runs, processes the found email, and
    checks the email for an alias in the subject line that exactly
    matches the alias saved for the scenario. Refer to  [Create an
    External Request Scenario](Create_an_External_Request_Scenario)
    for more information about aliases.
3.  If an email’s subject line contains an alias that has been
    configured for an external request scenario, dspCompose™ compares
    the sender’s email address to the list of email addresses on the
    *Template (External Request Scenario Email Address)* page for the
    scenario. Refer to [Add Email Addresses for a
    Scenario](Add_Email_Addresses_for_a_Scenario) for more
    information.
4.  If the email has been added to the external request scenario,
    dspCompose™ creates a new request for the template using the
    settings from the scenario.

<span style="font-weight: bold;">NOTE</span>: If an external request
scenario is set up without an external role as the initial role, the
user assigned to the lowest priority Data role will receive the initial
workflow when the user sends an email to enter the request.

<span style="font-weight: bold;">NOTE</span>: The email poller is
schedule to run every 10 minutes.

<span style="font-weight: bold;">NOTE</span>: Once the request is
created, the workflow for processing the request is the same as any
other request. Refer to [Process Requests](Process_Requests) for
more information.

This section includes:

  - [Configure an External Request
    Scenario](Configure_an_External_Request_Scenario)
  - [Set External Role Contacts for an External Request
    Scenario](Set_External_Role_Contacts)
  - [Set the Current User as the External Role
    Contact](Set_the_Current_User_as_the_External_Role_Contact)
  - [Submit an Email for an External Request
    Scenario](Submit_an_Email_for_an_External_Request_Scenario)
  - [Add Email Addresses for a
    Scenario](Add_Email_Addresses_for_a_Scenario)
