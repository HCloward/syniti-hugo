+++
title = 'Post Data for a Process Based on a GUI Script Template'
solution = 'Platform'
+++

# Post Data for a Process Based on a GUI Script Template

<span id="Post Data using a GUI Script Steps" class="popUpLink">\>Review
the steps in the process. </span>

A process post allows the posting of a process through Integrate.
Integrate automatically creates a process post for a process template
with the name **Auto Generated Post For – \[Process Name\].** A user can
also configured multiple process posts for a single process with each
process post record having different post settings.

The posting of encrypted values happens automatically. When posting, if
Integrate sees data that has been encrypted by the Secure component of
the DSP®, it will decrypt the data before posting. The data remains
encrypted in the database as the decryption happens only during the
posting process.

**NOTE**: Posting with encrypted data adds time to the posting process.

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

**NOTE**: A process must be active to add or edit a process post.

To use a post process record to post data to SAP:

1.  Click **Categories** on *Navigation pane*.

2.  Click the **Processes** icon for a category.

3.  Click the **Postings** icon for a process.
    
    **NOTE**: A process must be active for the **Postings** icon to be
    available.

4.  Click **Edit** for a posting; the *Vertical View* displays. 
    
    *[View the field descriptions for the Process Post page’s Vertical
    View.](../Page_Desc/Process_Post_H#Process_Post_V_All_Tabs)*

5.  Enter a Where clause to limit the data set in the **Where Clause**
    field.
    
    **NOTE:** If a Where Clause is not specified, Integrate uses an
    empty string. ***When posting a BDC, GUI, or BAPI/RFC template with
    more than one loop, the WHERE CLAUSE must apply to ALL views mapped
    to the loops*.**

6.  Click **Save**.

7.  Click **View Primary Loop Data** to verify that the where clause is
    correct.

8.  Navigate back to the *Process Post* page’s *Vertical* View.

9.  Click **Advanced** tab.

10. Select <span style="font-weight: bold;">StandardSAPPosting</span>
    from the <span style="font-weight: bold;">BDC Post Method</span>
    list box.
    
    **NOTE:** If a selection is not made, Integrate uses **Standard SAP
    Posting**. This is the only allowable post method for a template
    process based on a GUI script template.

11. Click **Create GUI Debug Script** check box, if applicable.
    
    **NOTE:** If **Create GUI Debug Script** is enabled, Integrate
    creates a copy of the actual GUI script run against SAP and writes
    it to the Message table along with the results of the post. This
    script can be downloaded from the *Messages* page and can be run in
    the SAP GUI to debug a GUI script posting. Refer to [Debug a GUI
    Script Posting](Debug_a_GUI_Script_Posting) for detailed
    information on how to run the debug script in the SAP GUI.
    
    **NOTE:** If using the **Create GUI Debug Script** option for a
    process with multiple templates that contain a GUI Script template,
    use the **Start Template Priority** and **End Template Priority**
    fields to restrict the posting to the GUI Script template only.
    Refer to [Debug a GUI Script
    Posting](Debug_a_GUI_Script_Posting) and Post a Process with
    Multiple Templates for more information.
    
    **NOTE:** Refer to [BDC Post Methods and Settings on the Advanced
    tab](../Page_Desc/BDCPostMethodsSettingsAdvTab) for more
    information about additional options on this tab.

12. Click <span style="font-weight: bold;">Create GUI Debug
    Script</span> to generate the script without uploading it, if
    necessary.
    
    <span style="font-weight: bold;">NOTE</span>: The script can then be
    reviewed prior to upload to ensure it was created properly.

13. Click <span style="font-weight: bold;">Download Full GUI Debug
    Script</span> to view the script.
    
    <span style="font-weight: bold;">NOTE</span>: Refer to [Debug a GUI
    Script Posting](Debug_a_GUI_Script_Posting) for more
    information.

14. Click **Post** on the Page toolbar; a confirmation message displays.
    
    **NOTE**: A process based on a GUI script can only be posted in the
    background. Other posting methods are not available. In this case,
    the Post icon does not display on the
    <span style="font-style: italic;">Process Post</span> page’s
    <span style="font-style: italic;">Vertical</span> View and the
    Foreground Post icon does not display on the Posting tab of the
    <span style="font-weight: normal; font-style: italic;">Process
    Post</span> page’s <span style="font-style: italic;">Vertical</span>
    View. If such a process is included in a process with multiple
    templates, that process can only be posted in the background as
    well. Refer to [Post a Process with Multiple
    Templates](Post_a_Process_with_Multiple_Templates) for more
    information.

15. Click **Ok**.
    
    **NOTE**: Once the post is complete, Integrate displays a message
    detailing how many records successfully posted, and how many records
    failed.

16. Click **View Messages** on the Page toolbar when the post is
    complete.
    
    **NOTE**: Integrate displays a record for each record in the
    dataset, with a message returned from SAP.

17. If the post was unsuccessful, click the **Debug** icon for each
    message for additional information to debug the posting as well as
    to determine the exact steps being performed in SAP. Refer to [Debug
    a GUI Script Posting](Debug_a_GUI_Script_Posting) for more
    information.
