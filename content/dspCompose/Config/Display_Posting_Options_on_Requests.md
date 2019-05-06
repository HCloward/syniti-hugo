# Display Posting Options on Requests

The **Posting and File** tab on the
*[Parameters](../Page_Desc/Parameters.htm)* page has check boxes that
correspond to the posting options available in dspCompose™. If a
Template Administrator enables a check box on this page, that posting
option is available to users with the Post role on the *[Request
(Post)](../Page_Desc/Request_Post.htm)* page. If a Template
Administrator disables a check box on the *Parameters* page, the posting
option does not display on the *Request (Post)* page and is unavailable
to the Post role when submitting a request.

Posting options determine whether a request is posted in the background
immediately, in the foreground immediately, or in the background at a
scheduled start
time.

**<span style="font-size: 11.0pt;font-family: Arial, sans-serif;">NOTE</span>**:
A request based on a GUI Script template cannot use the Foreground post
method.

A request is posted in the background if there is a large amount of data
to process that may affect system performance or may time out a session.
Monitor posts that run in the background on the *[Request Role Finish
Monitor](../Page_Desc/Request_Role_Finish_Monitor.htm)* page.

<span style="font-size: 11.0pt;font-family: Arial, sans-serif;">A post
that runs in the foreground processes immediately and is appropriate for
requests that are not so large as to time out the system.</span>

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
dspCompose](User_Credentials_in_dspCompose.htm) for more information.

<span style="font-weight: bold;">NOTE</span>: When posting in dspCompose
using the Schedule Post feature, users must have permission to the Post
Monitor group in Integrate to successfully post.
