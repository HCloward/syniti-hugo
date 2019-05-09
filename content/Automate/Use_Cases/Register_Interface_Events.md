+++
title = 'Register Interface Events'
solution = 'Platform'
+++

# Register Interface Events

Once the basic interface has been established, an Interface Designer can
add interface events to interfaces using the *[Interface
Events](../Page_Desc/Interface_Events)* page.

Supported event types are:

  - [Stored Procedure](Register_Stored_Procedure_Events)
  - [WebApp](Register_WebApp_Events)
  - [Workflow](Register_Workflow_Events)

Events run sequentially based on their priority; those with the lowest
priority run first. There are 2 cases where events run simultaneously:

1.  If an event submits a job to the job queue (i.e., runs in the
    background), the next event immediately starts running as soon as
    the job from the previous event has been added to the job queue.
2.  If there is not a WAIT parameter passed to an interface CommandExec
    event, the next event is immediately started once the CommandExec
    has started running.

Events that run simultaneously, i.e., if an event submits a job to the
background, the next event does not wait for the previous job to finish.
To configure events to run sequentially, refer to [Run Interface Events
Sequentially](Run_Interface_Events_Sequentially).

To help with performance, it is recommended to have more interfaces with
fewer events each than to have several stored procedures registered to
one interface.
