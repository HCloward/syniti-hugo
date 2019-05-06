# Update Construct WebApp and Data Source

By default, the WebApp that displays the Construction pages is Construct
and the Source data source used for construction pages is
sdbDSPConstruct. Using these default values, a construct page, the
underlying table, menu registrations and the schema of the construction
table are automatically generated. Refer to [Use a Custom WebApp with
Construct](../../Construct/Use_Cases/Use_a_Custom_WebApp_with_Construct.htm)
for more information.

The Construct WebApp and source data source can be changed in Console
for custom WebApps. For example, a client may require that
data-sensitive content be added to a WebApp called ConstructHR. This
data will not be tracked for construction completion status.

To update the WebApp and Source Data Source for Construct in Console:

1.  Select **Waves** in the *Navigation* pane, or select **Console** in
    the Context bar.

2.  Click the **Process Areas** icon for a Wave.

3.  Click the **Vertical View** icon for a Process Area.

4.  Click **Edit**;
    
    *[View the field descriptions for the Wave : Process Areas page’s
    Vertical view](../Page_Desc/Wave_Process_Areas.htm#Wave)*

5.  Select a component in the **Construction Web App ID** list box.

6.  Select a source database in the **Construction Source Data Source**
    list box.
    
    **NOTE**: These data sources are registered in Common. Refer to
    [Register a Data Source in Common](#) for more information.

7.  Click **Save**.
