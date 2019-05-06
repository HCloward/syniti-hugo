# Create Template Roles

If the following two settings are enabled for global roles, these roles
are automatically registered to a new template. The **Add Roles On
Template Creation** check box on the *Parameters* page (**Configuration
\> Parameters**) and the **Auto Copy** check box on the *Roles* page’s
*Vertical* View (**Configuration \> Roles**) are enabled by default.

Once a template is created, roles can be added or deleted as necessary.

A Template Administrator can add a custom role at the template level
only, and is not required to add it to the pool of global roles, or to
copy it from the list of global roles. Changes to template roles are not
tied to global roles and apply only to the role at the template level.
Updates to global roles do not overwrite changes to roles at the
template role level.

**NOTE**: When a user adds a role at the template level, that user is
automatically granted access to the template role. Any other users who
should be assigned to the template role must be granted access on the
*User Template Role Access* page, accessible from the *Navigation
<span style="font-style: normal;">pane</span>* by selecting
**Configuration \> Users \> Templates**.

**NOTE**: To add a role at the template level, the template must not be
active or must be in Developer Mode. Refer to [Modify an Active Template
in Developer Mode](Modify_an_Active_Template_in_Developer_Mode.htm) for
more information.

To create a role at the template level:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Add**.
    
    *[View the field descriptions for the Template (Role)
    page.](../Page_Desc/Template_Role_H.htm)*

5.  Enter the sort order in **PRIORITY
    <span style="font-weight: normal;">field</span>**, which determines
    the order the roles on a request are processed. The role with the
    lowest priority is processed first.
    
    **NOTE**: Priority should also control how dependencies are created.
    Roles should never be available for processing until the roles on
    which they depend have been processed. Role dependencies should
    never be set up such that, for example, a role with priority of 50
    would become available for processing before a role with priority of
    30 or 40 had been processed. Refer to [Add Role
    Dependencies](Add_Role_Dependencies.htm) for more information.

6.  Select an option from the **ROLE ID** list box.

7.  Click **Save**; the *Vertical* View displays.

8.  Click **Save**.
