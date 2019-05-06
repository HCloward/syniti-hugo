# Add Email Addresses for a Scenario

When a request is received at the external data email account,
dspCompose™ checks the email’s subject line for a valid alias for an
external request scenario. If an alias is found, dspCompose™ will then
validate that the sender’s email has been added to the external request
scenario.

<span style="font-weight: bold;">NOTE</span>: If the sender is an
external user who is not registered in the platform, that email must be
added to the platform. Refer to [Add Email Addresses for External
Users](../Config/Add_Email_Addresses_for_External_Users.htm) for more
information.

<span style="font-weight: bold;">NOTE</span>: If the template associated
with the external request scenario is active, no email address can be
added, edited or deleted. To update or add an email address, the
template must be in Developer mode. Refer to [Modify an Active Template
in Developer Mode](Modify_an_Active_Template_in_Developer_Mode.htm) for
more information.

Refer to [Create an External Request
Scenario](Create_an_External_Request_Scenario.htm) and [Create the
external request scenario that creates an Excel-initiated
request](Create_an_External_Request_Scenario_for_an_Excel_Initiated_Requestel.htm)
for more information.

To add an email address that can send a request for the scenario:

1.  Select **Team** from *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Vertical View** for a template.

4.  Click **Configuration** tab.

5.  Click **External Request Scenarios**.

6.  Click **Email Addresses** for the scenario.
    
    <span style="font-weight: bold;">NOTE:</span> If no records exist,
    the page displays in add mode. Otherwise, click
    <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Template (External Request
    Scenario Email Address)
    page](../Page_Desc/Template_External_Request_Scenario_Email_Address.htm)

7.  Enter an email address in the **EMAILADDRESS** field. The email
    address must contain a period (.) and an "at" sign (@) in order to
    be valid.

8.  Enter the sender’s name in the **NAME** field.
    
    <span style="font-weight: bold;">NOTE</span>: This name displays in
    the workflow email.

9.  Select the language of the email from the **LANGUAGEID** list box.
    
    <span style="font-weight: bold;">NOTE</span>: The LANGUAGE ID sets
    the language used for the<span> </span> workflow message sent for
    the ExternalData event. Language-specific messages are added on the
    *Workflow Message* page and the *Workflow Language Message* page.
    Refer to [Configure Workflow
    Messages](../Config/Configure_Workflow_Messages.htm) for more
    information.

10. Include additional information about the email address in
    **COMMENT** field, if necessary.

11. Click **Save**.

Refer to [Set External Role Contacts for an External Request
Scenario](Set_External_Role_Contacts.htm) for more information about
configuring external request scenarios.
