+++
title = 'Enable or Disable Messages for a Role'
solution = 'Data Quality'
+++

# Enable or Disable Messages for a Role

If a user assigned to a role constantly works in a Content WebApp, the
application generates many messages in the form of emails  that may not
be useful. The Designer can disable messages so that the user assigned
to the role doesn’t receive messages via email.

Before performing this task, [Create a Category](Create_a_Category.htm)
and [Add a Role](Add_a_Role.htm).

Refer to [Manage Roles](Manage_Roles.htm) for more information about
roles.

dspConduct™ generates messages for roles as a request moves through the
workflow.

Messages are sent:

  - To a role with the Application role type when the dependencies for
    that role are completed and that role is ready for action
  - To a role with the Application role type when a request containing
    that role is reset (i.e., when a user assigned to the Application
    role type clicks the Reset button or when the Review role type
    clicks the Reject button on the
    <span style="font-style: italic;">[Request
    Role](../Page_Desc/Request_Role_H.htm)</span> page in dspConduct™)
  - To a role with the Review role type when all Application role types
    that have a predecessor dependency with that role are complete
    (i.e., when a role with the Application role type clicks the Finish
    button on the [Request Role](../Page_Desc/Request_Role_H.htm) page
    in dspConduct™)
  - To a role with the Post role type when all Review role types that
    have a predecessor dependency with that role are complete (i.e.,
    when a user assigned to the Review type role clicks the Approve
    button on the [Request Role](../Page_Desc/Request_Role_H.htm) page
    in dspConduct™)

For example, when a role with the Application role type clicks the
Finish button, the role with the role type of Review receives a message
that a request is ready for review.

<span style="font-weight: bold;">NOTE</span>: Role dependencies control
which role’s tasks are dependent on the completion of another role’s
tasks. Refer to [Add Dependencies to
Roles](Role_Dependencies.htm#Add_Dependencies_to_Roles) for more
information.

Messages are enabled by default.

To disable messages for a role in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \> Design
    </span>in the <span style="font-style: italic;">Navigation</span>
    pane.

2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    category.

3.  Click <span style="font-weight: bold;">Vertical View</span> for a
    role.

4.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Role page’s Vertical
    View](../Page_Desc/Role_H_dspConduct.htm#Role_V)

5.  Disable the <span style="font-weight: bold;">Send Workflow</span>
    check box.
    
    **NOTE:** Users assigned to this role do not receive workflow
    messages as the request moves through the workflow.

6.  Click <span style="font-weight: bold;">Save</span>.
