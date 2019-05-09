+++
title = 'Post Data with a Custom Template'
solution = 'Platform'
+++

# Post Data with a Custom Template

A Custom template allows a user to create a mechanism for posting to any
system.

<span style="font-family: Arial, sans-serif;">A user must create all of
the associated files and code to support the Custom template.</span>

After a Custom template has been [added to a
process](Add_the_Custom_Template_to_a_Process) and the [process has
been activated](Activate_the_Process_Custom_Template), the process
can be posted.

Integrate automatically creates a process post for a process template
with the name **Auto Generated Post For \[Process Name\]**<span>when the
process is saved.</span>

**NOTE**: Data can be posted using a multiple template process. Refer to
[Post a Process with Multiple
Templates](Post_a_Process_with_Multiple_Templates) for more
information.

**NOTE**: When posting data to a target system, a Template Administrator
can register an After Post Rule to a process template. The rule runs
after the process template executes successfully and before the next
process template begins processing (if posting with a multi-template
process). When a process template that has an After Post Rule registered
posts successfully, the data is passed to the next dependent process
template as an input parameter. Refer to [Register After Post Rules to a
Process
Template](Register_After_Post_Rules_to_a_Process_Template_Overview)
for more information.

<span style="font-weight: bold;">NOTE</span>: A process must be active
to add or edit a process post.

To post data using a Custom template:

1.  Click **Categories** on *Navigation pane*.

2.  Click the **Processes** icon for a category.

3.  Click the **Postings** icon for a process.
    
    <span style="font-weight: bold;">NOTE</span>: A process must be
    active for the **Postings** icon to be available.

4.  Click the <span style="font-weight: bold;">Connections</span> icon
    for a process post to view the Connection ID.
    
    <span style="font-weight: bold;">NOTE</span>: A process post record,
    with a blank Connection ID, is required for the post process to
    work.

5.  Return to the <span style="font-style: italic;">[Process
    Post](../Page_Desc/Process_Post_H)</span> page.

6.  Click the **Post** icon; a confirmation message displays.

7.  Click **OK**.
    
    <span style="font-weight: bold;">NOTE</span>: Once the post is
    complete, Integrate displays a message detailing how many records
    successfully posted and how many records failed.

8.  Click **View Messages** icon when the post is complete.

**NOTE**: Integrate displays a record for each record in the dataset,
with a message returned from the system. Message text must be provided
by the user and included in the custom code.

<span style="font-weight: bold;">NOTE</span>: A developer can log
posting messages to assist with troubleshooting and add them to
Integrate’s ttDebugLog table as part of the custom template
implementation.
