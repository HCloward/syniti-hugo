+++
title = 'Finish a Role with the Post Role Type'
solution = 'Master Data Management'
+++

# Finish a Role with the Post Role Type

Roles with the Post role type send the collected and validated data to
the system(s) of record after all dependent Application and Review roles
are completed.

A Role Processor uses the *[Request
Role](../Page_Desc/Request_Role_H.htm)* page to finish roles, indicating
that the work assigned to that role is complete for the request. Once
the user clicks the Finish button, the Final Finish process runs. At
this point, the request status is either:

  - **Finish Processing** - This Request has been posted and is awaiting
    Finished data download.

<span style="font-weight: bold;">NOTE</span>: A request is in this
status when a user clicks the Finish button for the Post role but no
results have come back to dspConduct™ request yet.  Depending on
processing time, a user may not see the request in this status. For
example, if a CranPort package download processes in a few seconds, the
Finish Processing status does not display for the user.

  - **Finish Failed** - This Request has been posted but the downloading
    of Finished data failed.
  - **Finished** - This Request has been posted and the Finished data
    has downloaded successfully.

Refer to [Final Finish Process for a
Reque](Final_Finish_Process_for_a_Request_Overview.htm)st for more
information.

<span style="font-weight: bold;">NOTE</span>: The Post role cannot
finish until the request has been posted. The request may be in a
request status of Posted, meaning that the request has posted all data
without errors. The request may instead be in a request status of Posted
with Errors, meaning that at least one posting process has failed.

Before performing this task, a request must have been approved or the
Review Role must be set to AutoFinish. Refer to [Approve a
Request](Approve_a_Request.htm) and [Auto Finish a
Role](Auto_Finish_a_Role.htm) for more information.

After the Final Finish process, when the Post role is finished:

  - All Integrate processes associated with the scenario have completed.
  - The request status is Finished.
  - A request is automatically created for any dependent scenarios.

<span style="font-weight: bold;">NOTE</span>: Dependent scenario
requests are created by dspConduct™ when dependencies for scenarios
within the business process are completed. Dependencies are considered
completed even when a scenario exists as a dependency but is not
technically part of the business process. Refer to [Business Process
Execution during Final
Finish](Business_Process_Execution_During_Final_Finish.htm) for more
information.

  - The users assigned to the Application role for the dependent
    scenario’s request receive a notification that work on the newly
    created request can begin. Refer to [Add a Dependent Scenario to a
    Scenario](Add_a_Dependent_Scenario.htm) for more information.

<span style="font-weight: bold;">NOTE</span>: A setting can be
configured at the Category level to post data automatically after all
dependent roles are complete (i.e., the Application role(s) is finished
and the Review role has approved the updates.)  In this case, the
request process bypasses the Post role, and that role does not need to
finish the request. Refer to [Create a Category](Create_a_Category.htm)
and [Auto Post a Request](Post_a_Request.htm#Auto_Post_a_Request) for
more information.  

<span style="font-weight: bold;">NOTE</span>: For new requests that are
automatically created as part of a multi-scenario business process, the
Content Request page OnValidate event is automatically executed. The
Cransoft UserID 'process' must have access to the Content Request page
in order to execute the OnValidate event.

A Role Processor can view the details of finished roles, including the
name of the user who finished the role and the date and time the role
was finished. Using this information, a Role Processor can follow up
with users for additional information, if needed.

<span style="font-weight: bold;">NOTE</span>: If multiple users are
assigned to the role, only one of those users must finish the role.

**NOTE**: If the User Response Required on Warnings option is enabled at
the Role or Scenario role level, after a user clicks Finish for the
role, any validation failures require a user response to continue the
process.

To finish a role with the Post role type in dspConduct™:

1.  Click <span style="font-weight: bold;">dspConduct \>
    </span>**Requests** in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click the **Roles** icon for a request.
3.  Click **Finish** for the Post role.

**NOTE**: When a user clicks the Finish icon for a Post role, a
validation stored procedure runs to check for any post errors. If post
errors exist, a warning message displays. This feature ensures a request
is not finished with posting errors without the user’s permission.

The system tracks the user ID of the Role Processor and the date and
time the role was finished in the FINISHED BY and FINISHED ON fields.

After posting, a Role Processor can review posting messages. If a
posting failed, a user can correct any errors based on these message and
post the request again.
