+++
title = 'Finish a Role with the Application Role Type'
solution = 'Master Data Management'
+++

# Finish a Role with the Application Role Type

A Role Processor uses the <span style="font-style: italic;">[Request
Role](../Page_Desc/Request_Role_H)</span> page to finish roles,
indicating that the work assigned to that role is complete for the
request.

Before performing this task, a request must have been created.  Refer to
[Create a Request](Create_a_Request) for more information.

Roles with the Application role type gather, enter, or make changes to
data using pages in the Content WebApp for preparation to send to the
system(s) of record. These pages are associated with tasks. To view the
tasks assigned to a role before finishing it, click the Tasks button on
the <span style="font-style: italic;">[Request
Role](../Page_Desc/Request_Role_H)</span> page.

<span style="font-weight: bold;">NOTE</span>: If multiple users are
assigned to the role, only one of those users is required to finish the
role.

<span style="font-weight: bold;">NOTE</span>: When a role is finished,
the system makes any dependent roles active, and notifies users assigned
to the roles that work is ready to be completed. Refer to Set
Dependencies for a Role for more information.

<span style="font-weight: bold;">NOTE</span>: If changes must be made to
tasks associated with a role with a type of Application after it is
finished, the Role Processor must reset the role. Refer to [Reset a
Role](Reset_a_Role) for more information.  

<span style="font-weight: bold;">NOTE</span>: The Finish process
initiates the workflow email to users assigned to the next role (if that
role has messaging enabled). The Finish process displays a notification
from within dspConduct™ to users assigned to the next role (if that role
has messaging enabled). Refer to [Enable or Disable Messages for a
Role](Enable_or_Disable_Messages_for_a_Role) for more information.

**NOTE**: A setting can be configured to finish this role automatically.
Refer to [Auto Finish a Role](Auto_Finish_a_Role) for more
information.

**NOTE**: If the User Response Required on Warnings option is enabled at
the Role or Scenario role level, after a user clicks Finish for the
role, any validation failures require a user response to continue the
process.

To finish a role in dspConduct™:

1.  Click <span style="font-weight: bold;">dspConduct \> Requests</span>
    in the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    request.
3.  Click the <span style="font-weight: bold;">Finish</span> button for
    a role with an Application type.   

The system tracks the user ID of the Role Processor and the date and
time the role was finished in the FINISHED BY and FINISHED ON fields.

<span style="font-weight: bold;">NOTE</span>: All validation rules and
business processes are run, dependencies are validated, and a workflow
email is sent to the users assigned to dependent roles as long as
workflow is enabled for the user. The role is not finished if validation
rules fail.
