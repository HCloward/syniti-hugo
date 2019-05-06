# Download Tables

**NOTE**: To receive a workflow email that a table download has failed
in Collect, a user must be assigned to a security role that has the
Collect WebApp group WorkFlowFailureAll or WorkFlowFaiureByTargetAccess
assigned. Refer to [Set
Security](../../../Platform/Sys_Admin/Use_Cases/Setting_security.htm) in
System Administration for more information.

### Download sdb Tables in Collect

To download sdb Source tables in Collect:

1.  Register the sdb\* Target in Collect. Refer to [Register
    Targets](../../../Platform/Collect/Use_Cases/Register_and_Use_Targets.htm#Register_Targets)
    for detailed information.
2.  Register the Source to the sdb\* Target. Refer to [Register Sources
    to
    Target](../../../Platform/Collect/Use_Cases/Register_and_Use_Sources.htm#Register_Sources_to_Target)
    for detailed information.
3.  Register the table to the Source. Refer to [Manually Register Tables
    to
    Source](../../../Platform/Collect/Use_Cases/Manually_Register_Tables_to_Source.htm)
    for detailed information.
4.  Select the table on the
    <span style="font-style: italic;">[Tables](../../../Platform/Collect/Page_Desc/Tables_H.htm)</span>
    page (**Collect \> Tables**).
5.  Click **Build and Refresh** on the Page toolbar.
6.  Perform step 3 and following for each table.

### Download dg\* Tables in Collect

To download the tables in the dg\* database registered at the Wave level
in Collect:

1.  Manually register the tables to the Source for the dg\* Target.
    
    **NOTE:** Refer to [Manually Register Tables to
    Source](../../../Platform/Collect/Use_Cases/Manually_Register_Tables_to_Source.htm)
    in Collect for detailed information.

2.  Build and Refresh each table
    
    **NOTE**: Refer to [Build Package for
    Table](../../../Platform/Collect/Use_Cases/Build_Package_for_Table.htm)
    in Collect for more information.
