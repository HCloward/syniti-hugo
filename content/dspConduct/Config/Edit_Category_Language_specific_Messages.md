# Edit Category Language-specific Messages

By default, dspConduct™ sends workflow messages to users who have access
to a request when a request is created, canceled, deleted, finished,
rejected or reset. dspConduct™ is installed with default workflow
messages in English and the processing to send these messages. Default
messages are used as the starting point for Category Language-specific
messages.

A Designer can modify the Subject, Message, and Email From to fit a
specific language, or can update the Default message information for
English language messages.

<span style="font-weight: bold;">NOTE</span>: The Email From address for
workflow messages should be supplied by the client and added to
messages, though this is not required.

<span style="font-weight: bold;">NOTE</span>: A Designer can add custom
workflow messages at the category level. However, the Content WebApp
must provide all code to process these messages.

<span style="font-weight: bold;">NOTE</span>: If a workflow language
message must not be sent or must be replaced with a custom message, the
ENABLED check box on the <span style="font-style: italic;">[Category
Workflow Language
Message](../Page_Desc/Category_Workflow_Language_Message_H.htm)</span>
page must be disabled.

On the <span style="font-style: italic;">[Category Workflow Language
Message](../Page_Desc/Category_Workflow_Language_Message_H.htm)</span>
page, a record for each of the Workflow Message Default Events displays.

Refer to [Configure Workflow Messages
Overview](Configure_Workflow_Messages_Overview.htm) for general
information.

All \#variable\# content is substituted with the actual value of the
variable when the workflow is processed.  In the Message body,
\#BusinessProcessName\# and \#ScenarioName\# may be added after the Role
information.  For example, to include Business Process and Scenario
values as part of the Workflow body, edit the message and change the
body from:

Role: \#RoleName\#

  to:

Role: \#RoleName\#

Business Process: \#BusinessProcessName\#

Scenario: \#ScenarioName\#

Messaging can be disabled for a role if notifications are sent too
frequently or if notifications are not needed. Refer to [Enable or
Disable Messages for a
Role](../Use_Cases/Enable_or_Disable_Messages_for_a_Role.htm) for more
information.

To edit a language-specific workflow message:

1.  Select <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Vertical View</span> for a
    category.

3.  Click the <span style="font-weight: bold;">Workflow Messages</span>
    icon.

4.  Click Messages for a <span style="font-weight: bold;">LANGUAGE
    ID</span>.
    
    **NOTE**: The languages that display in the LANGUAGE ID column are
    defined as active in the platform.

5.  Click <span style="font-weight: bold;">Edit</span> for the Event
    with the message to edit.
    
    [View the field descriptions for the Category Workflow Language
    Message
    page.](../Page_Desc/Category_Workflow_Language_Message_H.htm)

6.  Enter the email subject line text in
    <span style="font-weight: bold;">SUBJECT</span> field.
    
    **NOTE**: The subject line can contain a value preceded and followed
    by \# is a dynamic substitution value for replacement at run time.

7.  Enter text to display in the body of the workflow message in
    <span style="font-weight: bold;">MESSAGE</span> field.
    
    **NOTE:** The body of the email can contain a value preceded and
    followed by \# is a dynamic substitution value for replacement at
    run time.

8.  Enter a valid email address in
    <span style="font-weight: bold;">EMAIL FROM</span> field.
    
    **NOTE:** The EMAIL FROM default value should be changed at the
    client site to a value specific for the client, though this is not
    required. The email address must contain an @ sign and a period (.)
    to be considered valid.

9.  Click the <span style="font-weight: bold;">ENABLED</span> check box
    to disable it if the workflow language message must not be sent to
    users in the category or if a custom message must be used.
    
    **NOTE**: The check box is selected by default for all default
    events with the exception of the LateNotify event.
    
    **NOTE:** The LateSummary Event sends a summary email that contains
    links to Requests that have late roles. The LateNotify event sends
    individual emails for each late role. If both of these events are
    enabled, a user receives both a summary email and individual emails
    for each late Role. It is recommended that either LateNotify Event
    or LateSummary Event be activated but not both. Refer to [Set up SLA
    Notifications in dspConduct™](Set_Up_SLA_Notifications.htm) for more
    information on SLAs, which determine when a request is late.
    
    **NOTE**: To enable or disable multiple messages, use the CTRL or
    Shift key to select them, then click Enable or Disable in the Page
    toolbar.

10. Click <span style="font-weight: bold;">Save</span>.
