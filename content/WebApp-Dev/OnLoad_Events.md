# OnLoad Events

OnLoad Events execute prior to the page displaying, allowing lazy data
population. Use OnLoad Events only when necessary because executing a
SQL Stored Procedure automatically increases page load time by at least
100 milliseconds, and page load time should never exceed a full second
for a good user experience.

Refer to [Create Events](Create_Events.htm) and [Event Design
Process](Event_Design_Process.htm) for general information.

Event Complexity

An event that runs every single page load should perform very little
work. If it is an event that is only meant to run once after a certain
scenario, then there should be a quick check to determine whether the
condition has been met. For example, a Metrics page may need to be
refreshed after data on a Task page has been modified. Instead of
recomputing metrics after every update on the Task page, toggle a dirty
flag OnValidate of a record on the Task page. Then, the OnLoad event on
the Metrics page can determine whether a recompilation is necessary or
not. Even though adding this flag to the OnValidate record on the Task
page adds complexity to the Task page, the load time of the Metrics page
is only affected when recomputing metrics.

Use complex events to reduce the scope of the processing based on, for
example, binding or key criteria, distributing that 500ms among several
other page navigations. Complex events can distribute the overhead based
on need.

Complex Events can also be used for:

  - Preparing for rendering static content (like an .aspx page)
  - Computing or recomputing metrics
  - Creating a temporary record (commonly used as form input)
