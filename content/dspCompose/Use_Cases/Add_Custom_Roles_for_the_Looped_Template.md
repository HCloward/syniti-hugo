+++
title = 'Add Custom Roles for the Looped Template'
solution = 'Data Quality'
+++

# Add Custom Roles for the Looped Template

Before performing this task:

1.  Create a looped template and process in Integrate. Refer to
    [Configure Process Template Loops for a BDC Script Template with
    Looping
    Enabled](../../../Platform/Integrate/Use_Cases/ConfigureProcTempLoopsBDCLoopEn.htm)
    or [Configure Process Template Loops for a GUI Script Template with
    Looping
    Enabled](../../../Platform/Integrate/Use_Cases/ConfigureProcTemplLoopsGUILoopgEn.htm)
    in Integrate for more information.
2.  [Create all tt Tables and tx Views for the Integrate
    Process](Create_All_tt_Tables_and_tx_Views_for_the_Integrate_Process.htm)
3.  [Create rt Tables from the tt
    Tables](Create_rt_Tables_from_the_tt_Tables.htm)
4.  [Create Custom Pages and Views](Create_Custom_Pages_and_Views.htm)
5.  [Create a Template that Uses the Custom Pages in
    dspCompose™](Create_a_Template_that_uses_the_Custom_Pages.htm)

Refer to [Create Template Roles](Create_Template_Roles.htm) for detailed
information about creating a custom role at the template level.

When the template created in [Create a Template that Uses the Custom
Pages in
dspCompose™](Use_the_Custom_Pages_in_dspCompose_for_the_BAPI_Process.htm)
is saved, a Data Entry role will be automatically generated for the
template. This Data Entry role should be assigned the
<span class="underline"><span style="color: #ff0000;">header</span></span>
data page (created in [Create Data Entry Pages and
Views](Create_Custom_Pages_and_Views.htm#Create_Data_Entry_Pages_and_Views))
following the instructions below. Add a role with Role-Type of ‘Data’
for each additional data entry page, and assign the pages following the
instructions below.

A Review role will also be automatically generated when the template is
saved. Assign this Review role to the header review page (created in
[Create Approval Pages and
Views](Create_Custom_Pages_and_Views.htm#Create_Approval_Pages_and_Views))
following the instructions below. Add a role with Role Type of ‘Review’
for each additional review page, and assign the pages following the
instructions below.

Assign dependencies to the new roles and edit dependencies for existing
Review- and Post-type roles to take the new roles into consideration.
Refer to [Add Role Dependencies](Add_Role_Dependencies.htm) for more
information.

**NOTE**: Customizations can be made to the data entry and/or review
pages to link header and detail pages, thus reducing the number of roles
required to process the data. The approach outlined in this use case is
the most straightforward approach to use as an example.

To add the custom data entry and review pages to the template roles:

1.  Click <span style="font-weight: bold;">Team</span> on
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Templates</span> for a team.

3.  Select **Roles** for the template.

4.  Click **Vertical View** for the header Data Entry role.
    
    <span style="font-weight: bold;">NOTE</span>: This is the Data Entry
    role that was automatically generated for the template when the
    template created in [Create a Template that Uses the Custom Pages in
    dspCompose™](Create_a_Template_that_uses_the_Custom_Pages.htm) was
    saved,

5.  Click the **Page Settings** tab.

6.  Click the **Custom Page** check box to enable it.

7.  Click **Edit**.
    
    [View the field descriptions for the Template (Role) page's Vertical
    View](../Page_Desc/Template_Role_H.htm)

8.  Select the name of the component that stores the custom data entry
    page in **Web App ID** list box.
    
    **NOTE**: The Web App ID is the data entry page created for the
    header data in [Create Data Entry Pages and
    Views](Create_Custom_Pages_and_Views.htm#Create_Data_Entry_Pages_and_Views).

9.  Select the name of the page from the **Page ID** list box.

10. Click **Save**.

11. Repeat steps 1-10 for each of the additional data entry roles.

12. Close the *Template (Role)* page's
    <span style="font-style: italic;">Vertical</span><span>View</span>.

13. Click **Vertical View** for the Review role.

14. Click the **Page Settings** tab.

15. Click the **Custom Page** check box to enable it.

16. Click **Edit**.
    
    <span style="font-size: 11pt;">*[View the field descriptions for the
    Template (Role) page's Vertical
    View](../Page_Desc/Template_Role_H.htm)*</span>

17. Select the name of the component that stores the custom review page
    from the **Web App ID** list box.
    
    **NOTE**: The Web App ID is the header approval page created in
    [Create Approval Pages and
    Views](Create_Custom_Pages_and_Views.htm#Create_Approval_Pages_and_Views).
    Register the view to the appropriate Approval page.

18. Select the name of the page from the **Page ID** list box.

19. Click **Save**.

20. Repeat steps 12-19 for each of the additional Review roles.
    
    **NOTE**: The Post role will use the standard *Request (Post)* page.

To process the request:

1.  Activate the template.

2.  Add a request to use the template.

3.  Click **Roles** for the template.

4.  Click **DATA ENTRY** for the Data role.
    
    **NOTE**: The header Data Entry page displays. The standard import
    options to facilitate data entry can be used. Refer to [Import a
    File at the Request Role
    Level](Import_a_File_at_the_Request%20Role_Level.htm) for more
    information.

5.  Click **Finish** for the Data Entry role once data entry is
    complete.

6.  Process all additional Data Entry roles.

7.  Review and approve the roles.
    
    **NOTE**: The Approval pages created in [Create Approval Pages and
    View](Create_Custom_Pages_and_Views.htm#Create_Approval_Pages_and_Views)
    display when the Review role(s) click DATA ENTRY.

8.  Click **DATA ENTRY** for the Post role.

9.  Click **Post**.
    
    **NOTE**: Posting will be processed by Integrate.

To view posting messages:

1.  Select **Requests** on the *Navigation
    <span style="font-style: normal;">pane</span>*.
2.  Click **Vertical View** for the request.
3.  Click **Archive Page ID**.
4.  View the posting information in the Post Error, Post Message, Posted
    On and Posted By columns.
