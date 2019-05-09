+++
title = 'Use Target Design with Full Construction'
solution = 'Migration'
+++

# Use Target Design with Full Construction

To begin a Full Construction in Target Design, add a Target Source as
{Full Construction}.

**NOTE**: If the default WebApp (Construct) and the default data source
(sdbDSPConstruct) is not used, the AutoGen process outlined in this
section is not performed. Refer to [Update the WebApp and Source Data
Source for
Construct](../../Console/Use_Cases/Update_Construct_WebApp_and_Data_Source)
for more information.

<span style="font-weight: bold;">NOTE</span> After a {Full Construction}
Target Source has been saved and the Target has been synced to Map, a
user can update the Length field to a larger number and this update is
applied to the Construct table when the Target is next synced. However,
a user cannot update the Length field to a smaller number and cannot
change the Data Type after the {Full Construction} Target Source has
been saved and the Target has been synced to Map.

To add the Target Source in Target Design:

1.  Click **dspMigrate** in the *Navigation* pane.

2.  Click **Design** in the Context bar.

3.  Click the **Targets** icon on the
    *[Design](../../Design/Page_Desc/Design)* page.

4.  Click the **Sources** icon for a Target.

5.  Click **Add**.
    
    *[View the field descriptions for the Target Sources
    page](../../Design/Page_Desc/Target_Sources_H_Design)*
    
    **NOTE**: The Add button is only available if the selected Target
    has a Design Status of In Design.

6.  Select **{Full Construction}** from the **SOURCE DATA SOURCE** list
    box.

7.  Select **Full Construction** from the **SOURCE TYPE** list box.
    
    **NOTE**: This is a hard-required field.

8.  Click **Save**.

9.  Click **Vertical View** for the Full Construct Target Source.

10. Click **Edit**.
    
    [View the field descriptions for the Target Sources page’s Vertical
    View](../../Design/Page_Desc/Target_Sources_H_Design#Target_Sources_V)

11. Select a value from the **Construct Auto Gen Level** list box.
    Values are:
    
      - **Off** - Construct objects and pages are not generated.
    
      - **New** - Adds new fields to the page table and new column
        properties to page. Does not rebuild page views.
    
      - **Rebuild** - Drops and recreates all views and column
        properties and adds new fields to the page table.

12. Select a value from the **Construct Auto Gen Build View** list box.
    Values are:
    
      - **Horizontal Only** – All fields are displayed and editable on
        the *Horizontal* View.
    
      - **Horizontal/Vertical Mix** – Only required fields are displayed
        and editable on the *Horizontal* View. All other fields are on
        the *Vertical* View.
    
      - **Vertical Only** – All fields are edited on the *Vertical*
        View.
        
        **NOTE:** The tabs on the *Construct* page’s *Vertical* View are
        created and displayed based on the Application Screen, Field
        Order and Key Field settings on the *[Target
        Fields](../../Design/Page_Desc/Target_Fields_H_Target_Design)*
        page’s *Vertical* View:
        
          - If an application screen is specified, a tab with the
            Application Screen name is created.
          - If no application Screen is specified, a tab labeled Not
            Specified is created.
          - If **Vertical Only** is selected for **Construct Auto Gen
            Build View** all fields identified as key fields on the
            *[Target
            Fields](../../Design/Page_Desc/Target_Fields_H_Target_Design)*
            page’s *Vertical* View are edited on a tab labeled Required
            Fields. Key fields are always displayed on the *Horizontal*
            View.
          - Fields are sorted based on the Field Order field.

13. Click **Save**.

14. On the *[Targets](../../Design/Page_Desc/Targets_H_Design)*
    page, select the Target.

15. Click the **Sync to Map** icon in the Page toolbar.

When the user clicks the Sync to Map icon (active when the Target is in
a Design Status of In Design or Design Finished), the following occurs:

  - In Assemble, a CranPort package is built to move data from the
    Construct table underlying the page to the sdbDSPConstruct data
    source.
  - In Collect, the process is registered with a Target of
    sdbDSPConstruct and a Source of Construct with the table name of the
    table underlying the Construct page.
  - The Construction page is created using all active fields within the
    specified Target in Design.

**NOTE**: If any part of the Collect registration for the Target or
Source is not present, the sync to Map process adds the Target or Source
(within Collect) as needed before adding the table.

  - In Target Design, the data source sdbDSPConstruct is added to the
    [Target Sources](../../Design/Page_Desc/Target_Sources_H_Design)
    page as a Source data source.
  - In the sdbDSPConstruct data source, the pages, tables, menu
    registrations and the schema of the construction table are added.
  - In the table underlying the Construct page, a column is added for
    the Wave and Process Area that contains the Target and Source (i.e.,
    the context where the Construct page was added), which sets security
    for the Construct page. Only users who have access to the context
    can enter data on the Construct page.
  - A column is added to the table to track when construction is
    complete for a field.

**NOTE**: Records are complete based on site-specific requirements and
can be enforced by stored procedures registered to an event on the
Construct page.

  - The following column properties are automatically generated when a
    Construct page is created:
    
      - Indicator fields in SAP are assigned a column property of
        checkbox with allowed values of 'X' and ' '.
        
        **NOTE:** The Checkbox field format is configured on the *Target
        Fields* page’s *Vertical* View.
    
    <!-- end list -->
    
      - Date fields are assigned a column property of DateTime with a
        format of Date.
        
        **NOTE:** The Date field format is configured on the *Target
        Fields* page’s *Vertical* View.

<!-- end list -->

  - Basic validations to check the following on the *Construct* page are
    automatically generated:
    
      - Duplicate data in a primary key
      - Invalid values
      - Empty required field

<!-- end list -->

  - When using Target Design with Full Construction, fields with an
    associated check table or domain value in Map on the *[Value Mapping
    (Config)](../../Map/Page_Desc/Value_Mapping_Config_H)* page are
    generated with list boxes and the list box format can be configured
    on the *[Construct](../Page_Desc/Construct_Page)* page. However,
    list boxes are not generated for fields with a 'master data'
    configuration type.

  - Fields that are deactivated in Target Design are hidden on the
    Construct page with a page view. To prevent the loss of constructed
    data if a user incorrectly deactivates a field in Target design, the
    field remains in the DCS table and any previously constructed data
    remains in the field.

  - Key fields are set as hard-required on the Construct page and
    required fields are set to soft-required.

  - If a required indicator is changed in Target Design, the change is
    reflected on the Construct page.

  - In Map, the Target Source is registered on the
    <span style="font-style: italic;">Target Sources</span> page, with
    the Target table name, a Source ID of DSPConstruct and a Source
    database object (i.e., the Source table) that is stored in the
    DSPCostruct sdb. All active fields for the Target are added with a
    default action of Copy.

  - In Transform, rules are processed using the dspDSPConstruct database
    to update Target Rules.

  - In Target Design, to view the name of the construction page that was
    created, click *Vertical* View for the {Full Construction} Source
    data source on the *[Target
    Sources](../../Design/Page_Desc/Target_Sources_H_Design)* page.
    The Construction Page ID field lists the name of the page which
    follows the naming convention \[WebApp ID\] – \[Target table name\]
    – Full Construct – \[Wave name\].

**NOTE**: A user can register a different page for Full Construction
than the page that was automatically generated. However, if the user
updates the Construction Page ID field with this other page name, none
of the automation (such as adding fields to the Construct page) is
performed and the construction page must be built manually. Refer to
[Build a Construction Page
Manually](../../../Platform/Common/Use_Cases/Build_a_Construction_Page_Manually)
for more information.

**NOTE**: If a field is activated in Target Design after the Construct
page was generated, the Construct page is updated with the newly
activated field. If a field is deactivated in Target Design after the
Construct page was generated, the column is not deleted from the
Construct page. It must be manually removed from the table.
