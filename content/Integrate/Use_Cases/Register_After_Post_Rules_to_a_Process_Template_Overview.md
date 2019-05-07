+++
title = 'Register After Post Rules to a Process Template Overview'
solution = 'Platform'
+++

# Register After Post Rules to a Process Template Overview

Rules pull data from a target or source to refresh local data after it
has been changed or to manipulate the local data to prepare for the next
process template to execute.

When posting data to a target system, a Template Administrator can
register an After Post Rule to a process template. The rule runs after
the process template executes successfully and before the next process
template begins processing (if posting with a multi-template process).

The following can be registered as an After Post Rule:

  - <span style="font-weight: bold;">Business Rule</span> - A stored
    procedure that may take a variable of @PostingID GUID. If this
    property exists, then the posting ID of the posting passes to the
    procedure. When a business rule After Post rule is encountered,
    Integrate runs the rule and waits for it to complete before running
    the next rule. Refer to [Register a Stored Procedure as an After
    Post Rule](Register_a_Stored_Procedure_as_an_After_Post_Rule.htm)
    for more information.
  - <span style="font-weight: bold;">Collect Download</span> - A Collect
    rule that downloads a Collect source - target - table registration.
    Refer to [Register a Collect Download as an After Post
    Rule](Register_a_Collect_Download_as_an_After_Post_Rule.htm) for
    more information.
  - <span style="font-weight: bold;">Status View</span> - A view used to
    communicate the status of the posting to the user. The view status
    is "pass" when there are no records in the view for the PostingID.
    The view status is "fail" if the view contains at least one record
    of data for the PostingID. If the status is "fail" then that status
    is written as the status for the posting of that template. Refer to
    [Register a Status View as an After Post
    Rule](Register_a_Status_View_as_an_After_Post_Rule.htm) for more
    information.

<span style="font-weight: bold;">NOTE</span>: It is possible to register
a Business Rule as an After Post Rule to update Collect Where clause
settings for the individual posting ID as well as to write data to
tables that can be used by the Status View. By using the three types of
After Post Rules together in a process template, an advanced user can
configure a complex posting and download scenario.

When a process template with an After Post Rule registered posts
successfully, the data is passed to the next dependent template process
as an input parameter. For example, a user can configure a process with
multiple templates that creates a material and extends the material to
different plants. The first template creates a material number and
contains a stored procedure After Post Rule that captures the material
number and uses it as an input parameter to next template. The next
template uses the material number parameter created by the first
template to extend the material number to different plants.

<span style="font-weight: bold;">NOTE</span>: After Post Rules do not
run when the process causes a validation to fail. The rules do run if
there are posting errors (i.e., a record does not post to the target
system because there are errors in the data).

<span style="font-weight: bold;">NOTE</span>: The execution order for
both process templates and After Post Rules is determined by the
priority. Set the priority for process templates on the
<span style="font-style: italic;">[Process
Templates](../Page_Desc/Process_Templates_H.htm)</span> page. Set the
priority for After Post Rules on
the[<span style="font-style: italic;">Process Templates: After Post
Rules</span>](../../../Master_Data_Mgmt/dspConduct/Page_Desc/Process_Templates_After_Post_Rules_H.htm)
page.

<span style="font-weight: bold;">NOTE</span>: Each process template can
have one or many After Post Rules registered.  

<span style="font-weight: bold;">NOTE</span>: The process template must
be inactive to add After Post Rules.
