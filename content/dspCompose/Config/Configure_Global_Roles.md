+++
title = 'Configure Global Roles'
solution = 'Data Quality'
+++

# Configure Global Roles

dspCompose™ is delivered with three global roles, Data, Review and Post,
which can be modified. They can be copied to a template either manually
or automatically if the **Auto Copy** option is selected on the
*Vertical* View of the *Roles* page.

Users assigned to the <span style="font-weight: bold;">Data role</span>
enter request data by manually entering or editing data, performing a
mass change, or importing data. Refer to [Enter Data for a
Request](../Use_Cases/Enter_Data_for_a_Request) for more
information.

Users assigned to the <span style="font-weight: bold;">Review
role</span> review the data entered by the Data role, and approve or
reject the data. Refer to [Review Request
Data](../Use_Cases/Review_Request_Data) for more information.

Users assigned to the <span style="font-weight: bold;">Post role</span>
post the approved data to SAP. Refer to [Post Request Data to a Target
ERP System](../Use_Cases/Post_Request_Data_to_a_Target_ERP_System)
for more information.

Users assigned to the External Data role receive a spreadsheet generated
by dspCompse™, enter request data, and email the spreadsheet to
dspCompose™. This data, once it passes validations, becomes the basis
for a request. The External Data role type is delivered with
dspCompose™, but must be added on the *Roles* page to be used. Refer
to [Add External Data Role to Global
Roles](../Use_Cases/Add_External_Data_Role_to_Global_Roles) for more
information.

If the parameters **Add Roles On Template Creation** (set on the
*Parameters* page) and **Auto Copy** (set on the *Roles* page’s
*Vertical* View**)** for the global role are enabled, these roles are
automatically registered to a new template. These options are enabled by
default.

A Template Administrator can also create a global role that can be
copied to a template.

If a global role is copied to a template and a user modifies that role
at the template level, these changes will not be overridden by global
role settings.

If a user deletes a global role at the template level that has the
**Auto Copy** option selected at the global role level, the global role
will not be added back to the template.

**NOTE**: The External Data role can also be added to the *Roles* page
before being added to a template. Refer to [Use External Data Roles in
Request
Processing](../Use_Cases/Use_External_Data_Roles_in_Request_Processing)
for more information.

To configure a global role:

1.  Select **Configuration \> Roles** on the *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Edit**.
    
    *[View the field descriptions for the Roles
    page.](../Page_Desc/Roles_H)*

3.  Enter the sort order in **PRIORITY
    <span style="font-weight: normal;">field</span>**, which determines
    this role’s place in the order of roles displayed on the *Roles*
    page and the order the roles on a request are processed. The role
    with the lowest priority is processed first.
    
    **NOTE**: Priority also controls how dependencies are created. Roles
    should never be available for processing until the roles on which
    they depend have been processed. Role dependencies should never be
    set up such that, for example, a role with priority of 50 would
    become available for processing before a role with priority of 30 or
    40 had been processed. Refer to
    <span style="color: #000000;font-family: Arial, sans-serif;font-size: 11pt;">[Add
    Role Dependencies](../Use_Cases/Add_Role_Dependencies)</span>
    for more information.

4.  Enter a brief description about the global role in **DESCRIPTION**
    field.

5.  Click **Save<span style="font-weight: normal;">.</span>**

6.  Click<span style="font-weight: bold;">Vertical View</span>.

7.  Click<span style="font-weight: bold;">Edit</span>.
    
    *[View the field descriptions for the Roles page's Vertical
    View.](../Page_Desc/Roles_H)*

8.  Select the **Force Validation Before Finish** check box to enable it
    to require validation to be complete before the selected role can be
    finished.
    
    **NOTE**: Refer to [Add Validations to
    Roles](../Use_Cases/Add_Validations_to_Roles) and [Validate a
    Role](../Use_Cases/Validate_a_Role) for more information.

9.  Select an option from the **Prevent Finish Severity** list box.
    
    **NOTE**: When an option is selected from the Prevent Finish
    Severity list box, dspCompose™ prevents a role from finishing if,
    during processing, a validation fails that matches the selected or
    higher severity level. Values are:
    
      - **Error** – Marks the role status as
        <span style="font-style: italic;">invalid</span> until the error
        is corrected and the Validation Rule passes.
    
      - **Message** – Marks the role status as
        <span style="font-style: italic;">valid</span> but a message
        displays.
    
      - **Warning** –
        <span style="font-size: 10.0pt;font-family: Arial, sans-serif;">Displays
        a message but the user can proceed with the task even if the
        validation</span><span> </span><span style="font-size: 10.0pt;font-family: Arial, sans-serif;">fails</span>.

10. Click <span style="font-weight: bold;">Save</span>.
