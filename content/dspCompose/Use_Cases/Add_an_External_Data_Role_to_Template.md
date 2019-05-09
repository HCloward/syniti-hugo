+++
title = 'Add an External Data Role Type to a Template'
solution = 'Data Quality'
+++

# Add an External Data Role Type to a Template

To use <span style="font-family: Arial, sans-serif;">an external role in
request processing</span>, a Template Administrator assigns a role with
a role type of External Data to a template.

To assign a role at the template level:

1.  Select **Team** on the *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.
    
    **NOTE**: A user may set up the template with an External Data role
    as the initial role and the only Data role in the template. A
    template can also have multiple Data roles, with External Data role
    and Data role.

4.  Click **Add**.
    
    *[View the field descriptions for the Template (Role)
    page.](../Page_Desc/Template_Role_H)*

5.  Enter the sort order in **PRIORITY** field.
    
    **NOTE**: If this template should be used for External Request
    Scenarios, and the data from the External Data role should start the
    process, the External Data role should be the initial role. Give
    this role the lowest priority. Refer to [Use External Request
    Scenarios](Use_External_Request_Scenarios) for more information.

6.  Select **External Data** from the **ROLE ID** list box.

7.  Click **Save**; the *Vertical* View displays.

8.  Click **Save**.
    
    **NOTE**: Set up dependencies for the External Data role for any
    roles that should follow it in the workflow. For example, the Review
    role and the Post role should be dependent on the External Data
    role.

9.  Click **Dependencies** for the role.

10. Close the <span style="font-style: italic;">Template
    (Role)</span><span>Vertical view.</span>

11. Click the **DEPENDS** check box for the
    <span style="font-family: Arial, sans-serif;">Review Role and the
    Post Role</span> to enable it. This certifies that the External Data
    role must be finished before the Data Reviewer role can be started.
    
    **NOTE**: The External Data role can be configured like any other,
    with event rules, column controls, validations, and other settings.
    Refer to [Configure Templates](Configure_Templates) for more
    information.
