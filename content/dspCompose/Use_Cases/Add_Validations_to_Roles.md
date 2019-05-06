# Add Validations to Roles

Role validations allow for template-specific data standards to be
applied at both the role and the request level. dspCompose™ runs
validations registered to roles when a user assigned to that role enters
a record for the request, or when a user clicks **Validate** for a role
on the *Request (Roles)* page.

**NOTE:** Role validations are views stored in a data source, typically
the cMass\_Data database. The view must exist in the database before the
role validation can be added to the template.

Validations related to list boxes, check boxes, and required fields can
also be triggered when validating a role, if certain parameters are
enabled. Refer to [Enable Role
Validations](../Config/Enable_Role_Validations.htm) for more
information.

A user can also:

  - Import validations from the registered page

  - Register validations from any pages in any component

Page-level validations run against the pages to which they are
registered and tie registration failures to that page. Role-level
validations are tied to the page assigned for the template role.

**NOTE**: All registered validation views must contain the Request ID
and ID columns from the Data Entry page for the template.

**NOTE**: To add validations to a role at the template level, the
template must not be active or must be in Developer Mode. Refer to
[Modify an Active Template in Developer
Mode](Modify_an_Active_Template_in_Developer_Mode.htm) for more
information.

**NOTE**: If a template with Org Units uses role validations, the
security view must be added to that role validation rule. Org Unit
security can then restrict validation failures to records associated
with Org Unit values, and users will only see validation failures for
records they can access. Refer to [Add the Org Unit Security View to
Template Role Validation Rules](Add_the_Org_Unit_Security_View_to.htm)
for more information.

To add role validations to a template:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Validations** for a role.

5.  Click **Add**; *Vertical* View displays.
    
    *[View the field descriptions for the Template (Role Validations)
    page’s Vertical
    View.](../Page_Desc/Template_Role_Validations_H.htm)*

6.  Enter sort value in **Priority** field.
    
    **NOTE**: If there are multiple validations, the priority is the
    order in which the validations are run.

7.  Select an option from the **WebApp ID** list box if adding a page
    validation rule.
    
    **NOTE**: The WebApp ID contains the page with the validation
    registered.

8.  Select an option from the **Page ID** list box if adding a page
    validation rule.
    
    **NOTE**: Validations are registered on this page. The page is
    contained in the WebApp selected in the WebApp ID list box.

9.  Select an option in the **Object Name** list box if adding a page
    validation rule.
    
    **NOTE**: The Object Name is the validation to import to the
    template role.

10. Select a data source from **Data Source ID** list box if adding a
    role-level validation.
    
    **NOTE**: The Data Source ID contains the validation.

11. Select an option from the **Role Object Name** list box.
    
    **NOTE**: The Role Object Name is the role-level validation.

12. Select severity from **Severity** list box.
    
    **NOTE**: The Severity determines the severity of the failure if a
    page-level or role-level validation fails.
    
    **NOTE: **Validation rules are assigned a **Severity**:
    
      - **Error** – Marks the role status as
        <span style="font-style: italic;">invalid</span> until the error
        is corrected and the validation rule passes.
    
      - **Message** – Marks the role status as
        <span style="font-style: italic;">valid</span> but a message
        displays.
    
      - **Warning** – Displays a message but the user can proceed with
        the task even if the validation fails.

13. Enter validation error text in **Comment** text field.
    
    **NOTE:** The Comment is the message that will display to the user
    if the validation fails.

14. Click **Save**.

Refer to [Validate a Role](Validate_a_Role.htm) for more information.
