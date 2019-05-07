+++
title = 'Reset a Role'
solution = 'Data Quality'
+++

# Reset a Role

Reset a role if a mistake is made or if information is incomplete after
the Data or Review role have been finished.

If the Review role rejects or partially rejects a request, the Data
Entry role(s) on which the Review role is dependent will be
automatically reset.

A role can also be reset manually.

**NOTE**: The Data Entry role and the Review role can use the reset
feature. The Post role cannot use this feature.

Resetting a role resets all dependency and workflow emails for all users
assigned to the roles and dependent roles. Any completed information
remains and can be edited.

**NOTE**: If the request has Org Units assigned, dspCompose™ will only
send workflow emails to users who have Org Unit security for values on
the request.

<span style="font-weight: bold;">NOTE</span>: The Reset process
initiates the workflow email to users assigned to the next role (if the
SEND WORKFLOW check box is enabled on the *User* page for this user).
The Reset process displays a notification from within dspCompose™ to
users assigned to the next role (if the SEND NOTIFICATION check box is
enabled on the *User* page for this user).

To reset a role:

1.  Click the **Workflow** link in the email to be directed to the
    request.
    
    *Or*  
    Select **Requests** on the *Navigation* pane.

2.  Click **Roles** for a request.
    
    **NOTE:** The count on the **Roles** icon is the number of roles the
    current user can access, not the total number of roles for the
    request.

3.  Click **Reset** for the Date Entry or Review role.

**NOTE:** The user(s) assigned to the role that was reset are notified
via email and pop-up notification within dspCompose™ that the role must
be completed.
