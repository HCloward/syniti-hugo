+++
title = 'Set Validation Threshold'
solution = 'Data Quality'
+++

# Set Validation Threshold

At the template role level, a Template Administrator can set a
validation threshold to monitor when a user, including an external role
user, is unable to pass a role. When a user clicks the **Validate**
button on the *Request (Roles)* page for a role, and at least one record
in a validation fails, dspCompose™ logs the failure and keeps a count of
failed records. When this count exceeds the validation threshold,
dspCompose™ sends the validation contacts an email. If the role finishes
successfully, dspCompose™ resets the validation count.

<span style="font-weight: bold;">NOTE:</span> For the Validate button to
display on the <span style="font-style: italic;">Request (Roles)</span>
page, validations must exist for the template. Refer to [Add Validations
to Roles](Add_Validations_to_Roles.htm)  for more information.

**NOTE:** To set a validation threshold and contacts at the template
level, the template must not be active or must be in Developer Mode.
Refer to [Modify an Active Template in Developer
Mode](Modify_an_Active_Template_in_Developer_Mode.htm) for more
information.

<span style="font-weight: bold;">NOTE:</span> This setting is not
available for the Post role as the Validate button does not display for
this role.

To set a validation threshold and add contacts:

1.  Click **Team** on *Navigation* pane.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Vertical View** for a role.

5.  Click the **Approve and Finish Settings** tab.

6.  Click **Edit**.
    
    *[View the field descriptions for the Template (Role) page’s
    Vertical View.](../Page_Desc/Template_Role_H.htm)*

7.  Enter a number in the **Validation Threshold** field.
    
    **NOTE**: If the **Validation Threshold** field is left blank or
    contains 0, dspCompose™ will never send an email to the validation
    contacts.

8.  Click **Save**.

9.  Click **Contacts**.
    
    **NOTE:** If no records exist, the page displays in add mode.
    Otherwise, click Add.
    
    [View the field descriptions for the Template (Role Validation
    Threshold Contact)
    page](../Page_Desc/Template_Role_Validation_Threshold_Contact.htm)

10. Select a user from the **USER ID** list box.
    
    **NOTE:** This user will receive an email when the validation
    threshold for this template role has been exceeded.

11. Click **Save**.
