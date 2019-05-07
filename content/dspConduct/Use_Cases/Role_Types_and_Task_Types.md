+++
title = 'Role Types and Task Types'
solution = 'Master Data Management'
+++

# Role Types and Task Types

Each role is assigned a role type to define how role data within a
request can be manipulated. Role types are:

  - <span style="font-weight: bold;">Application</span> – Gathers,
    enters or makes changes to data using pages in the Content WebApp
    for preparation to send to the system(s) of record.
  - <span style="font-weight: bold;">Display</span> – Views data but is
    unable to make changes. Users assigned to a role with a Display role
    type are not active participants in the process.
  - <span style="font-weight: bold;">Review</span> – Evaluates and
    reviews data, either approving or rejecting all changes made within
    the execution of a request. Data can be viewed but not modified. A
    role with this role type can also review everything within the tasks
    of their dependent Application roles within a scenario. Refer to
    [Review a Request Overview](Review_a_Request_Overview.htm) for more
    information.
  - <span style="font-weight: bold;">Post</span> – Posts data to a
    target system(s) after the Application and Review roles have been
    completed. Refer to  [Post a Request](Post_a_Request.htm) for more
    information.
  - <span style="font-weight: bold;">ManualPost</span> – Performs work
    outside of dspConduct™ by using a custom posting process or
    performing a physical task. Refer to [Use Manual
    Post](Post_a_Request.htm#Use_Manual_Post_) for more information.

A task type is assigned to each task to control which tasks can be
registered to roles. A task type is not a security parameter, meaning it
cannot be used to limit security to a page.

<span style="font-weight: bold;">NOTE</span>: Any Task pages that are of
type Application must be registered on the
<span style="font-style: italic;">[dspConduct™
Task](../Page_Desc/dspConduct_Task_H.htm)</span> page. dspConduct™ does
not create task pages with an Application type. These pages are created
in the Content WebApp.

Task types are:

  - <span style="font-weight: bold;">Application</span> – Tasks that
    gather, enter or make changes to data using pages in the Content
    WebApp for preparation to send to the system(s) of record.
  - <span style="font-weight: bold;">Display</span> – Tasks that can be
    viewed but cannot be changed.
  - <span style="font-weight: bold;">Review</span> – Tasks that evaluate
    and review data, helping the Review role decide to approve or reject
    data changes or additions made within the execution of a request.
  - <span style="font-weight: bold;">Post</span> – Tasks that post data
    to a target system after the application and review roles have been
    completed.

Task types are used in conjunction with role types. When adding a task
to a role, the tasks being assigned to a role are validated based on the
task and role types.

Tasks with Application or Display types can be added to a role with a
role type of Application or Display.

Tasks with a task type of Application, Display or Review can be added to
a role with a role type of Review.

Tasks with a task type of Application, Display or Post can be added to a
role with a role type of Post.
