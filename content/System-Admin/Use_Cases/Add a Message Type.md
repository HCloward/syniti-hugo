+++
title = 'Add a Message Type'
solution = 'Platform'
+++

# Add a Message Type

Message types allow users to configure how messages display in the DSP®,
setting the text, background color and images that display. Message
types also have a number of configuration settings that relate to how
the message behaves.

The DSP is delivered with message types that should not be updated. A
user can create custom message types to use for custom WebApps.

A user can add a message type by clicking the **Copy** icon in the Page
toolbar on the *Message Types* page and using the copy as the basis for
a new message type.

To add a message type:

1.  Select **Admin \> Configuration \> Setup \> Message Types**.

2.  Click **Add**.
    
    [View the field descriptions for the Message Types
    page](../Page_Desc/Message%20Types.htm)

3.  Enter a name in the **MESSAGE TYPE NAME** field.
    
    **NOTE**: Name the message so that developers and users can
    ascertain the scope of the message type and the application it runs
    in (for example, Cransoft.Event.Error).

4.  Enter the text that displays at the top of the message in the
    **TITLE** field.

5.  Select the name of the image that displays on the message from the
    **IMAGE ID** list box.
    
    **NOTE**: Images are added on the
    *[Images](../Page_Desc/Images%20H.htm)* page. Refer to [Add an Image
    to the DSP](Add%20an%20Image%20to%20the%20DSP.htm) for more
    information.

6.  Select the background color for the message from the **COLOR ID**
    list box.

7.  Enter a description of the message type, such as Notification, in
    the **DESCRIPTION** field.

8.  Click **Save**; the *Vertical* View displays.

9.  Enter a value in the **Retention Days** field, or retain the default
    value.
    
    **NOTE**: This field sets the number of days a message with this
    message type is stored in the database.

10. Enter a value in the **MESSAGE EXPANSION THRESHOLD** field, or
    retain the recommended default value.
    
    **NOTE**: This field sets a character limit for message details. If
    the character limit is exceeded, a generic message displays. The
    user must click a link to view the details in a separate pane.

11. Check the **Require Action** check box if the user must close the
    message by clicking it.
    
    **NOTE**: If unchecked, the message fades after a few seconds.

12. Check the **Archive** check box to retain an archive of the message
    which can be viewed by clicking the Messages tab on the Quick Panel.

13. Check the **Online Alert Only** check box, if needed.
    
    **NOTE**: If checked, if the message is sent when a user is not
    logged in, it will not display in the DSP when the user logs in. The
    user must click the Messages tab in the Quick Panel to view the
    message. If unchecked, the message displays as soon as the user logs
    in.

14. Click the **Read On Alert** check box to not increment the unread
    message counter displayed on the Messages tab on the Quick Panel. If
    unchecked, the number is always incremented.

15. Click **Save**.

**NOTE**: If the message type is to be used with a workflow business
rule, configure these additional options.

Select an option in the **Workflow Send Message** list box to indicate
how the DSP displays messages using this message type. Options are:

  - **Always send**

  - **Never send**

  - **Send only when user is offline**
    
    **NOTE**: If the user is online, the message/email isn't sent. It
    does not display in the DSP, and does not display on the Messages
    tab in the Quick Panel.

  - **Send only when user is online**

Select an option in the **Workflow Send Email** list box to indicate how
the DSP sends email when a message displays using this message type.
Options are:

  - **Always send**

  - **Never send**

  - **Send only when user is offline**
    
    **NOTE**: If the user is online, the email isn't sent.

  - **Send only when user is online**
