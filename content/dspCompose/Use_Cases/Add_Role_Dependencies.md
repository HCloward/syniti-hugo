+++
title = 'Add Role Dependencies'
solution = 'Data Quality'
+++

# Add Role Dependencies

Roles within a template can be dependent on other roles, meaning one
role cannot be finished until another is completed. Dependencies drive
the workflow notification process by emailing the user assigned to the
next dependent role.

Dependent roles run according to what is called *upstream dependency*,
meaning if Role 2 is dependent on Role 1 and Role 3 is dependent on Role
2, Role 3 must be defined to be dependent on both Role 1 and Role 2,
even though it is not directly dependent on Role 1.

**NOTE:** A role’s priority should also control how dependencies are
created. Roles should never be available for processing until the roles
on which they depend have been processed. Role dependencies should never
be set up such that, for example, a role with priority of 50 would
become available for processing before a role with priority of 30 or 40
had been processed.

**NOTE:** The dependencies configured for global roles are automatically
added to template roles. The Review role is dependent on the Data role.
The Post role is dependent on the Data Role and the Review role. These
dependencies cannot be changed at the global level. Click
**Dependencies** for a role to modify the configured dependencies for
the template.

**NOTE**: To add a role dependency to a template role, the template must
not be active or must be in Developer Mode. Refer to [Modify an Active
Template in Developer
Mode](Modify_an_Active_Template_in_Developer_Mode.htm) for more
information.

To register a dependency to a role:

1.  Click **Team** on *Navigation pane*.
2.  Click **Templates** for a team.
3.  Click **Roles** for a template.
4.  Click **Dependencies** for a role.
5.  Click the **DEPENDS** check box to enable it, indicating that the
    selected role is dependent upon this role. For example, a user
    selects **Dependencies** for the Review role. By default, the Data
    role will have the **DEPENDS** check box enabled, meaning that the
    Review role is dependent on the Data role.

**NOTE:** Add each upstream role the selected role should be dependent
upon.
