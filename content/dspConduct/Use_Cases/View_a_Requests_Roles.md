+++
title = 'View a Request’s Roles'
solution = 'Master Data Management'
+++

# View a Request’s Roles

On the <span style="font-style: italic;">[Request
Role](../Page_Desc/Request_Role_H)</span> page, a Role Processor can
review the roles assigned to requests to which the user has access. Only
requests with roles that are assigned to the current user display.

Before performing this task, [add a role](Add_a_Role), [add a task
to the role](Add_a_Task_to_a_Role), and [create a
request](Create_a_Request).

<span style="font-weight: bold;">NOTE</span>: The logged in user must
have been assigned to the role.

<span style="font-weight: bold;">NOTE</span>: If a role has the Auto
Extend Display option set, this role displays as read only for all users
assigned to roles in the Category. In other words, if a user is not
assigned to a role, but the Auto Extend Display option is enabled for a
role, the user can view (but not update) the role for the request
regardless of whether the user is assigned to the role.

The role no longer displays on the
<span style="font-style: italic;">[Request
Role](../Page_Desc/Request_Role_H)</span> page when the request:

  - Has posted successfully to the target system (in the case of roles
    with the Auto Extend Display option enabled)
  - Has been assigned to another role to which the current user is not
    assigned
  - Is cancelled or deleted

To view a request’s roles in dspConduct™:

1.  Click <span style="font-weight: bold;">dspConduct \> Requests</span>
    in the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    request.
