+++
title = 'Post a Request'
solution = 'Data Quality'
+++

# Post a Request

A Role Processor with the Post role type posts a request to a target
system after the Review role is finished.

When a Role Processor posts a request for the Post role, the request can
be posted by:

  - The Integrate process assigned to the scenario (used when posting to
    SAP). Refer to [Add a Process to a
    Scenario](Add_an_Integrate_Process_to_a_Scenario.htm) for more
    information.
  - Manual post. Refer to Use Manual Post for more information.
  - A custom posting process developed for a target system.

<span style="font-weight: bold;">NOTE</span>: Custom posting pages or
processes are created and maintained by users.

Posting takes place on the<span style="font-style: italic;">[Request
Group Post](../Page_Desc/Request_Group_Post.htm)</span> and [Request
Post Process](../Page_Desc/Request_Post_Process.htm) pages, which are
automatically assigned to any role with the role type of Post.

A post can be posted individually or as a group post, which posts each
process in priority order. The lowest priority is posted first.

dspConduct™ updates the request status during the posting process.

A request moves to the Posting Started status when a Post role clicks
the Post or Group Post icon on the [Request Group
Post](../Page_Desc/Request_Group_Post.htm) and [Request Post
Process](../Page_Desc/Request_Post_Process.htm) pages.  

A request moves to the Posted with Errors status when all Integrate
processes associated with the request are finished processing and at
least one posting process has failed.

A request moves to the Posted status when all Integrate processes
associated with the request are finished processing and all postings are
successful.

<span style="font-weight: bold;">NOTE</span>: When a Request is created,
each Integrate Process assigned to the Scenario is assigned a unique
Posting ID which can be used to assist while troubleshooting. Integrate
uses this Posting ID as a parameter for Integrate Process Template rules
and validations. The Integrate Process is also passed a Where Clause
used for the posting data views that only contains the Request ID (e.g.
“WHERE RequestID = 999”).

<span style="font-weight: bold;">NOTE</span>: After a request is
finished, the Post role can be finished, during which the Final Finish
process runs. The data that was posted is downloaded into target tables.
Refer to [Finish a Role with the Post Role
Type,](Finish_a_Role_with_the_Post_Role_Type.htm) and Register Tables
for Download as a Finish Process in dspConduct™.

**NOTE: <span style="font-weight: normal;">A post can be posted multiple
times. The messages related to posting failure or success on the
[Request Post Message](../Page_Desc/Request_Post_Message.htm) page
displays information about the latest post.</span>**

**NOTE**: A setting can be configured to automatically post a request.
Refer to [Auto Post a Request](#Auto_Post_a_Request) for more
information.

<span style="font-weight: bold;">NOTE</span>: A dependent scenario may
exist in another category. Refer to [Allow a Scenario to be used in
Other Categories](Allow_a_Scenario_to_be_used_in_Other_Categories.htm)
for more information.  When a business process uses a scenario from
another category, the request that is created for that scenario will be
created in the database/Webapp that is the default WebApp for that other
category. For example, a category called Northwest Region has a default
WebApp of NWRegion. It  contains a scenario called Create SoldTo –
General Data. This scenario has been configured for use in the category
US Operations. A scenario in US Operations is Create SoldTo. A user
could create a business process in the US Operations category that uses
the Create SoldTo scenario as a parent of the Create SoldTo – General
Data scenario from the Northwest Region category. When the business
process is executed, a request is created in the NWRegion WebApp.  

This section contains the following topics:

  - [Post a Request](#Post_a_Request)
  - [Auto Post a Request](#Auto_Post_a_Request)
  - [Use Manual Post](#Use_Manual_Post_)
  - [Schedule a Post for a Specified Date and
    Time](#Schedule_a_Post_for_a_Specified_Date_and_Time)

## <span id="Post_a_Request"></span>Post a Request

A Role Processor with the Post role type can post a request to a target
system.

<span style="font-weight: bold;">NOTE</span>: Credentials must be
detected to post data. The Credentials Detected check box on the
<span style="font-style: italic;">[Request Group
Post](../Page_Desc/Request_Group_Post.htm)</span> page must be enabled.
If it is disabled, set credentials. Refer to [Add Stored Credentials as
a User on a Page in
Integrate](../../../Data_Quality/dspCompose/Config/Add_Stored_Credentials_as_a_User_on_a_Page_in_Integrate_or_dspCompose.htm)
for more information.

To post a request in dspConduct™:

1.  Click <span style="font-weight: bold;">dspConduct \> Requests</span>
    in the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    request.
3.  Click the <span style="font-weight: bold;">Tasks</span> icon for the
    post role.
4.  Click <span style="font-weight: bold;">Request Post</span>.
5.  Click the <span style="font-weight: bold;">Group Post</span> icon on
    the <span style="font-style: italic;">[Request Group
    Post](../Page_Desc/Request_Group_Post.htm)</span> page to run each
    posting process listed on the
    <span style="font-style: italic;">[Request Post
    Process](../Page_Desc/Request_Post_Process.htm)</span> page
6.  Click the <span style="font-weight: bold;">Post</span> icon for a
    process on the <span style="font-style: italic;">[Request Post
    Process](../Page_Desc/Request_Post_Process.htm)</span> page.
7.  A confirmation message displays; click
    <span style="font-weight: bold;">OK</span>.
8.  After the Posting Status updates to Success or Failure, click the
    Message icon for each process to view details.

<span style="font-weight: bold;">NOTE</span>: A Designer can configure
users to receive workflow notifications when the posting status is
updated to Success or Failed. Refer to [Send Workflow Notifications when
a Post Fails or
Succeeds](../Config/Send_Workflow_Notifications_when_a_Post_Fails_or_Succeeds.htm)
for more information.

Continue with [Finish a Role with the Post Role
Type](Finish_a_Role_with_the_Post_Role_Type.htm).

## <span id="Auto_Post_a_Request"></span>Auto Post a Request

A Designer can configure the Auto Post Role setting on the
<span style="font-style: italic;">[Scenario
(Roles)](../Page_Desc/Scenarios_Roles_H.htm)</span> page’s
<span style="font-style: italic;">Vertical</span> View, which allows a
request to be automatically posted after all data dependencies have been
completed, all validations have passed, and the Review role approves the
request. In this case, a user assigned to the Post role does not click
the Post button to initiate the posting.

Before performing this task a role with the Post role type must exist in
the scenario. Refer to [Add a Role to a
Scenario](Add_a_Role_to_a_Scenario.htm) for more information.

Refer to [Post a Request Overview](Post_a_Request.htm) for general
information.

If the request posts unsuccessfully the Post role must take further
action, unless the Auto Finish Role setting is enabled for the Post
role. In this case, the role automatically finishes with a status of
Posted with Errors. Refer to [Auto Finish a
Role](Auto_Finish_a_Role.htm) for more information.

**NOTE**: When using Auto Post, the Post Workflow Notification records
at the specific Scenario's Post role are used to determine which users
receive posting success or failure notifications.

<span style="font-weight: bold;">NOTE:</span> The Auto Post Role feature
can only be used if default credentials are set for all connections used
by the scenario's Integrate processes. Refer to [Add a Process to a
Scenario](Add_an_Integrate_Process_to_a_Scenario.htm) and [Add Default
User Credentials to a
Connection](../../../Platform/Common/Use_Cases/Add_Default_User_Credentials_to_a_Connection.htm)
for more information.

To enable the Auto Post Role setting for a scenario role with the Post
role type:

1.  Select <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Scenarios</span> icon for
    a category.

3.  Click the <span style="font-weight: bold;">Roles</span> icon.

4.  Click <span style="font-weight: bold;">Vertical View</span> for a
    role with the role type of Post.

5.  Click the <span style="font-weight: bold;">Auto Post Role</span>
    check box to enable it.
    
    **NOTE:** This check box only displays for roles with a role type of
    Post.

## <span id="Use_Manual_Post_"></span>Use Manual Post

A user assigned to a role with a role type of ManualPost can use
dspConduct™ workflow to track completion of tasks that are performed
manually outside of dspConduct™.

A ManualPost role receives notification that work can be started, and
finishes that work by using a custom post process or performing a
physical task. When the task is complete, the ManualPost role user
clicks Finish on the <span style="font-style: italic;">[Request
Role](../Page_Desc/Request_Role_H.htm)</span> page. dspConduct™ only
tracks the name of the user who clicked the button and the time the
Finish button was clicked. There is no Integrate, Collect or dspConduct™
processing associated with the ManualPost role.

Depending on how the Business Process is configured, a dependent
scenario may begin after the ManualPost role finishes.

Refer to [Add a Dependent Scenario to a
Scenario](Add_a_Dependent_Scenario.htm) for more
information.

## <span id="Schedule_a_Post_for_a_Specified_Date_and_Time"></span>Schedule a Post for a Specified Date and Time

A Role Processor with the Post role type can schedule a post to process
at a date and time in the future.

Before a Role Processor can perform this task, a Designer must enable
this feature at the
[role](Configure_the_Post_Later_Feature_at_the_Role_Level.htm) or
[scenario
role](Configure_the_Post_Later_Feature_at_the_Scenario_Role_Level.htm)
level.

To schedule a post:

1.  Click <span style="font-weight: bold;">dspConduct \> Requests</span>
    in the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    request.
3.  Click the <span style="font-weight: bold;">Tasks</span> icon for the
    Post role.
4.  Click the <span style="font-weight: bold;">Task ID</span>.
5.  Click <span style="font-weight: bold;">Edit</span>.
6.  Click the <span style="font-weight: bold;">Post Start Time
    </span>field and select the date and time in the calendar.
7.  Click <span style="font-weight: bold;">Save</span>.
8.  Click <span style="font-weight: bold;">Schedule Post</span>.
