+++
title = 'Reset a Role'
solution = 'Master Data Management'
+++

# Reset a Role

A Request Processer resets a role if a mistake is made or if information
is incomplete after a role with the type of Application or Review has
been finished.

This section contains the following topics:

  - [Reset a Role with the Review Role
    Type](#Reset_a_Role_with_the_Review_Role_Type)
  - [Reset a Role with an Application Role
    Type](#Reset_a_Role_with_an_Application_Role_Type)

## <span id="Reset_a_Role_with_the_Review_Role_Type"></span>Reset a Role with the Review Role Type

A Review role is reset when a Role Processor rejects a role \> task
combination during the review process.

Refer to [Review a Request](Review_a_Request_Overview) and [Reject a
Request](Reject_a_Request) for more information.

Before performing this task, a [request must have been
created](Create_a_Request) and a role with the type Application must
have been finished.

Resetting a Review role:

  - Resets all Application roles associated with the selected role \>
    task combination and all Application roles that are dependent on
    those roles.
  - Resets all dependency and workflow emails for all users assigned to
    the Application roles and their dependent roles.

<span style="font-weight: bold;">NOTE</span>: The DEPENDENCY COMPLETE
check box is no longer enabled for any dependent Application roles. No
buttons are active for the dependent role. The role that was reset must
be finished before work can begin for any dependent roles.

  - Sets the Application role with the lowest priority to active.
  - Retains any completed information.
  - Allows the Application role to edit the completed information.
  - Clears the FINISHED ON and FINISHED BY fields for the Application
    role and the Review role.

<span style="font-weight: bold;">NOTE</span>: These fields are populated
again when the role is finished.

  - Activates the Finish and Tasks icons for the Application role.
  - Dithers the Tasks, Finish, and Reject icons for the Review role

<span style="font-weight: bold;">NOTE</span>: The Reset process
initiates the workflow email to users assigned to the Application role
(if that role has messaging enabled). The Reset process displays a
notification from within dspConduct™ to users assigned to the role (if
that role has messaging enabled). Refer to [Enable or Disable Messages
for a Role](Enable_or_Disable_Messages_for_a_Role) for more
information.

<span style="font-weight: bold;">NOTE</span>: A user who is not assigned
to the request’s role but is assigned to a role in the Category can view
the role if the Auto Extend Display option is set for the role. This
user cannot update the
role.

## <span id="Reset_a_Role_with_an_Application_Role_Type"></span>Reset a Role with an Application Role Type

A Request Processer resets a role if a mistake is made or if information
is incomplete after a role with the type of Application or Review has
been finished.

Before performing this task, [a request must have been
created](Create_a_Request) and a [role with the type Application
must have been
finished](Finish_a_Role_with_the_Application_Role_Type).

When a request is reset, the user assigned to the Application role for
the request receives a notification depending on how the user and role
are configured. That email contains a link to the Request Role page, so
that the user can update the request as needed and finish the
Application role again.

Resetting a role:

  - Resets all dependency and workflow emails for all users assigned to
    the roles and dependent roles.
  - Resets dependent roles.

<span style="font-weight: bold;">NOTE</span>: The DEPENDENCY COMPLETE
check box is no longer enabled for the dependent role. No buttons are
active for the dependent role. The role that was reset must be finished
before work can begin for any dependent roles.

  - Sets the role to active.

<span style="font-weight: bold;">NOTE</span>: The role must be finished
for the request to continue processing.

  - Retains any completed information.
  - Allows the user to edit the completed information.
  - Clears the FINISHED ON and FINISHED BY fields for the role.

<span style="font-weight: bold;">NOTE</span>: These fields are populated
again when the role is finished.

  - Activates the Finish and Task buttons for the role.
  - Notifies the Requester who can access the role.

<span style="font-weight: bold;">NOTE</span>: The Reset process
initiates the workflow email to users assigned to the next role (if that
role has messaging enabled). The Reset process displays a notification
from within dspConduct™ to users assigned to the next role (if that role
has messaging enabled). Refer to [Enable or Disable Messages for a
Role](Enable_or_Disable_Messages_for_a_Role) for more information.

<span style="font-weight: bold;">NOTE</span>: A user who is not assigned
to the request’s role but is assigned to a role in the Category can view
the role if the Auto Extend Display option is set for the role. This
user cannot update the role.

<span style="font-weight: bold;">NOTE</span>: An Application role type
can be reset when the request is being reviewed. It cannot be reset once
the request is assigned to the Post role.

To reset a role in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    Requests</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    request.
    
    **NOTE:** The count on the Roles icon is the number of roles for the
    request. The count may not reflect the number of roles that display
    on the <span style="font-style: italic;">[Request
    Role](../Page_Desc/Request_Role_H)</span> page for the current
    user. The current user can only access roles to which that user is
    assigned and roles that have the Auto Extend Display setting
    enabled.

3.  Click <span style="font-weight: bold;">Reset</span> for the role
    with an Application type.
