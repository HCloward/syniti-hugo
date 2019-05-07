+++
title = 'Add and Configure Template Roles'
solution = 'Data Quality'
+++

# Add and Configure Template Roles

A role is a single step in the mass change process. A role type is
assigned to a role to define how the role data within the request is
manipulated. There are three global role types:

  - **Data -** Gathers or makes changes to data
  - **Review -** Evaluates and reviews data and is responsible for
    approving or rejecting work. Data can be viewed but not modified.
  - **Post -** Posts data to the target system, and the final role in
    the process after the Data and Review roles have been completed.

A Template Administrator can also add an External Data role to a
template. External Data roles have role type of **ExternalData.** Refer
to [Use External Data Roles in Request
Processing](Use_External_Data_Roles_in_Request_Processing.htm) for more
information.

The three global roles can be:

  - Modified without overriding settings at the template-role level
  - Copied to a template manually
  - Copied to a template automatically if the **Auto Copy** option is
    selected on the *Vertical* View of the *Roles* page, accessible by
    selecting **Configuration \> Roles** on the *Navigation pane*

A Template Administrator can also add a role at the template level only,
and is not required to add it to the pool of global roles. Changes to
template roles are not tied to global roles and apply only to the role
at the template level.

Refer to [Configure Global Roles](../Config/Configure_Global_Roles.htm)
for more information.

To configure template roles:

  - [Create Template Roles](Create_Template_Roles.htm)
  - [Add Role Dependencies](Add_Role_Dependencies.htm)
  - [Add Validations to Roles](Add_Validations_to_Roles.htm)
  - [Set Target Role for Request Rejections from a Review
    Role](Set_Target_Role_for_Request_Rejections.htm)
  - [Assign a Custom Page to a Template
    Role](Assign_a_Custom_Page_to_Template_Role.htm)
