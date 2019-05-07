+++
title = 'Create a Template from an Integrate Template'
solution = 'Data Quality'
+++

# Create a Template from an Integrate Template

If a template has already been created in Integrate that can be reused
in dspCompose™, create a dspCompose™ template based on an existing
recording from Integrate (stored in an Integrate template) to post a new
set of legacy data.

Integrate templates can be reused by many dspCompose™ templates.

**NOTE:** A dspCompose™ template can also be based on an Intergrate
template with multiple loops. Refer to [Use dspCompose™ with Integrate
Looped Templates](Use_dspCompose_with_Integrate_Looped_Templates.htm)
for more information.

To create a dspCompose™ template from an Integrate template in
dspCompose:

1.  Click **Team** on the *Navigation* pane.

2.  Click the **Create Template** icon for a team.

3.  Click **Create from Integrate template**.
    
    **NOTE:** If no records exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    [View the field descriptions for the Create Template (Integrate
    Template) page](Create_Template_Integrate_Template.htm)

4.  Enter a name in the **TEMPLATE NAME** field.
    
    **NOTE:** The name must be unique and can contain A-Z, 0-9, and
    underscore. No special characters are allowed in template names. If
    a special character is entered in a template name, dspCompose™ will
    replace it with an underscore when the template is saved.

5.  Select an option from the **CONNECTION ID** list box.
    
    **NOTE:** If a user adds a request based on this template and does
    not select a connection ID, the default connection assigned to the
    Integrate Template is used for the request. Refer to [Establish a
    Connection to a Target
    System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
    for more information.

6.  Select an option in the **INTEGRATE TEMPLATE ID** list box.
    
    **NOTE:** The templates listed in the **INTEGRATE TEMPLATE ID** list
    box are active. Integrate templates that are not active cannot be
    used for dspCompose™ template creation.

7.  Click **Save**.

8.  Click **Create Template**; a confirmation message displays.

9.  Click **Ok**.

Refer to [Configure Templates](Configure_Templates.htm) for more
information.
