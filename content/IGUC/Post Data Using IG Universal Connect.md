+++
title = 'Post Data Using IG Universal Connect'
solution = 'Platform'
+++

# Post Data Using IG Universal Connect

A Template Administrator can post data to a Target system using a
Process post based on an IG Universal Connect Template, which uses a
Boomi Process when posting data.

When a process is posted with an IG Universal Connect Template,
Integrate runs the  tx\*Int view mapped at the Process – Template – Loop
level applying the Where Clause from the process post. The IG Universal
Connect with parameter values (if applicable) from the tx\*Int view runs
for each record returned from the Where clause.

Integrate automatically creates a Process post for a Process template
with the name Auto Generated Post For \[Process Name\]. A user can also
configure multiple Process posts for a single Process with each Process
post record having different post settings.

<span style="font-weight: bold;">NOTE</span>: A Process must be active
to add or edit a process post.

<span style="font-weight: bold;">NOTE</span>: When posting data to a
target system, a Template Administrator can register an After Post rule
to a process template. The rule runs after the Process template executes
successfully and before the next Process template begins processing (if
posting with a multi-template Process). When a process template that has
an After Post rule registered posts successfully, the data is passed to
the next dependent Process template as an input parameter. Refer to
[Register After Post Rules to a Process
Template](../Integrate/Use_Cases/Register_After_Post_Rules_to_a_Process_Template_Overview.htm)
for more information.

**NOTE**: When Integrate executes a Boomi process, it passes in the
LinkID for the execution, which is used to return a status to the DSP®
once the execution is complete. **The user must add any additional
parameters required for the process.**

To edit a Process post and post data for a Process in Integrate:  

1.  Click <span style="font-weight: bold;">Categories</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Processes</span> icon for
    a category.

3.  Click the <span style="font-weight: bold;">Postings</span> icon for
    a Process.

4.  Click <span style="font-weight: bold;">Edit</span> for a process
    post; the <span style="font-style: italic;">Vertical</span> View
    displays.
    
    [View the field descriptions for the Process Post page’s Vertical
    View.](../Integrate/Page_Desc/Process_Post_H.htm#Process_Post_V_All_Tabs)

5.  Enter a Where Clause to restrict the data set in the
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
    
    <span style="font-weight: bold;">NOTE</span>: If a Where Clause was
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
    completed successfully’ returned in the MESSAGE column.
    
    **NOTE**: If the Process fails, access the Boomi AtomSsphere Process
    Reporting area for details. Locate the failed posted details using
    the execution ID which displays in the failed message in the DSP®.
