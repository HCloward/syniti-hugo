# Set External Role Contacts

If the template that uses an external request scenario also uses an
External Data role, the users assigned to this role must also be set as
external role contact for the template.

<span style="font-weight: bold;">NOTE:</span> If the sender is an
external user who is not registered in the platform, that email must be
added to the platform. Refer to [Add Email Addresses for External
Users](../Config/Add_Email_Addresses_for_External_Users.htm) for more
information.

Refer to [Use External Data Roles in Request
Processing](Use_External_Data_Roles_in_Request_Processing.htm) for more
information about assigning an External Data role to a template.

To set the external role contacts for the template:

1.  Select **Team** from *Navigation* pane.

2.  Click **Templates** for a team.

3.  Click **Vertical View** for a template.

4.  Click **Configuration** tab.

5.  Click **External Request Scenarios**.

6.  Click **External Roles** for a scenario.
    
    **NOTE**: This icon only displays when a template has an External
    Data role assigned.

7.  Click <span style="font-weight: bold;">Edit</span>.
    
    *[View the field descriptions for the Template (External Request
    Scenario External Role)
    page.](../Page_Desc/Template_External_Request_Sceanario_External_Role.htm)*
    
    **NOTE**: **EXTERNAL ROLE ID** is the ID for the External Data role.

8.  Enter the address of the user associated with the External Data role
    for this template in **RECIPIENT EMAIL ADDRESS** field. The email
    address must contain a period (.) and an "at" sign (@) in order to
    be valid.
    
    **NOTE:** This user will receive the initial email when the request
    is ready for processing if the External Data role is the initial
    role in the external request scenario.

9.  Enter a name in **NAME** field.

10. Select an option from the **LANGUAGE ID** list box.

11. Click **Save**.

Refer to [Set the Current User as the External Role Contact for an
External Request
Scenario](Set_the_Current_User_as_the_External_Role_Contact.htm) for
more information.
