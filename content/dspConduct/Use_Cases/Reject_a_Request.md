+++
title = 'Reject a Request'
solution = 'Master Data Management'
+++

# Reject a Request

A Role Processor can reject a request (a role \> task combination) for a
Review role.

Before performing this task, a request must have been submitted via the
Content WebApp. The request must have passed to the Review role after
all dependencies are complete for the Application role and the final
Application role (the role with the highest priority) is finished.

Refer to [Review a Request Overview](Review_a_Request_Overview.htm) for
general information about the review process.

A Reviewer may enter a reject reason for a Review role. The Reviewer may
then click Reject for the Review role. At that rejection time, the user
assigned to the Application role for the request receives a notification
about the rejection depending on how the user and role are configured.
That email contains a link to the
<span style="font-style: italic;">[Request
Role](../Page_Desc/Request_Role_H.htm)</span> page, so that the user can
update the request as needed and finish the Application role again.

When a Review role is rejected, the review role is reset. Refer to
[Reset a Role with a Review Role
Type](Reset_a_Role.htm#Reset_a_Role_with_the_Review_Role_Type) for more
information.

**NOTE**: If the User Response Required on Warnings option is enabled at
the Role or Scenario role level, after a user clicks Finish for the
role, any validation failures require a user response to continue the
process.

To reject a request in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    Requests</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    request.

3.  Click the <span style="font-weight: bold;">Tasks</span> icon for a
    Review role.
    
    **NOTE:** The Tasks icon for the Review role is disabled until the
    Application role(s) with the highest priority is finished.

4.  Click the <span style="font-weight: bold;">TASK ID</span> button to
    review changes entered by the Application role(s).

5.  Navigate back to the <span style="font-style: italic;">[Request Role
    Task](../Page_Desc/Request_Role_Task.htm)</span> page.

6.  Click the <span style="font-weight: bold;">Reviewer Workbench
    </span>icon on the Page toolbar.
    
    **NOTE:** The <span style="font-style: italic;">[Request Review
    Task](../Page_Desc/Request_Review_Task.htm)</span> page opens in a
    new tab so that the Role Processor can review the task while working
    on the rejection.

7.  Click the <span style="font-weight: bold;">Roles</span> icon for the
    task.
    
    **NOTE:** The count on the Roles icon is the number of roles for the
    request. The count may not reflect the number of roles that display
    on the <span style="font-style: italic;">[Request
    Role](../Page_Desc/Request_Role_H.htm)</span> page for the current
    user. The current user can only access roles to which that user is
    assigned and roles that have the Auto Extend Display setting
    enabled.
    
    <span style="font-weight: bold;">NOTE</span>: The request is not
    rejected until this icon is clicked. The
    <span style="font-style: italic;">[Request Role
    Task](../Page_Desc/Request_Role_Task.htm)</span> page displays all
    of the Application tasks that are assigned to Application and
    Display roles in the scenario. Application tasks are the only tasks
    that display, as these are the only tasks that can be edited.
    
    **NOTE:** If the same task is assigned to multiple roles, the Review
    role can reject a specific role \> task combination.
    
    **NOTE:** To search for a field in the request and the roles that
    can access that field, the user can click the Column Search icon.
    Refer to [Search for Scenario Role Task Column Assignments while
    Reviewing a
    Request](Search_for_Scenario_Role_Task_Column_Assignments_while_Reviewing_a_Request.htm)
    for more information.

8.  Click the Review Changes icon on the [Request Review
    Task](../Page_Desc/Request_Review_Task.htm) page to display the
    updates to the task to determine whether to approve or reject them.

9.  Click <span style="font-weight: bold;">Edit</span> for a role
    assigned to the task to reject.
    
    **NOTE:** Multiple roles can be assigned to a task and rejected
    individually.  
    
    [View the field descriptions for the Request Review Task Roles
    page.](../Page_Desc/Request_Review_Task_Roles.htm)

10. Click the <span style="font-weight: bold;">REJECTED</span> check box
    to enable it.

11. Enter the reason for the rejection in the
    <span style="font-weight: bold;">REJECT REASON</span> field.
    
    A rejection reason is required when rejecting a role.

12. Click <span style="font-weight: bold;">Save</span>.

13. Click the <span style="font-weight: bold;">Reject</span> icon in the
    Page toolbar of the <span style="font-style: italic;">[Request
    Review Task](../Page_Desc/Request_Review_Task.htm)</span> page.
    
    <span style="font-weight: bold;">NOTE</span>: The request is not
    rejected until this icon is clicked.

The Application role is reset. The Finish icon for that role is active
and the request must be updated and finished again.
