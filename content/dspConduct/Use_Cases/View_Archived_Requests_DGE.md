+++
title = 'View Archived Requests'
solution = 'Master Data Management'
+++

# View Archived Requests

A user who belongs to dspConduct™ WebApp group ArchiveUser or PowerUser
can view archived request data, including roles, tasks, post processes
and finish download messages.

An Administrator adds users to WebApp groups. Archived request data does
not display for a user unless that user is assigned to one of these
WebApp groups.

Requests are archived when:

A request remains in a request status longer than the number of days set
on the <span style="font-style: italic;">[Category Request
Status](../Page_Desc/Category_Request_Status)</span> page

An event runs in the Content WebApp that archives the request

<span style="font-weight: bold;">NOTE</span>: A Designer must register
stored procedures to an event in the Content WebApp to manage the
archiving process. The process must archive Content Request-related
table data and also call dspConduct™ process to archive dspConduct™
Request-related table data.

Use the following pages, accessed for a request on the
<span style="font-style: italic;">[Archived
Request](../Page_Desc/Archived_Requests)</span> page, to view
details.

  - [Archived Request Roles](../Page_Desc/Archived_Request_Roles)
    page displays roles assigned to the archived request.
  - [Archived Request Role
    Task](../Page_Desc/Archived_Request_Role_Task) page displays the
    tasks assigned to a role for the selected archived request.
  - [Archived Request Role
    Log](../Page_Desc/Archived_Request_Role_Log) page displays log
    records that detail when Request/Request Role activities occurred,
    such as whether a request was ever reset or rejected, or the date a
    role was finished.
  - [Archived Request Post
    Process](../Page_Desc/Archived_Request_Post_Process) page
    displays the Integrate process(es) assigned to the archived request
    at the scenario level.
  - [Archived Request Post
    Message](../Page_Desc/Archived_Request_Post_Message) page
    displays the posting message returned for each record from the
    target system.
  - [Archived Finish Download
    Messages](../Page_Desc/Archived_Finish_Download_Messages)
    displays every action that took place during the Post role’s Final
    Finish download for the archived request.

<!-- end list -->

  - If an active request had SLA details, the
    <span style="font-style: italic;">[Archived Request Role
    SLA](../Page_Desc/Archived_Request_Role_SLA)</span> page
    displays the SLA details once the request is archived.
