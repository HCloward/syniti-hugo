+++
title = 'Post Request Data to a Target ERP System'
solution = 'Data Quality'
+++

# Post Request Data to a Target ERP System

Once all roles have been approved by the user assigned to the Review
role, the request data is ready to be posted. As a recommendation, if a
large number of records is to be posted, post request data during
non-peak work hours, for example, after 5:00 p.m.

**NOTE**: When the Review role user clicks the **Approve** icon for the
request, the user assigned to the Post role for the request receives an
email if the **SEND WORKFLOW** check box is checked for that user on the
*[User](../Page_Desc/User_H.htm)* page.

**NOTE**: If the request has Org Units assigned, dspCompose™ only sends
workflow emails to users who have Org Unit security for values on the
request.

The posting options available for a request are set on the
*[Parameters](../Page_Desc/Parameters.htm)* page on the **Posting and
File** tab. If a Template Administrator enables a check box on this
page, that posting option is available to users with the Post role on
the *[Request (Post)](../Page_Desc/Request_Post.htm)* page. If a
Template Administrator disables a check box on the *Parameters* page,
the posting option does not display on the *Request (Post)* page, and is
unavailable to the Post role when processing a request.

<span style="font-size: 11.0pt;font-family: Arial, sans-serif;">Posting
options determine whether a request is posted in the background
immediately, in the foreground immediately, or in the background at a
scheduled start time.</span>

**NOTE:** A request based on a GUI Script template cannot use the
Foreground post method.

A request is posted in the background if there is a large amount of data
to process that may affect system performance or may time out a session.
Monitor posts that run in the background on the *[Request Role Finish
Monitor](../Page_Desc/Request_Role_Finish_Monitor.htm)* page. Refer to
[Monitor Requests](Monitor_Requests.htm) for more information.

<span style="font-size: 11.0pt;">A post that runs in the foreground
processes immediately and</span> is used for requests that do not time
out the system based on the number of records to process.

Posting options include:

  - <span style="font-weight: bold;">Foreground Post</span> -
    Immediately posts data in the foreground using stored user
    credentials.  
    
    <span style="font-weight: bold;">NOTE:</span> This option is not
    available if the request uses a GUI Script template type.

  - **Background Post -** Posts a request in the background using stored
    credentials.

  - **Schedule Post -** Posts a request at a scheduled time using stored
    credentials.

Refer to [User Credentials in
dspCompose™](../Config/User_Credentials_in_dspCompose.htm) for more
information.

<span style="font-weight: bold;">NOTE:</span> When posting in
dspCompose™ using the Schedule Post feature, users must be assigned to
the Post Monitor group in Integrate to successfully post.

Refer to [Display Posting Options on
Requests](../Config/Display_Posting_Options_on_Requests.htm) for more
information.

To post request data in dspCompose™:

1.  Click the **Workflow** link in the email to be directed to the
    request.
    
    *Or*
    
    Select **Requests** in the *Navigation
    <span style="font-style: normal;">pane</span>.*

2.  Click **Roles** for a request.
    
    <span style="font-weight: bold;">NOTE:</span> The count on the
    **Roles** icon is the number of roles the current user can access,
    not the total number of roles for the request.

3.  Click **Request (Post)** for the **Post ROLE ID**.
    
    <span style="font-weight: bold;">NOTE:</span> If performing a
    Schedule Post, refer to [Setting the Post Start
    Time](Setting_the_Post_Start_Time.htm) for more information.

4.  Click the applicable post method icon; a confirmation message
    displays.
    
    <span style="font-weight: bold;">NOTE:</span> If the Foreground
    Post, Background Post or Post Later options do not display, check
    boxes for the corresponding posting methods are disabled on the
    <span style="font-size: 11.0pt;font-style: italic;">[Parameters](../Page_Desc/Parameters.htm)</span><span style="font-size: 11.0pt;">
    page. </span>Refer to [Display Posting Options on
    Requests](../Config/Display_Posting_Options_on_Requests.htm) for
    more information.
    
    <span style="font-weight: bold;">NOTE:</span> If posting via Post
    Start Time, refer
    to<span style="font-size: 11.0pt;color: #0000ff;">[Setting the Post
    Start Time](Setting_the_Post_Start_Time.htm)</span>for more
    information.

5.  Click **Yes**.
    
    <span style="font-weight: bold;">NOTE:</span> When posting in the
    foreground, a message displays indicating the success or failure of
    the post. dspCompose™ supports partial posts if some records error
    out. In the case of a partially successful post, the initial Data
    Entry role is reset and the failed records display on the data entry
    page for the initial Data Entry role. Refer to [Review Posting
    Messages](Review_Posting_Messages.htm) for more information.

6.  Return to the *[Request (Roles)](../Page_Desc/Request_Roles_H.htm)*
    page.

7.  Click **Finish** for the **Post** Role ID.

**NOTE**: When a user clicks the **Finish** button for a Post role, a
validation stored procedure runs to check for any post errors. If post
errors exist, a warning message displays. This feature ensures a request
is not finished with posting errors without the user’s permission.

**NOTE**: At the template-role level for a Post role, a Template
Administrator can register tables for download as a Finish process.
Additional configuration settings allow a Template Administrator to set
Collect rules to run on table data after the download is finished, and
to specify filter columns for both source and target data. Refer to
[Register Tables for Download as a Finish Process using
Collect](Register_Tables_to_Download_as_a_Finish_Process_Using_Collect.htm)
for more information.

<span style="font-weight: bold;">NOTE</span>:  If no tables have been
registered for download as a Finish process or no columns have been
configured for the tables for download, warning messages display. Refer
to [Register Tables for Download as a Finish Process using
Collect](Register_Tables_to_Download_as_a_Finish_Process_Using_Collect.htm)
for more information.

<span style="font-weight: bold;">NOTE</span>: A rule can be associated
with this template level event. Refer to [Register Rules to
Template-level Events](Register_Rules_to_Template%20level_Events.htm)
 for more information.
