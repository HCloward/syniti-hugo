+++
title = 'Create a Custom Template'
solution = 'Data Quality'
+++

# Create a Custom Template

dspCompose™ allows the user to build a custom template, in which
everything about the template, including the tables or views the
template is based on, is created and defined outside of dspCompose™.
Custom templates can be used when setting up and posting a BAPI, or when
linking dspCompose™ to existing applications to use pages from these
applications to create a custom component.

Refer to [Set up and Post a BAPI using Integrate and
dspCompose™](Set_up_and_Post_a_BAPI_Using_Integrate_and_dspCompose.htm)
for more information.

<span style="font-weight: bold;">NOTE</span>: A Post Message table must
be defined on the <span style="font-style: italic;">Template (Post
Message Table) page</span> (Team \> Templates \> Vertical View \>
Configuration \> Post Message Tables). This page must have a record for
the Data Entry table that contains the column where the returned Post
Message is stored. If the Post Message table is not defined, an error
displays when a user clicks Post on the
<span style="font-style: italic;">Request (Roles)</span> page and the
posting process stops.

To create a custom template:

1.  Select **Team** on the *Navigation pane*.

2.  Click **Create Template** for the team.

3.  Click **Create Custom Template**.
    
    **NOTE:** If no records exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    *[View the field descriptions for the Create Custom Template
    page.](Create_Custom_Template.htm)*

4.  Enter a name in **TEMPLATE NAME** field.
    
    **NOTE**: The name must be unique and can contain A-Z, 0-9, and
    underscore. No special characters are allowed in template names. If
    a special character is entered in a template name, dspCompose™ will
    replace it with an underscore when the template is saved.

5.  Enter an ERP transaction code in **TRANSACTION CODE** field.

6.  Select a connection from
    <span style="font-weight: bold;">CONNECTION</span> list box.
    
    <span style="font-weight: bold;">NOTE</span>: Refer to [Establish a
    Connection to a Target
    System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
    for more information.

7.  Click **Save<span style="font-weight: normal;">.</span>**

8.  Click<span style="font-weight: bold;">Complete
    Template</span><span style="font-weight: normal;">icon to create the
    custom template; a confirmation message
    displays.</span>

9.  Click<span style="font-weight: bold;">Ok</span><span style="font-weight: normal;">;
    the</span><span style="font-weight: normal;font-style: italic;">Templates</span><span style="font-weight: normal;">page
    displays.</span>

10. Click <span style="font-weight: bold;">Vertical View</span>.

11. Click **Configuration** tab.

12. Click **Post Message Tables**.
    
    **NOTE**: Post Message Tables are used by the post process to
    determine where posting messages are written when a request is
    posted.
    
    **NOTE:** When the template is saved initially, data source and
    table names are automatically added to the Post Message table.
    Update the data source and table names for a custom template with
    the correct values where posting messages for the custom template
    should be written.

13. Navigate to the *Vertical* View of the *Templates* page.

14. Click the **Configuration** tab.

15. Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Templates page's Vertical
    View.](../Page_Desc/Templates_H.htm#Templates_V_All_Tabs)

16. If the custom template should be based on an Integrate template,
    select the template from **Integrate Template ID** list box.

17. If the custom template should be based on an Integrate process,
    select the template from **Integrate Process ID** list box.
    
    **NOTE**: If the template should be linked to a page in another
    component, refer to [Link a Template to a
    Page](Link_a_Template_to_a_Page.htm) for more
    information.

18. Click<span style="font-size: 11.0pt;font-family: Arial, sans-serif;font-weight: bold;">Save</span>.

19. Click **Advanced** tab.

20. Click **Custom Archive Tables**.
    
    <span style="font-weight: bold;">NOTE:</span> If no records exist,
    the page displays in add mode. Otherwise, click **Add**.
    
    [View the field descriptions for the Template (Archive Settings)
    page](../Page_Desc/Template_Archive_Settings.htm)
    
    **NOTE**: Maintain custom archive tables on the *Template (Archive
    Settings)* page. These tables must be configured in order to
    activate the template.

21. Select an option from **ACTIVE TABLE DATA SOURCE ID** list box.
    
    **NOTE**: The ACTIVE TABLE DATA SOURCE ID stores the table upon
    which the template is based and the data source that contains
    manually created objects for the custom template.

22. Select an option from **ACTIVE TABLE NAME** list box.
    
    <span style="font-weight: bold;">NOTE:</span>The ACTIVE TABLE NAME
    displays the name of the active table on an open request where data
    is pulled from and inserted into the ARCHIVE TABLE NAME.

23. Select an option in the **ARCHIVE TABLE DATA SOURCE ID** list box.
    
    **NOTE**: The ARCHIVE TABLE DATA SOURCE ID stores the table where
    archive data will be written and will be used in step 29 below.

24. Select an option from **ARCHIVE TABLE NAME** list box.
    
    **NOTE:** The ARCHIVE TABLE NAME is the name of the archive table
    where data is inserted from the ACTIVE TABLE NAME.

25. Click **Save**.

26. Navigate to the *Templates* page’s *Vertical* View, **Advanced**
    tab.

27. Click <span style="font-weight: bold;">Edit</span>.
    
    <span style="font-style: italic;">[View the field descriptions for
    the Templates page](../Page_Desc/Templates_H.htm)</span>

28. Select an option from the **Template Archive Web App ID** list box.
    
    **NOTE**: Select the option set in the **ARCHIVE TABLE DATA SOURCE
    ID** on the *Template (Archive Settings)* page in step 24 above.

29. Select
    <span style="font-size: 10.0pt;font-family: Arial, sans-serif;">the
    same option set in the **ARCHIVE TABLE DATA SOURCE ID** on the
    *Template (Archive Settings)* page in step 24 above</span> from the
    **Template Archive Page ID** list box.

30. Select an option from the **Template Archive Page ID** list box.
    
    **NOTE:** This page ID is automatically set for a template when the
    template is processed and when roles are configured. If non-custom
    review roles are used, the Template Archive Page ID is set to the
    system-generated page.

31. Click <span style="font-weight: bold;">Save</span><span>.</span>

32. Click the **General** tab.

33. Click **Generate Custom**.
    
    <span style="font-weight: bold;">NOTE</span>: Do not generate a
    custom template until the custom page settings have been entered on
    the Template (Role) page. Refer to [Assign a Custom Page to a
    Template Role](Assign_a_Custom_Page_to_Template_Role.htm) for more
    information.
    
    **NOTE**: Clicking this icon is required, and must be performed
    before requests can be added and processed for the template. When a
    user clicks this icon, if the custom template uses Org Units,
    dspCompose™ builds the objects associated with Org Units.
    dspCompose™ does not build any other objects for custom templates.
    The Org Unit objects will be built in the database that hosts the
    template's Data Entry page.

34. Click **Activate** on the Page toolbar.
    
    <span style="font-weight: bold;">NOTE</span>: If assigning a custom
    page from a custom WebApp to a role, enter all the custom page
    information following these steps before generating the custom
    template (by clicking <span style="font-weight: bold;">Generate
    Custom</span> on the
    <span style="font-style: italic;">Templates</span> page).
