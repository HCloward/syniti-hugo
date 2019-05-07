+++
title = 'Use the Custom Pages in dspCompose™ for the BAPI Process'
solution = 'Data Quality'
+++

# Use the Custom Pages in dspCompose™ for the BAPI Process

Before performing these steps:

1.  [Post Data Using A
    BAPI](../../../Platform/Integrate/Use_Cases/Post_Data_Using_a_BAPI.htm)
2.  [Create all tt Tables and Views for the BAPI
    Process](Create_tt_Tables_and_Views_for_the_BAP_Process.htm)
3.  [Create rt Tables From the tt Tables and Create Views for the BAPI
    Process](CreatertTblsttTableCreateVwsBAPI.htm)
4.  [Create Custom Pages and Views for the BAPI
    Process](Create_Custom_Pages_and_Views_for_the_BAPI_Process.htm)

Once all the custom pages and their views are created, use them in
dspCompose™ for the BAPI process.

To create the template:

1.  Select **Team** on the *Navigation* pane.

2.  Click **Templates** for a team.

3.  Click **Add**.
    
    *[View the field descriptions for the Templates page’s Vertical
    View.](../Page_Desc/Templates_H.htm#Templates_V_All_Tabs)*

4.  Enter a name in **Template Name** field.

5.  Select **Custom Setup** from the **Type** list box.

6.  Select the target ERP system connection from the **Connection** list
    box.

7.  Click **Save**.

8.  Click **Configuration** tab.

9.  Click **Post Message Tables**.

10. Click **Add**.
    
    *[View the field descriptions for the Template (Post Message Tables)
    page.](../Page_Desc/Template_Post_Message_Tables.htm)*
    
    <span style="font-weight: bold;">NOTE:</span> When the custom
    template is saved, one post message table is created by default. A
    post message table for the main table created in [Create all tt
    Tables and Views for the BAPI
    Process](Create_tt_Tables_and_Views_for_the_BAP_Process.htm) must
    also be added.

11. Select the data source that stores the **tt** table created in
    [Create all tt Tables and Views for the BAPI
    Process](Create_tt_Tables_and_Views_for_the_BAP_Process.htm) from
    the **DATA SOURCE ID** list box.

12.  Select the **tt** table name from the **TABLE NAME** list box.

13. Select **ID** from the **POSTING PRIMARY KEY COLUMN** list box.

14. Select **PostError** from the **POST ERROR COLUMN** list box.

15. Select **PostMessage** from the **POST MESSAGE COLUMN** list box.

16. Click **Save**.

17. Navigate to the *Templates* page’s *Vertical* View.

18. Click **Configuration** tab.

19. Click **Edit**.
    
    *[View the field descriptions for the Templates page’s Vertical
    View.](../Page_Desc/Templates_H.htm)*

20. Select the name of the Integrate BAPI process created in Create a
    BAPI Template and Process in Integrate from the **Integrate Process
    ID** list box.

21. Click **Advanced** tab.

22. Select the component name that contains the Archive page created in
    [Create Archive
    Page](Create_Custom_Pages_and_Views_for_the_BAPI_Process.htm#Create_Archive_Page_for_the_BAPI_Process)
    from the **Template Archive WebAppID** list box.

23. Select the page name for the Archive page created in [Create Archive
    Page](Create_Custom_Pages_and_Views_for_the_BAPI_Process.htm#Create_Archive_Page_for_the_BAPI_Process)
    from the **Template Archive Page ID** list box

24. Click **Save**.

To add the custom data entry and review pages to the template roles:

1.  Select **Roles** for the template.

2.  Click **Vertical View** for the Data role.

3.  Click **Page Settings** tab.

4.  Click the **Custom Page** check box to enable it.

5.  Click **Edit**.
    
    *[View the field descriptions for the Template (Role) page's
    Vertical View](../Page_Desc/Template_Role_H.htm)*

6.  Select the name of the component that stores the custom data entry
    page from the **Web App ID** list box.
    
    **NOTE:** The Web App ID is the data entry page created in [Create
    Data Entry Page and
    View](Create_Custom_Pages_and_Views_for_the_BAPI_Process.htm#Create_Data_Entry_Page_and_View_for_the_BAPI_Process).

7.  Select the name of the page from the **Page ID** list box.

8.  Click **Save**.

9.  Close the <span style="font-style: italic;">Template
    (Role)</span><span>page's</span><span style="font-style: italic;">Vertical</span><span>View.</span>

10. Click **Vertical View** for the Review role.

11. Click **Page Settings** tab.

12. Click the **Custom Page** check box to enable it.

13. Click **Edit**.
    
    *[View the field descriptions for the Template (Role) page's
    Vertical View](../Page_Desc/Template_Role_H.htm)*

14. Select the name of the component that stores the custom review page
    from the **Web App ID** list box.
    
    **NOTE:** The Web App ID is the data entry page created in [Create
    Approval Page and
    View](Create_Custom_Pages_and_Views_for_the_BAPI_Process.htm#Create_Approval_Page_and_View_for_the_BAPI_Process).

15. Select the name of the page from the **Page ID** list box.

16. Click **Save**.
    
    **NOTE**: The Post role will use the standard *Request (Post)* page.

To process the request:

1.  Activate the template.  
    Refer to [Activate the Template](Activate_the_Template.htm)  for
    more information.

2.  Create a request based on the template.  
    Refer to [Create Requests](Create_Requests.htm)  for more
    information.

3.  Click **Roles** for the template.

4.  Click **DATA ENTRY** for the Data role.
    
    **NOTE:** The Data Entry page created in [Create Data Entry Page and
    View](Create_Custom_Pages_and_Views_for_the_BAPI_Process.htm#Create_Data_Entry_Page_and_View_for_the_BAPI_Process)
    displays. The standard import options to facilitate data entry can
    be used. Refer to [Import a View at the Request-Role
    Level](Import_a_View_at_the_Request%20Role_Level.htm) for more
    information.

5.  Click **Finish** for the Data role once data entry is complete.

6.  Review and approve the role.
    
    **NOTE:** The Approval page created in [Create Approval Page and
    View](Create_Custom_Pages_and_Views_for_the_BAPI_Process.htm#Create_Approval_Page_and_View_for_the_BAPI_Process)
    displays when the Review role clicks DATA ENTRY.

7.  Click **DATA ENTRY** for the Post role.

8.  Click **Post**.
    
    **NOTE:** Posting will be processed by Integrate.

To view posting messages:

1.  Select **Requests** on the *Navigation* pane.
2.  Click **Vertical View** for the request.
3.  Click **Archive Page ID**.
4.  View the posting information in the Post Error, Post Message, Posted
    On and Posted By columns.
