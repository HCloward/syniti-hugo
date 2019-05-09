+++
title = 'Create a Template that Uses the Custom Pages in dspCompose™'
solution = 'Data Quality'
+++

# Create a Template that Uses the Custom Pages in dspCompose™

Before performing this task:

1.  Create a looped template and process in Integrate. Refer to
    [Configure Process Template Loops for a BDC Script Template with
    Looping
    Enabled](../../../Platform/Integrate/Use_Cases/ConfigureProcTempLoopsBDCLoopEn)
    or [Configure Process Template Loops for a GUI Script Template with
    Looping
    Enabled](../../../Platform/Integrate/Use_Cases/ConfigureProcTemplLoopsGUILoopgEn)
    in Integrate for more information.
2.  [Create all tt Tables and tx Views for the Integrate
    Process](Create_All_tt_Tables_and_tx_Views_for_the_Integrate_Process)
3.  [Create rt Tables from the tt
    Tables](Create_rt_Tables_from_the_tt_Tables)
4.  [Create Custom Pages and Views](Create_Custom_Pages_and_Views)

Once all of the custom pages and their views are created, follow these
steps to use them in
dspCompose<span style="font-family: Arial, sans-serif;">™</span>.

<span style="font-weight: bold;">NOTE</span>: A Post Message table must
be defined on the <span style="font-style: italic;">Template (Post
Message Table) page</span> (Team \> Templates \> Vertical View \>
Configuration \> Post Message Tables). This page must have a record for
the Data Entry table that contains the column where the returned Post
Message is stored. If the Post Message table is not defined, an error
displays when a user clicks Post on the
<span style="font-style: italic;">Request (Roles)</span> page and the
posting process stops.

To create a template that uses the custom pages:

1.  Select **Team** on the *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Add**.
    
    **NOTE**: If creating the template on the *Create Template* page, do
    not use the **Create From Integrate Template** option to create the
    template.
    
    *[View the field descriptions for the Templates page’s Vertical
    View.](../Page_Desc/Templates_H#Templates_V_All_Tabs)*

4.  Enter a name in **Template Name** field.

5.  Select **Custom Setup** from the **Type** list box.

6.  Select the target ERP system connection from the **Connection** list
    box.

7.  Click **Save**.

8.  Click **Configuration** tab.

9.  Click **Post Message Tables**.

10. Click **Add**.
    
    *[View the field descriptions for the Template (Post Message Tables)
    page.](../Page_Desc/Template_Post_Message_Tables)*
    
    <span style="font-weight: bold;">NOTE</span>: When the custom
    template is saved, one post message table is created by default. A
    post message table for the main table created in [Create all tt
    Tables and tx Views for the Integrate
    Process](Create_All_tt_Tables_and_tx_Views_for_the_Integrate_Process)
    must also be added.

11. Select the data source that stores the **tt** tables created in
    [Create all tt Tables and tx Views for the Integrate
    Process](Create_All_tt_Tables_and_tx_Views_for_the_Integrate_Process)
    from the **DATA SOURCE ID** list box.

12. Select the **tt** table name for the
    <span class="underline"><span style="color: #ff0000;">header</span></span>
    table from the **TABLE NAME** list box.

13. Select **ID** from the **POSTING PRIMARY KEY COLUMN** list box.

14. Select **PostError** from the **POST ERROR COLUMN** list box.

15. Select **PostMessage** from the **POST MESSAGE COLUMN** list box.

16. Click **Save**.

17. Click **Add**.
    
    *[View the field descriptions for the Template (Post Message Tables)
    page.](../Page_Desc/Template_Post_Message_Tables)*

18. Select the data source that stores the **rt** tables created in
    [Create all tt Tables and tx Views for the Integrate
    Process](Create_All_tt_Tables_and_tx_Views_for_the_Integrate_Process)
    from the **DATA SOURCE ID** list box.

19. Select the **rt** table name for the
    <span class="underline"><span style="color: #ff0000;">header</span></span>
    table from the **TABLE NAME** list box.

20. Select **ID** from the **POSTING PRIMARY KEY COLUMN** list box.

21. Select **PostError** from the **POST ERROR COLUMN** list box.

22. Select **PostMessage** from the **POST MESSAGE COLUMN** list box.

23. Click **Save**.
    
    **NOTE**: The following steps must be performed for *each
    additional***tt / rt** table combination:

24. Click **Add**.
    
    *[View the field descriptions for the Template (Post Message Tables)
    page.](../Page_Desc/Template_Post_Message_Tables)*

25. Select the data source that stores the **tt** tables created in
    [Create all tt Tables and tx Views for the Integrate
    Process](Create_All_tt_Tables_and_tx_Views_for_the_Integrate_Process)
    from the **DATA SOURCE ID** list box.

26. Select the **tt** table name for the
    <span class="underline"><span style="color: #ff0000;">detail</span></span>
    table from the **TABLE NAME** list box.

27. Select **ParentID** from the **POSTING PRIMARY KEY COLUMN** list
    box.

28. Select **PostError** from the **POST ERROR COLUMN** list box.

29. Select **PostMessage** from the **POST MESSAGE COLUMN** list box.

30. Click **Save**.

31. Click **Add**.

32. Select the data source that stores the **rt** tables created in
    [Create all tt Tables and tx Views for the Integrate
    Process](Create_All_tt_Tables_and_tx_Views_for_the_Integrate_Process)
    from the **DATA SOURCE ID** list box.

33. Select the **rt** table name for the
    <span class="underline"><span style="color: #ff0000;">detail</span></span>
    table from the **TABLE NAME** list box.

34. Select **ParentID** from the **POSTING PRIMARY KEY COLUMN** list
    box.

35. Select **PostError** from the **POST ERROR COLUMN** list box.

36. Select **PostMessage** from the **POST MESSAGE COLUMN** list box.

37. Click **Save**.

To continue configuring the template:

1.  Navigate to the *Templates* page’s *Vertical* View.

2.  Click **Configuration** tab.

3.  Click **Edit**.
    
    [View the field descriptions for the Templates page’s Vertical
    View.](../Page_Desc/Templates_H#Templates_V_All_Tabs)

4.  Select the name of the Integrate template created in Create a Looped
    Template and Process in Integrate from the **Integrate Template ID**
    list box.

5.  Select the name of the Integrate process created in Create a Looped
    Template and Process in Integrate from the **Integrate Process ID**
    list box.

6.  Click **Advanced** tab.

7.  Select the component name that contains the Archive pages created
    for the
    <span class="underline"><span style="color: #ff0000;">header</span></span>
    loop in [Create Archive
    Pages](Create_Custom_Pages_and_Views#Create_Archive_Pages) from
    the **Template Archive WebAppID** list box.

8.  Select the page name for the Archive page created in [Create Archive
    Pages](Create_Custom_Pages_and_Views#Create_Archive_Pages) from
    the **Template Archive Page ID** list box.
    
    **NOTE**: The page listed here will be the page linked to from
    **Archive Page ID** on the *Request* page after posting. Depending
    upon the business requirements, modifications may need to be made to
    this page and underlying view to link to pages for the other data
    entered and archived.

9.  Click **Save**.

10. Click **Custom Archive Tables**.
    
    [View the field descriptions for the Template (Archive Settings)
    page](../Page_Desc/Template_Archive_Settings)

11. Click **Add.**

12. Select the component name that contains the **tt** tables created in
    [Create all tt tables and tx views for the Integrate
    Process](Create_All_tt_Tables_and_tx_Views_for_the_Integrate_Process)
    from the <span style="font-weight: bold;">ACTIVE TABLE DATA SOURCE
    ID</span> list box.

13. Select the tt
    <span class="underline"><span style="color: #ff0000;">header</span></span>
    table name from the **Active Table Name** list box.

14. Select the component name that contains the **rt** tables created in
    [Create rt Tables from the tt
    Tables](CreatertTblsttTableCreateVwsBAPI) from the
    <span style="font-weight: bold;">ARCHIVE TABLE DATA SOURCE ID</span>
    list box.

15. Select the corresponding **rt** table name from the
    <span style="font-weight: bold;">ARCHIVE TABLE NAME</span> list box.
    
    **NOTE**: Repeat steps 11-15 for each of the
    **tt**/**rt**<span class="underline"><span style="color: #ff0000;">detail</span></span>
    tables created for the Integrate Process loops.
    
    Continue with [Add Custom Roles for the Looped
    Template](Add_Custom_Roles_for_the_Looped_Template).
