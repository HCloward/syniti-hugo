# Request (Post)

<div class="use">

Use this page to [Post Request Data to a Target ERP
System](../Use_Cases/Post_Request_Data_to_a_Target_ERP_System.htm) and
[Set the Post Start Time.](../Use_Cases/Setting_the_Post_Start_Time.htm)

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspCompose \>
    Requests</span> in the *Navigation* pane*.*
2.  Click <span style="font-weight: bold;">Roles</span> for a request.
3.  Locate<span style="font-weight: bold;"> Post Role ID</span>.
4.  Click <span style="font-weight: bold;">Request (Post)</span> for
    the Post ROLE ID.

Field

Description

Connections

Click to open the *[Request Post
Connections](Request_Post_Connections.htm)* page to view the connection
to the target system for each Integrate template associated with the
request.

Credentials Detected

If enabled, the user name and password have been detected based on the
user credentials setting.

If disabled, the credentials have not been detected and must be added
for the request to post successfully.

Refer to [Establish a Connection to a Target
System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
for more information.

Post Now

Foreground Post

Click to immediately post request data to a target ERP system in the
foreground.  

The user credentials used to post data can be acquired using the methods
outlined in [Establish a Connection to a Target
System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm).

**NOTE:** This option is not available if a request is based on a GUI
Script template.

A post that runs in the foreground is used for requests that do not time
out the system based on the number of records to process.

**NOTE:** If this icon does not display, the Foreground Post check box
is disabled on the
<span style="font-style: italic;">[Parameters](Parameters.htm)</span>
page. Refer to [Display Posting Options on
Requests](../Config/Display_Posting_Options_on_Requests.htm) for more
information.

Background Post

Click to immediately post request data to a target ERP system in the
background.

The user credentials used to post data can be acquired using the methods
outlined in [Establish a Connection to a Target
System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm).

A request is posted in the background if there is a large amount of data
to process that may affect system performance or may time out a session.
Monitor posts that run in the background on the *[Request Role Finish
Monitor](Request_Role_Finish_Monitor.htm)* page.

**NOTE:** If this icon does not display, the Background Post check box
is disabled on the
<span style="font-style: italic;">[Parameters](Parameters.htm)</span>
page. Refer to [Display Posting Options on
Requests](../Config/Display_Posting_Options_on_Requests.htm) for more
information.

Post Later

Post Start Time

Displays the time the request begins posting to the target ERP system.
Refer to<span> </span>[Setting the Post Start
Time](../Use_Cases/Setting_the_Post_Start_Time.htm) for more
information.

Schedule Post

Click to add the request data to the background posting queue. The
request posting process begins at the Post Start Time.

The user credentials used to post data can be acquired using the methods
outlined in [Establish a Connection to a Target
System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm).

**NOTE:** When posting in dspCompose™ using the Schedule Post feature,
users must have permission to the Post Monitor group in Integrate to
successfully post.

**NOTE:** If this icon does not display, the Schedule Post check box is
disabled on the
<span style="font-style: italic;">[Parameters](Parameters.htm)</span>
page. Refer to [Display Posting Options on
Requests](../Config/Display_Posting_Options_on_Requests.htm) for more
information.
