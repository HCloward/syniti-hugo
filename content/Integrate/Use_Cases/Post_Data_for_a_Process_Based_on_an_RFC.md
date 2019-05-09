+++
title = 'Post Data for a Process Based on an RFC'
solution = 'Platform'
+++

# Post Data for a Process Based on an RFC

<span id="Post Data using an RFC Steps" class="popUpLink">\>Review the
steps in the process. </span>

A process post allows the posting of a process through Integrate.
Integrate automatically creates a process post for a process template
with the name **Auto Generated Post For \[Process Name\].** A user can
also configure multiple process posts for a single process with each
process post record having different post settings.

To post data, edit the process post Integrate generated (or add a
process post), post the data, and review the messages regarding posting
status.

**NOTE**: A process must be active to add or edit a process post.

<span style="font-weight: bold;">NOTE</span>: Data can be posted using a
multiple template process. Refer to [Post a Process with Multiple
Templates](Post_a_Process_with_Multiple_Templates) for more
information.

<span style="font-weight: bold;">NOTE</span>: When posting data to a
target system, a Template Administrator can register an After Post Rule
to a process template. The rule runs after the process template executes
successfully and before the next process template begins processing (if
posting with a multi-template process). When a process template that has
an After Post Rule registered posts successfully, the data is passed to
the next dependent process template as an input parameter. Refer to
[Register After Post Rules to a Process
Template](Register_After_Post_Rules_to_a_Process_Template_Overview)
for more information.

To edit a process post and post data for a process:  

1.  Click the **Postings** icon on the *Process* page.

2.  Click **Edit** for a process post; the *Vertical* View displays. 
    
    *[View the field descriptions for the Process Post page’s Vertical
    View.](../Page_Desc/Process_Post_H#Process_Post_V_All_Tabs)*

3.  Enter a where clause to restrict the data set in **Where Clause**.
    
    **NOTE:**When posting a BDC, GUI, or BAPI/RFC template with more
    than one loop, the WHERE CLAUSE must apply to ALL views mapped to
    the loops.

4.  Click **Save**.

5.  Click **View Primary Loop Data** to verify the data for the first
    loop.
    
    **NOTE**: If a where clause was not entered, all records for the
    primary loop display.

6.  Navigate back to the *Vertical* View.

7.  Click **Advanced** tab.

8.  Select **StandardSAPPosting** from the **BDC Post Method** list box.
    
    **NOTE**: Process posts based on RFC templates use the
    **StandardSAPPosting** post method only.

9.  Enter a user name and password for SAP if needed.
    
    **NOTE**: Refer to [Establish a Connection to a Target
    System](../../Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview)
    for more information.

10. Click **Save**.

11. Click **Post** on the Page toolbar; a confirmation message displays.

12. Click **Ok**.
    
    **NOTE**: Integrate displays a message listing the number of
    successful records and failed records for the post.

13. Click **View Messages** on the Page toolbar when the post is
    complete.
    
    **NOTE**: Click **Delete Messages** button to remove all messages
    for the post record, if applicable. The Message table is not
    automatically cleared; it must be manually cleaned out.
    
    **NOTE**: If the posting is successful, each record displays with a
    message “The function call completed successfully’ returned from SAP
    in the **MESSAGE** column.
