+++
title = 'Post Data for a Process Based on a BDC Script Template'
solution = 'Platform'
+++

# Post Data for a Process Based on a BDC Script Template

<span id="Post Data using a BDC Script Steps" class="popUpLink">\>Review
the steps in the process. </span>

A process post allows the posting of a process through Integrate.
Integrate automatically creates a process post for a process template
with the name **Auto Generated Post For \[Process Name\].** A user can
also configure multiple process posts for a single process with each
process post record having different post settings.

<span class="Body">The posting of encrypted values happens
automatically. When posting, if Integrate sees data that has been
encrypted by</span> the Secure component of the DSP®, it will decrypt
the data before posting. The data remains encrypted in the database as
the decryption happens only during the posting process.

**NOTE**: Posting with encrypted data adds time to the posting process.

<span style="font-weight: bold;">NOTE</span>: Data can be posted using a
multiple template process. Refer to [Post a Process with Multiple
Templates](Post_a_Process_with_Multiple_Templates.htm) for more
information.

<span style="font-weight: bold;">NOTE</span>: When posting data to a
target system, a Template Administrator can register an After Post Rule
to a process template. The rule runs after the process template executes
successfully and before the next process template begins processing (if
posting with a multi-template process). When a process template that has
an After Post Rule registered posts successfully, the data is passed to
the next dependent process template as an input parameter. Refer to
[Register After Post Rules to a Process
Template](Register_After_Post_Rules_to_a_Process_Template_Overview.htm)
for more information.

**NOTE**: A process must be active to add or edit a process post.

To use a post process record to post data to SAP:

1.  Click **Categories** on *Navigation pane*.

2.  Click the **Processes** icon for a category.

3.  Click the **Postings** icon for a process.
    
    **NOTE**: A process must be active for the **Postings** icon to be
    available.

4.  Click **Edit** for a posting; the *Vertical View* displays. 
    
    *[View the field descriptions for the Process Post page’s Vertical
    View.](../Page_Desc/Process_Post_H.htm#Process_Post_V_All_Tabs)*

5.  Enter a Where clause to limit the data set in the **Where Clause**
    field.
    
    **NOTE:** If a Where Clause is not specified, Integrate uses an
    empty string. The Where Clause syntax must be valid or Integrate
    will display an error. ***When posting a BDC, GUI, or BAPI/RFC
    template with more than one loop, the WHERE CLAUSE must apply to ALL
    views mapped to the loops*.**

6.  Click **Save**.

7.  Click **View Primary Loop Data** to verify that the where clause is
    correct.
    
    **NOTE**: The page displays the data from the first loop of the
    first template in the process post.

8.  Navigate back to the *Process Post* page’s *Vertical* View.

9.  Click **Advanced** tab.

10. Select from the **BDC Post Method** list box.
    
    **NOTE**: The settings configured on the **Advanced** tab depend on
    the **BDC Post Method** option selected and other factors. Refer to
    [*<span style="color: #0000ff;font-style: normal;">BDC Post Methods
    and Settings on the Advanced
    tab</span>*](../Page_Desc/BDCPostMethodsSettingsAdvTab.htm) for more
    information.

11. Click **Post** on the Page toolbar; a confirmation message displays.
    
    **NOTE**: Other posting methods are available.  Refer to
    *<span style="color: #0000ff;">[Posting
    Methods](Posting_Methods.htm)</span>* for more information.

12. Click **Ok**.
    
    **NOTE**: Once the post is complete, Integrate displays a message
    detailing how many records successfully posted and how many records
    failed.

13. Click **View Messages** on the Page toolbar when the post is
    complete.
    
    **NOTE**: Integrate displays a record for each record in the
    dataset, with a message returned from SAP.
    
    **NOTE**: If the process post is unsuccessful, make corrections and
    reset the post.

On the *Process Post* page’s *Vertical* View, on the **Posting** tab,
click **Reset**. Integrate resets the process post status regardless of
the reason for the posting failure or the current status of the post.

Refer to [Reset and Resubmit a Failed
Post](Reset_and_Resubmit_a_Failed_Post.htm) for additional information.
