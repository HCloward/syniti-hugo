+++
title = 'Review a Request Overview'
solution = 'Master Data Management'
+++

# Review a Request Overview

A Role Processor can review changes made to a task by dependent
Application roles.  These changes are entered on a page in the Content
WebApp, The Role Processor uses the Review role (any role with the role
type of Review) to approve or reject the request.

A Review role can be assigned the following task types.

All Application tasks assigned to Application and Display roles that the
Review role must review across all scenarios the Review role is assigned
to.

All Display tasks assigned to Application and Display roles that the
Review role has access to across all scenarios the Review role is
assigned to.

Any Review tasks the Reviewer must review in every scenario the Review
role is assigned to.

However, while reviewing a request, the Review role can review:

Application and Display tasks that have been assigned to the Review role
and have also been assigned to Application and Display roles that have
been assigned to the scenario.

Any Review task that has been assigned to the Review role.

By specifying the tasks a Review role can approve or reject, the request
workflow process can be tuned to restrict access to data to suit any
business need.

A Review role can be assigned a large set of tasks, allowing a single
Review role to be assigned to many scenarios. The reviewer can review
Application and Display tasks that have also been assigned to
Application and Display roles in each scenario.

A Review role can also be assigned a small set of tasks, allowing a
reviewer to review only those tasks in a request. For example, a
Designer can assign a Credit Approver Review role only those tasks
related to accounting and basic data about a customer.

When a request is rejected, the Review role is reset. Refer to [Reset a
Role with the Review Role
Type](Reset_a_Role.htm#Reset_a_Role_with_the_Review_Role_Type) for more
information.

When a request is Approved it moves to the Post role so that the changes
can be posted to the target system.

Refer to [Approve a Request](Approve_a_Request.htm) and [Reject a
Request](Reject_a_Request.htm) for more information.

The Review role can also [Review Request
Changes](Review_Request_Changes.htm).
