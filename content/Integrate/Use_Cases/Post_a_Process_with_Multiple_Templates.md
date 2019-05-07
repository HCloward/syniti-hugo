+++
title = 'Post a Process with Multiple Templates'
solution = 'Platform'
+++

# Post a Process with Multiple Templates

A process can contain multiple templates of different template types.  A
multi-template process must use a **Post Execution Method** of
**Synchronous** (set on the *Process* page’s *Vertical* View on the
**Advanced** tab). BDC Script, GUI Script, and BAPI/RFC templates can
use the Synchronous Post Execution Method, so these are the only
template types that can be assigned to a multiple template process.

User Defined template types use the asynchronous post execution method,
and cannot be assigned to a multiple template process.

Multiple templates in a process can use transaction stringing during the
posting process. Refer to [Post Data Using Transaction
Stringing](Post_Data_Using_Transaction_Stringing.htm) for more
information.

<span style="font-weight: bold;">NOTE</span>: If a process based on a
GUI script is included in a process with multiple templates, that
process can only be posted in the background. Other posting methods are
not available. In this case, the Post icon does not display on the
<span style="font-style: italic;">Process Post</span> page’s
<span style="font-style: italic;">Vertical</span> View and the
Foreground Post icon does not display on the Posting tab of the
<span style="font-style: italic;">Process Post</span> page’s
<span style="font-style: italic;">Vertical</span> View.

<span style="font-weight: bold;">NOTE</span>: After Post Rules can be
added to run after a template in a multi-template process. These rules
return data that is used as an input parameter for the next template in
the process. Refer to [Register After Post Rules to a Process
Template](Register_After_Post_Rules_to_a_Process_Template_Overview.htm)
for more information.

To post data for a process with multiple templates:

1.  Add templates and activate them. Refer to [Create a Basic
    Template](Create_a_Basic_Template.htm) and the sections for adding
    each template type for more information.
    
    **NOTE**: The steps for template creation and activation for
    templates that will be assigned to a multiple template process are
    identical to those for a template that will be the single template
    in a process.

2.  Add a process, and add the templates to the process. Refer to [Add
    Templates to a Process](Add_Templates_to_a_Process.htm) for more
    information.
    
    **NOTE**: When adding a template, the priority set for each template
    determines the order the template is posted. Templates are processed
    in ascending priority order.

3.  Configure the process template loops for each template in the
    process.
    
      - Use the Auto Generate Database Objects feature to automatically
        add tables and views for the template. Refer to [Generate
        Database Objects
        Automatically](Generate_Database_Objects_Automatically.htm) for
        more information.
      - Each loop must be linked to the parent loop through a
        relationship. Refer to [View and Configure Relationships for a
        Process Based on a BDC Script
        Template](ViewandConfigureRelationshipsBDC.htm), [View and
        Configure Relationships for a Process Based on a GUI Script
        Template](VwConfigureRelshpsGUIe.htm), [View and Configure
        Relationships for a Process Based on a
        BAPI](ViewandConfigureFieldMappingsBAPI.htm), and [View and
        Configure Relationships for a Process Bases on an
        RFC](VwConfigureRshpsProcRFC.htm) for more information.

4.  Activate the process. Refer to the sections for adding each template
    type for more information.

5.  Configure the process post. Use the **BDC Post Method** of
    **StandardSAPPosting**. No other options are allowed for
    multi-template processes. Refer to [Posting
    Methods](Posting_Methods.htm), [Use a Process Post Record to Post to
    SAP for a Process Based on a BDC Script
    Template](Post_Data_for_a_Process_Based_on_a_BDC_Script_Template.htm),
    [Use a Process Post Record to Post to SAP for a Process Based on a
    GUI Script
    Template](Post_Data_for_a_Process_Based_on_a_GUI_Script_Template.htm),
    [Use a Process Post to Post Data for a Process Based on a
    BAPI](Post_Data_for_a_Process_Based_on_a_BAPI.htm) or [Use a Process
    Post to Post Data for a Process Based on an
    RFC](Post_Data_for_a_Process_Based_on_an_RFC.htm) for more
    information.

6.  Set up testing scenarios for a process with multiple templates on
    the **Advanced** tab on the *Process Post Vertical* View to restrict
    the number of templates that Integrate posts. Enter the priority of
    the first template to include in the debug process in the **Start
    Template Priority** field, and the priority of the last template in
    the **End Template Priority** field.
    
    **NOTE:** If using the **Create GUI Debug Script** option for a
    process with multiple templates that contains a GUI Script template,
    use the **Start Template Priority** and **End Template Priority**
    fields to restrict the posting to the GUI Script template only. For
    example, if a multi-template process contains a GUI Script template
    with a priority of 30, and the **Create GUI Debug Script** option is
    to be used, enter 30 in the **StartTemplate Priority** and **End
    Template Priority** fields on the **Advanced** tab of the *Process
    Post* page’s *Vertical* View. When posting the process, Integrate
    will only post the GUI Script template, and the GUI debug script can
    be used on the template. Refer to [Debug a GUI Script
    Posting](Debug_a_GUI_Script_Posting.htm) for more information.

7.  Post the data. If the posting fails, troubleshoot the errors using
    information on the *Messages* page or download the message file on
    the *Message File* page. Refer to [Tips and
    Troubleshooting](Tips_and_Troubleshooting_Integrate.htm) for more
    information.

8.  Resubmit the post after correcting any errors. Click **Reset** for
    the process post on the *Process Post* page’s *Vertical* View on the
    **Posting** tab, then post the data again. Refer to [Reset and
    Resubmit a Failed Post](Reset_and_Resubmit_a_Failed_Post.htm) for
    more information.

**NOTE**: After resetting a post it can be submitted again regardless of
its status prior to the reset, and regardless of the reason for the
failure.
