+++
title = 'Post Data Using an SAP Data Services Job'
solution = 'Platform'
+++

# Post Data Using an SAP Data Services Job

A Template Administrator can post data to a target system using a
process post based on an SAP Data Services Job template. The SAP Data
Services Job template type uses a Data Services Job (consisting of a
Data Services Repository and a job name) when posting data.

For general information about SAP Data Services Job templates, refer to
[Post Data Using  an SAP Data Services Job
Overview](Post_Data_Using_an_SAP_Data_Services_Job_Overview).

Before performing this task, [create a
template,](Create_an_SAP_Data_Services_Job_template)[activate the
template](Activate_the_Template_DS_Job), [add the template to a
process](Add_the_Template_to_a_Process_DSJob) and [activate the
process](Activate_the_Process_DS_Job).

When a process is posted with an SAP Data Services Job template,
Integrate runs the  tx\*Int view mapped at the Process – Template – Loop
level applying the Where Clause from the process post. The Data Services
Job with Global Variables values (if applicable) from the tx\*Int view
runs for each record returned from the Where clause.

Integrate automatically creates a process post for a process template
with the name Auto Generated Post For \[Process Name\]. A user can also
configure multiple process posts for a single process with each process
post record having different post settings.

<span style="font-weight: bold;">NOTE</span>: A process must be active
to add or edit a process post.

<span style="font-weight: bold;">NOTE</span>: When posting data to a
target system, a Template Administrator can register an After Post rule
to a process template. The rule runs after the process template executes
successfully and before the next process template begins processing (if
posting with a multi-template process). When a process template that has
an After Post rule registered posts successfully, the data is passed to
the next dependent process template as an input parameter. Refer to
[Register After Post Rules to a Process
Template](Register_After_Post_Rules_to_a_Process_Template_Overview)
for more information.

To edit a process post and post data for a process in Integrate:  

1.  Click <span style="font-weight: bold;">Categories</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    a category.

3.  Click the <span style="font-weight: bold;">Postings</span> icon for
    a process.

4.  Click <span style="font-weight: bold;">Edit</span> for a process
    post; the <span style="font-style: italic;">Vertical</span> View
    displays.
    
    [View the field descriptions for the Process Post page’s Vertical
    View.](../Page_Desc/Process_Post_H#Process_Post_V_All_Tabs)

5.  Enter a where clause to restrict the data set in the
    <span style="font-weight: bold;">Where Clause</span> field.

6.  Click <span style="font-weight: bold;">Save</span>.

7.  Click <span style="font-weight: bold;">View Primary Loop Data</span>
    to verify the data for the first loop.
    
    <span style="font-weight: bold;">NOTE</span>: If a where clause was
    not entered, all records for the primary loop display.

8.  Navigate back to the
    <span style="font-style: italic;">Vertical</span> View.

9.  Click <span style="font-weight: bold;">Post</span> on the Page
    toolbar; a confirmation message displays.

10. Click <span style="font-weight: bold;">Ok</span>.
    
    <span style="font-weight: bold;">NOTE</span>: If a where clause was
    not entered, all records for the primary loop display. Integrate
    displays a message listing the number of successful records and
    failed records for the post.

11. Click <span style="font-weight: bold;">View Messages</span> on the
    Page toolbar when the post is complete.
    
    <span style="font-weight: bold;">NOTE</span>: Click the Delete
    Messages button to remove all messages for the post record, if
    applicable. The Message table is not automatically cleared; it must
    be manually cleaned out.
    
    <span style="font-weight: bold;">NOTE</span>: If the posting is
    successful, each record displays with a message “The function call
    completed successfully’ returned from SAP in the MESSAGE column.
