+++
title = 'Request Group Post'
solution = 'Master Data Management'
+++

# Request Group Post

<div class="use">

Use this page to:

  - [Post a Request](../Use_Cases/Post_a_Request.htm#Post_a_Request)
  - [Schedule a Post for a Specified Date and
    Time](../Use_Cases/Post_a_Request.htm#Schedule_a_Post_for_a_Specified_Date_and_Time)

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspConduct
    \></span><span style="font-weight: bold;">Requests</span> in the
    *Navigation* pane.
2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    request.
3.  Click the <span style="font-weight: bold;">Tasks</span> icon for the
    post role.
4.  Click the name of the task used to post requests.

Field

Description

Request ID

Displays the unique ID generated for the request when it was created in
the Content WebApp.

Scenario ID

Displays the name of the scenario to which the request belongs.

Request Status

Displays the name of the
<span id="Request Status dspConduct" class="popUpLink">request
status</span>.

Posted On

Displays the date of the latest posting.

Posted By

Displays:

  - The user ID of the user who clicked the Group Post icon on this page
    or
  - The user ID of the user who clicked Post icon on the Request Post
    Process page or
  - Process if the Post role is set to Auto Post

Refer to [Auto Post a
Request](../Use_Cases/Post_a_Request.htm#Auto_Post_a_Request) for more
information.

Posting

Credentials Detected

If enabled, credentials have been detected for the connection used by
the Integrate process.

If disabled, the Integrate process does not have credentials set.

Credentials must be set for the connection to post successfully. Refer
to [Add Stored Credentials as a User on a Page in
Integrate](../../../Data_Quality/dspCompose/Config/Add_Stored_Credentials_as_a_User_on_a_Page_in_Integrate_or_dspCompose.htm)
for more information.

Posting Credentials

Click to open the [User
Credentials](../../../Platform/Common/Page_Desc/User_Credentials_H.htm)
page to add or update user credentials for the connection to the data
source used to post the request.

By default, the system uses the user credentials associated with the
data source. Refer to [Establish a Connection to a Target
System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
for more information. 

Group Post

Click to post each process in the request in priority order.

Post Process

Click to open the <span style="font-style: italic;">[Request Post
Process](Request_Post_Process.htm)</span> page to view all post
processes and to post an individual process if needed.

Post Later

**NOTE:** This label and the fields below it display if the Scheduled
Post Allowed check box is enabled at the [Scenario
Role](../Use_Cases/Configure_the_Post_Later_Feature_at_the_Scenario_Role_Level.htm)
level for this request.

Schedule Post

Click to set the post to run at the time set in the Post Start Time
field.

The request status updates to Scheduled.

Post Start Time

Displays the date and time the request will post.

Scheduled By

Displays the name of the user who clicked the Schedule Post icon.
