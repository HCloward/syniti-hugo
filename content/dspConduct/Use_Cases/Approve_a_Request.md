+++
title = 'Approve a Request'
solution = 'Master Data Management'
+++

# Approve a Request

A Role Processor can approve a request for a Review role.

Before performing this task, a request must have been submitted via the
Content WebApp. The request passes to the Review role after all
dependencies are complete for the Application role and the final
Application role (the role with the highest priority) is finished.

Refer to [Review a Request Overview](Review_a_Request_Overview) for
general information about the review process.

**NOTE**: If the User Response Required on Warnings option is enabled at
the Role or Scenario role level, after a user clicks Finish for the
role, any validation failures require a user response to continue the
process.

To approve a request in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    Requests</span> in the Navigation pane.

2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    request.
    
    **NOTE:** The count on the Roles icon is the number of roles for the
    request. The count may not reflect the number of roles that display
    on the <span style="font-style: italic;">[Request
    Role](../Page_Desc/Request_Role_H)</span> page for the current
    user. The current user can only access roles to which that user is
    assigned and roles that have the Auto Extend Display setting
    enabled.

3.  Click the <span style="font-weight: bold;">Tasks</span> icon for a
    Review role.
    
    **NOTE:** The Tasks icon for the Review role is disabled until the
    request is finished by the highest priority Application role.

4.  Click the <span style="font-weight: bold;">TASK ID</span> button to
    review changes entered by the Application role(s).

5.  Navigate to the [Request Role](../Page_Desc/Request_Role_H)
    page.

6.  Click the <span style="font-weight: bold;">Approve</span> icon for
    the Review role.

Continue with [Post a Request](Post_a_Request).
