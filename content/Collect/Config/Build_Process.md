+++
title = 'Build Process'
solution = 'Platform'
+++

# Build Process

The following is a high-level overview of how Collect builds packages
and pulls data from the Source system.

1.  [Create Source and Target
    connections](../../Sys_Admin/Use_Cases/Register_a_Data_Source.htm)
    in System Administration (performed by an Administrator)
2.  [Register Targets in
    Collect](../Use_Cases/Register_and_Use_Targets.htm#Register_Targets)
3.  [Register Sources in
    Collect](../Use_Cases/Register_and_Use_Sources.htm#Register_Sources_to_Target)
4.  [Fetch tables](../Use_Cases/Register_and_Use_Tables.htm), which will
    build a System Type Group with the name of the Source in Common.
5.  [Activate the Tables in the System Type Group in
    Common](../../Common/Use_Cases/Activate_Deactivate_Tbls_System_Type_Group.htm).
6.  [Import the System Type Group tables in
    Collect](../Use_Cases/Import_Group_Tables.htm).
7.  [Build packages in Collect](../Use_Cases/Build_Package_Overview.htm)
    that automatically create tables, indices and primary keys
8.  [Refresh data in Collect](../Use_Cases/Refresh_Overview.htm).
