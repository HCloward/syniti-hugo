# Auto Finish a Role

A Designer can configure the Auto Finish Role setting on the
<span style="font-style: italic;">[Scenario
(Roles)](../Page_Desc/Scenarios_Roles_H.htm)</span> page’s
<span style="font-style: italic;">Vertical</span> View, which allows the
role to automatically finish if the role passes all validations. Auto
Finishing a role is useful when a request must pass through a role with
no action required from a user assigned to the role. For example, if a
request to update all fields with the same value in a table does not
need to be reviewed, the scenario role with the Review role type can be
configured to Auto Finish.

If the role fails any validations with an Error status, the role is not
finished.

The setting is available for roles of any role type.

Before performing this task at least one role must have been added to
the scenario. Refer to [Add a Role to a
Scenario](Add_a_Role_to_a_Scenario.htm) for more information.

If the Auto Finish Role setting is enabled for the Post role, and the
request posts unsuccessfully, the role automatically finishes with a
status of Posted with Errors.

To enable the Auto Finish Role setting for a scenario role:

1.  Select <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Scenarios</span> icon for
    a category.
3.  Click the <span style="font-weight: bold;">Roles</span> icon.
4.  Click <span style="font-weight: bold;">Vertical View</span> for role
    with the role type of Post.
5.  Click the <span style="font-weight: bold;">Auto Finish Role</span>
    check box to enable it.
