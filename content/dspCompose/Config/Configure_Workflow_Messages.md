# Configure Workflow Messages

Several workflow messages are delivered with dspCompose™ and can be
modified but not deleted. No workflow messages can be added.

dspCompose™ sends workflow messages when certain events occur, such as
when a request is ready for processing by the next role in the workflow,
when a request is reset or rejected, or when an email sent by an
External Data role fails validations.

Workflow messages can be set for multiple languages.

Refer to [Set up Workflow Messages](Set_up_Workflow_Messages.htm) for
more information.

**NOTE**: The address in the EMAIL FROM column for the EmailValidation
event and the ExternalData event are identical on the
<span style="font-style: italic;">Workflow Language Message</span>
page's <span style="font-style: italic;">Horizontal</span> View by
default. These addresses must be configured on site, and should contain
the same email address.

To modify a workflow message:

1.  Select **Configuration \> Workflow Message** on the *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Messages** for a **LANGUAGE
    ID<span style="font-weight: normal;">.</span>**

3.  Click **Edit** for an event to modify an existing message.
    
    [View the field descriptions for the Workflow Language Message
    page's Vertical View.](../Page_Desc/Workflow_Language_Message_H.htm)

4.  Enter the email subject line text in **SUBJECT
    <span style="font-weight: normal;">field</span>**.

5.  Enter text to display in the body of the workflow message in
    **MESSAGE <span style="font-weight: normal;">field</span>**.

6.  Enter a valid email address in **EMAIL FROM
    <span style="font-weight: normal;">field</span>**.
    
    **NOTE:** The EMAIL FROM value **must** be configured at the client
    site. The email address must contain an **@** sign and a period
    (**.**) to be considered valid.

7.  Click **Save**.
