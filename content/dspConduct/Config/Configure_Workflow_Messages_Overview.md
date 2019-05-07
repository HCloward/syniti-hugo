+++
title = 'Configure Workflow Messages Overview'
solution = 'Data Quality'
+++

# Configure Workflow Messages Overview

Requests are workflow-enabled, meaning that each user assigned to a role
in a request receives a notification when the tasks assigned to that
role have work assigned.

For example, when a user finishes a role by clicking Finish on the
<span style="font-style: italic;">[Request
Role](../Page_Desc/Request_Role_H.htm)</span> page, the Finish event is
triggered, and an email notification and/or a pop-up notification from
within dspConduct™ is sent to the next person(s) responsible for
subsequent role(s). The email and notification contain the workflow
message associated with the Finish event.

Users can set whether or not they receive notifications and the form in
which the notifications are sent (either via email or notifications from
within dspConduct™, or both). An Administrator can configure these
options for multiple users.

Refer to [Set User Workflow Receipt
Preferences](Set_User_Workflow_Receipt_Preferences.htm) for more
information about receipt options.

By default, dspConduct™ sends workflow messages to users who have access
to a request when a request is created, canceled, deleted, finished,
rejected or reset. A user can view the default messages installed, but
cannot update them. These default messages are used as a starting point
for all dspConduct™ categories.

<span style="font-weight: bold;">NOTE</span>: A Designer must navigate
to the [Category Workflow Language
Message](../Page_Desc/Category_Workflow_Language_Message_H.htm) page for
workflow message definitions to be created for active Languages.  If a
Designer does not navigate to the Category Workflow Language Message
page, no workflow message definitions will be available, and no
workflows messages will be sent.

**NOTE:** Workflow Messages for SLA notifications are sent when a time
constraint for completing tasks within a request role has passed. Refer
to [Setting up SLA notifications in
dspConduct™](Set_Up_SLA_Notifications.htm) for more information.

If the notification text must use a language other than English, a user
must [Create Language-specific Workflow Messages for a
Category](Create_Language-specific_Workflow_Messages_for_a_Category.htm).

A user can also [View Default Workflow
Messages](View_Default_Workflow_Messages.htm) or [Edit Category
Language-specific
Messages.](Edit_Category_Language_specific_Messages.htm)

<span style="font-weight: bold;">NOTE</span>: A user can create custom
workflow message events at the category level. These events must have
different names than the default events that were installed with
dspConduct™. For example, a user cannot create a custom workflow message
event with the name “Deleted.” The Content WebApp must provide the code
to process these messages. They are not processed by dspConduct™.

The following table lists the type of workflow messages and the type of
user that receives
them.

|                                                                       |                                                                                                                                                                                                                                                                                     |
| --------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Event                                                                 | Type of User that Receives Workflow                                                                                                                                                                                                                                                 |
| All roles in a request are rejected.                                  | Users who have access to the initial application role                                                                                                                                                                                                                               |
| A task for a request role is rejected.                                | Users who have access to that role                                                                                                                                                                                                                                                  |
| Request is canceled.                                                  | Users who have access to the request                                                                                                                                                                                                                                                |
| Request is deleted.                                                   | Users who have access to the request                                                                                                                                                                                                                                                |
| Role is reset.                                                        | Users who have access to the role that was reset. Also users who have access to subsequent roles that depend on the role that was reset will receive a workflow notifying them that the role was reset; they will receive another workflow when it is time to reprocess their role. |
| Role is finished.                                                     | Users who have access to next role to be processed in the scenario                                                                                                                                                                                                                  |
| Application role is finished and Review role is available.            | Users who belong to the Review role, if auditing is turned on in the Content WebApp and the tables that are used to add role data have been updated. Refer to [Review Request Changes](../Use_Cases/Review_Request_Changes.htm) for more information.                               |
| Request is submitted (Role is made active and ready to be processed). | Users who have access to the initial application role                                                                                                                                                                                                                               |
| Request posts successfully.                                           | Users configured to receive these notifications at the scenario role or request role level. Refer to [Send Workflow Notifications when a Post Fails or Succeeds](Send_Workflow_Notifications_when_a_Post_Fails_or_Succeeds.htm) for more information.                               |
| Request fails to post.                                                | Users configured to receive these notifications at the scenario role or request role level. Refer to [Send Workflow Notifications when a Post Fails or Succeeds](Send_Workflow_Notifications_when_a_Post_Fails_or_Succeeds.htm) for more information.                               |
| Final Finish package is created but does not run successfully.        | Users who belong to the Final Finish Admin WebApp group receive these notifications. Refer to [Send Workflow Notifications when a Final Finish Package Fails](Send_Workflow_Notifications_when_a_Final_Finish_Package_Fails.htm) for more information.                              |
