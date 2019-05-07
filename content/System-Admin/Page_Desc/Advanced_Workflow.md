+++
title = 'Advanced Workflow'
solution = 'Platform'
+++

# Advanced Workflow

<div class="use" data-xmlns="">

Use this page to [Configure Workflow
Fields](../Use_Cases/Configure_Workflow_Fields.htm).

</div>

To configure the workflow fields:

1.  Select **Admin \> WebApps** in the *Navigation* pane.
2.  Click the **Pages** icon for a WEB APP NAME.
3.  Click the **Events** icon for a DESCRIPTION.
4.  Click the **Business Rules** icon for an EVENT.
5.  Click **Vertical View** for a business rule with a PROCEDURE TYPE of
    Workflow.
6.  Click **Workflow Fields**.

Field

Description

Event

Displays the event that will cause the workflow to be executed. 

Alternate View

Displays the view used by the workflow.

General Fields

Message Type ID Field

Displays an option that overrides the static defined Message Type on the
vertical of the Business Rules page. A workflow can either sent
notifications to users and/or emails. To use, specify a MessageTypeID
defined on the Admin -\> Configuration -\> Messages Types page.

From

Displays the column name from the Alternate View that contains the
sender’s email address.

To

Displays the column name from the Alternate View that contains the email
address(es) or userID(s) of the TO recipients.

CC

Displays the column name from the Alternate View that contains the email
address(es) or userID(s) of the CC recipients. If the workflow contains
a link, each recipient receives a separate notification or email. 

BCC

Displays the column name from the Alternate View that contains the email
address(es) or userID(s) of the BCC recipients. If the workflow contains
a link, each recipient receives a separate notification or email. 

Subject

Displays the column name from the Alternate View that contains the
subject of the email.

Body

Displays the column name from the Alternate View that contains the
content of the email.

Email Fields

Email Attachment

Displays the column name from the Alternate View where the paths to the
file attachment(s) are specified. 

Message Fields

Group

This option allows several messages sent to a user to be grouped
together. If the user is off online when the message is sent, after
logging in only the most recent message in the group will be displayed
and/or considered unread.
