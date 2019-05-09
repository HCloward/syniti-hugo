+++
title = 'Set Up Service Pages for SLAs'
solution = 'Master Data Management'
+++

# Set Up Service Pages for SLAs

The *Request SLA Notification* Service page determines which request
roles are late to be processed. The *Request SLA Notification Workflow*
and <span style="font-style: italic;">Request SLA Summary
Workflow</span> service pages views the records created by *Request SLA
Notification Service* page and sends the workflows necessary for those
late request roles.

An Administrator configures service pages.

If the client site requires workflow notifications, the *Request SLA
Notification* Service page and either the *Request SLA Notification
Workflow* or <span style="font-style: italic;">Request SLA Summary
Workflow Service </span>pages must execute.

The Request SLA Notification Workflow service page sends any messages
from LateNotify event, if the event is enabled on the *[Category
Workflow Language
Message](../Page_Desc/Category_Workflow_Language_Message_H) page.*

The Request SLA Summary Workflow service page sends any messages from
the LateSummary event if the event is enabled on the *[Category Workflow
Language
Message](../Page_Desc/Category_Workflow_Language_Message_H)*page.

**NOTE**: The LateSummary event sends a summary email that contains
links to requests that have late roles. The LateNotify event sends
individual emails for each late role. If both of these events are
enabled, a user receives both a summary email and individual emails for
each late role. It is recommended that either LateNotify event or
LateSummary event be activated but not both.

In order for SLAs notification to work properly, an Administrator must
set the *Request SLA Notification Service* page and the *Request SLA
Notification Workflow* Service or Request SLA Summary Workflow page **to
run consecutively**.
