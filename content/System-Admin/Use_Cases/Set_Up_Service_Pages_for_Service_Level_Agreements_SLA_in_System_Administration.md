+++
title = ''
solution = 'Platform'
+++

## Set Up Service Pages for Service Level Agreements (SLA) in System Administration

For dspConduct™, the *Request SLA Notification* Service page determines
which request roles are late to be processed. The *Request SLA
Notification Workflow* and <span style="font-style: italic;">Request SLA
Summary Workflow</span> service pages views the records created by
*Request SLA Notification Service* page and sends the workflows
necessary for those late request roles.

If the client site requires workflow notifications, the *Request SLA
Notification* Service page and either the *Request SLA Notification
Workflow* or <span style="font-style: italic;">Request SLA Summary
Workflow Service </span>pages must execute.

The Request SLA Notification Workflow service page sends any messages
from LateNotify event, if the event is enabled on the *[Category
Workflow Language
Message](../../../Master_Data_Mgmt/dspConduct/Page_Desc/Category_Workflow_Language_Message_H.htm)
page.*

The Request SLA Summary Workflow service page sends any messages from
the LateSummary event if the event is enabled on tthe *[Category
Workflow Language
Message](../../../Master_Data_Mgmt/dspConduct/Page_Desc/Category_Workflow_Language_Message_H.htm)*page.**<span style="background: whitesmoke;">NOTE:</span>**
The LateSummary event sends a summary email that contains links to
requests that have late roles. The LateNotify event sends individual
emails for each late role. If both of these events are enabled, a user
receives both a summary email and individual emails for each late role.
It is recommended that either LateNotify event or LateSummary event be
activated but not both.

In order for SLAs notification to work properly, the *Request SLA
Notification Service* page and the *Request SLA Notification Workflow*
Service or Request SLA Summary Workflow page **must be set to run
consecutively**. For the *Request SLA Notification Service* page, the
Next Service Date must be set to run at a certain time (perhaps when the
system is less busy). The Next Service Date for Request SLA Notification
Workflow or <span style="font-style: italic;">Request SLA Summary
Workflow</span><span> </span> page must be set to run at a time later
than the Next Service Date set in the *Request SLA Notification* Service
page. The suggested interval between running the two Service pages is at
least 10 minutes.

Refer to [Configure Service Pages](Configure_Service_Pages.htm) for more
information about working with Service pages.
