+++
title = 'Use a Custom WebApp with Construct'
solution = 'Migration'
+++

# Use a Custom WebApp with Construct

A custom WebApp and its data source can be used with Construct. For
example, a client may require that data-sensitive content be added to a
custom WebApp called ConstructHR.

To use a custom WebApp with Construct, an Administrator must:

1.  Add the custom WebApp to the platform in System Administration.

2.  Assign users to the WebApp group for the custom WebApp to grant
    users access to the pages in the WebApp in System Administration.

3.  [Update the WebApp and Source Data Source for
    Construct](../../Console/Use_Cases/Update_Construct_WebApp_and_Data_Source)

4.  Build a Construction Page for a Custom WebApp Using AutoGen

To begin building the Construction page, add a Source of {Full
Construction} in Target Design:

1.  Select <span style="font-weight: bold;">Design</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Select the <span style="font-weight: bold;">Targets</span> icon on
    the *[Design](../../Design/Page_Desc/Design)* page.

3.  Select the <span style="font-weight: bold;">Sources</span> icon for
    a Target.

4.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Target Sources
    page](../../Design/Page_Desc/Target_Sources_H_Design)
    
    **NOTE:** The Add button is only available if the selected Target
    has a Design Status of In Design.

5.  Select <span style="font-weight: bold;">{Full Construction}</span>
    from the <span style="font-weight: bold;">SOURCE DATA SOURCE</span>
    list box.

6.  Click <span style="font-weight: bold;">Save</span>.

Once the source is saved, AutoGen:

  - Creates the underlying table for the page
  - Adds the fields to be used on the page to the table
  - Builds a CranPort package for the process to move the data entered
    in the Construct page to the sdbDSPConstruct data source
  - Registers the process in Collect as target sdbDSPConstruct and
    source of Construct with the table name of the table created for the
    constructed page
  - Assigns the page to the Source in Target Design with the name
    \[Target\] - \[Source\] - Full Construct - \[Wave\] (for example,
    Construct - MARC -FullConstruct-\_GLOBALTD).
