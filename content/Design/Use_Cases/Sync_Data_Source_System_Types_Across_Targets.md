# Sync Data Source System Types Across Targets

A Source data source can be assigned to only one System Type across all
Targets and Waves. For example, the Source data source of sdbSAP has
been assigned to the System Type SAPLEGACY for the Target ttMARA. If the
Target ttMAKT also uses the data source of sdbSAP, it cannot use a
different System Type such as SAP. The data source sdbSAP must use the
System Type SAPLEGACY.

An error displays when a user saves a Target Source that uses a Source
data source–System Type combination that is not the same as all other
Source data source-System Type combinations across all Targets in all
Waves.

To correct this error, view the Source data source-System Type
combinations across all Targets and sync them.

To sync:

1.  Select **Configuration \> Source** in the *Navigation* pane.

2.  Click the **Targets** icon for the Source data source.
    
    **NOTE**: The page displays all Targets in all Waves that use the
    data source, including Targets where the System Type has not been
    saved for the Source data source.

3.  Click **Edit**.
    
    [View the field descriptions for the Source Where Used
    page](../Page_Desc/Source_Where_Used.htm)

4.  Select the System Type in the **SYSTEM TYPE ID** list box that
    should be used for a Target.

**NOTE**: The same System Type should be selected for each Target that
has a System Type set.
