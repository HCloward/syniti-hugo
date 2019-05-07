+++
title = 'Add a Rule to a Template Role Event'
solution = 'Data Quality'
+++

# Add a Rule to a Template Role Event

A Template Administrator can configure rules that run when events occur
at the template role level.

These rules are stored procedures stored in a data source that is
accessible to dspCompose™.

For Data roles and External Data roles, a rule can be configured to run
when a user:

  - Clicks Data Entry on the *[*Request
    (Roles)*](../Page_Desc/Request_Roles_H.htm)* page to enter or update
    request data

  - Validates the role by clicking **Validate** on the *Request (Roles)*
    page

**NOTE**: The **Validate** button displays for the Data and Review role
if role validations exist for the template. Refer to [Add Validations to
Roles](Add_Validations_to_Roles.htm) and [Enable Role
Validations](../Config/Enable_Role_Validations.htm) for more
information.

  - Finishes the role by clicking **Finish** on the *Request (Roles)*
    page

  - Resets the role by clicking **Reset** on the *Request (Roles)* page

For Review roles, a rule can be configured to run when a user:

  - Rejects a role

<!-- end list -->

  - Clicks Data Entry on the *Request (Roles)* page to review request
    data

  - Validates the role by clicking **Validate** on the *Request (Roles)*
    page

**NOTE**: The **Validate** button displays for the Data and Review role
if role validations exist for the template. Refer to [Add Validations to
Roles](Add_Validations_to_Roles.htm) and [Enable Role
Validations](../Config/Enable_Role_Validations.htm) for more
information.

  - Finishes the role by clicking **Finish** on the *Request (Roles)*
    page

  - Resets the role by clicking **Reset** on the *Request (Roles)* page

For Post roles, a rule can be configured to run when a user

  - Finishes the role by clicking **Finish** on the *Request (Roles)*
    page

  - Clicks Data Entry on the *Request (Roles)* page to post a request

**NOTE**: To add a rule, the template must not be active or must be in
Developer Mode. Refer to [Modify an Active Template in Developer
Mode](Modify_an_Active_Template_in_Developer_Mode.htm) for more
information.

To add a rule to a template role event:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Events** for the role.

5.  Click **Rules** for the event.
    
    *[View the field descriptions for the Template (Role Event Rule)
    page.](../Page_Desc/Template_Role_Event_Rule.htm)*

6.  Enter a sort order in **PRIORITY**.
    
    **NOTE**: If there are multiple event rules, the PRIORITY determines
    the order in which dspCompose™ runs the event rule.

7.  Select a data source from the **DATA SOURCE ID** list box to
    determine where the rule is stored.

8.  Select a rule from the **RULE** list box.
    
    **NOTE**: The **RULE** list box only displays rules stored in the
    data source.

9.  Click **Save**.
