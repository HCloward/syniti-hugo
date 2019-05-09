+++
title = 'Create a System Type Group from Source Tables'
solution = 'Platform'
+++

# Create a System Type Group from Source Tables

System Type groups are logical groupings of tables, such as Customer or
Vendor. Use System Type groups for source database systems where a large
number of tables must be created and downloaded.

Create these groups using one of these methods:

  - [Create System Type groups from the Fetch
    process.](Create_Groups_from_the_Fetch_Process)
  - Create System Type groups from existing source tables.
  - [Create System Type groups manually in
    Common.](../../Common/Use_Cases/Add_System_Types_Groups)

To create groups from Existing Source Tables:

1.  Select **Collect \>Targets** in the *Navigation* pane.
2.  Click the **Sources** icon for a dgSAP Target.
3.  Click **Vertical View** icon for a SOURCE.
4.  Select the **Action** tab.
5.  Click the **Build Group** icon.

A System Type group is created with the naming convention
\<Target\>\_\<Source\> and the schema owner is defaulted to dbo for the
Group.

Example: dgSAP\_SAPRD2 for all active tables in Collect configuration.
