# Create an External Request Scenario

<span style="font-weight: bold;">NOTE:</span> If the template associated
with the external request scenario is active, no external request
scenarios can be added, edited or deleted. To add or change external
request scenarios, the template must be inactive and in Developer mode.
Refer to [Modify an Active Template in Developer
Mode](Modify_an_Active_Template_in_Developer_Mode.htm) for more
information.

To create an external request scenario:

1.  Select **Team** from the *Navigation* pane.

2.  Click the **Templates** icon for a team.

3.  Click the **Vertical View** icon for a template.

4.  Click the **Configuration** tab.

5.  Click the **External Request Scenarios** icon.

6.  Click **Add**.
    
    *[View the field descriptions for the Template (External Request
    Scenario)
    page.](../Page_Desc/Template_External_Request_Scenario.htm)*

7.  Enter a value in the **SUBJECT ALIAS** field.
    
    **NOTE:** When dspCompose™ receives an external email, if the
    subject line of the email contains this value, dspCompose™ will use
    this external request scenario for the template to create a request.
    This value must be unique, and does not have to be related to the
    template name.
    
    **NOTE:** The subject line of the email submitted for an external
    request scenario must:
    
      - Contain this alias
    
      - Match the alias exactly
    
      - Contain no other characters
    
    **NOTE:** The alias cannot exist as part of another alias for any
    other external request scenario. For example, if “Change Material”
    is the alias for one scenario, another scenario, whether attached to
    the same template or not, could not be called “Change Material 2.”

8.  Enter the name or a brief description of the scenario in the
    **SCENARIO DESCRIPTION** field.
    
    **NOTE:** Use this field to identify the scenario, and, if the
    template has multiple scenarios, to distinguish it from others
    attached to the template.

9.  Enter a description in the **REQUEST DESCRIPTION FORMAT** field.
    
    **NOTE:** The REQUEST DESCRIPTION FORMAT field is used on the
    *Request* page in the **DESCRIPTION** field for a request created
    from this external request scenario. The field accepts \#Date\# and
    \#RequesterEmailAddress\# as a dynamic substitution value for
    replacement at run time. The field defaults to Request from
    \#RequesterEmailAddress\# - \#Date\# where the RequesterEmailAddress
    is the address of the user who submitted the email to create the
    request, and the Date is the date that the email was received at the
    External Data Email Account.

10. Click the **Connections** icon to select a connection to the target
    system for each process template.
    
    **NOTE:** The connection is used to post the data during the posting
    role. dspCompose™ can post to multiple instances of the target
    system.
    
    **NOTE:** If a user adds a request based on this template and does
    not select a connection ID, the default connection assigned to the
    Integrate Template is used for the request. Refer to [Establish a
    Connection to a Target
    System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
    for more information.
    
    **NOTE:** The Process Templates for which a connection can be set
    are based on:
    
      - The Integrate template type. Refer to [Create a Basic
        Template](../../../Platform/Integrate/Use_Cases/Create_a_Basic_Template.htm)
        in Integrate for more information.
      - The "Allowed Connections" configured at the Integrate Process
        Template level. Refer to [Set Available Connections at the
        Process Template
        Level](../../../Platform/Integrate/Use_Cases/Set_Connections_at_the_Process_Template_Level.htm)
        in integrate for more information.

11. Click **Edit**.

12. Select the connection from the **CONNECTION ID** list box.

13. Click **Save**.

Continue with [Add Email Addresses for a
Scenario](Add_Email_Addresses_for_a_Scenario.htm) and [Set External Role
Contacts for an External Request
Scenario](Set_External_Role_Contacts.htm).
