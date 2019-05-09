# Setup and Configuration for ISA

Before working with ISA, configure settings and create objects in IS and
Central Management Console (CMC).

<span style="font-weight: bold;">NOTE:</span> All of these steps must be
performed for the ISA to work.

Refer to CMC documentation for information about working in the Central
Management Console.

Use CMC to:

  - Create projects
  - [Create a Database Connection to Store IS Failed
    Data](../Config/Create_a_Database_Connection_to_Store_IS_Failed_Data)

Use Information Steward to:

  - Create tables for connections
  - Import tables
  - Create views
  - Create rules
  - Bind the rules to tables or views
  - [Run the rules](../Config/Run_Rules_in_IS)

Use the System Administration component of the Data Stewardship Platform
(DSP)® to:

1.  Add Users
2.  Create an ISA Security Role
3.  Assign a Key Value of Target -dgRepository\_IS to the Security Role
4.  Add WebApp groups to the security role
5.  Add Users to the Security Role
6.  Set the Connection information for the ISSAP data source

Use the Common component of the Data Stewardship Platform (DSP)® to:

1.  [Add an SAP Data Services
    Definition](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common)

Use the Collect component of the Data Stewardship Platform (DSP)® to:

1.  Set Data Services ID for the dgRepository\_IS target.
    
    In Collect, select Targets \> Vertical view for dgRepository\_IS \>
    Edit \> select an option in the Data Services ID list box.

2.  [Set Data Services
    Connection](../Config/Set_Data_Services_Connections)

3.  [Build and Refresh
    tables](../../../Platform/Collect/Use_Cases/Build_Package_for_Table)

4.  [Refresh Tables if Projects, Rules, or Rule Bindings are
    Updated](../Config/Refresh_Tables_if_Projects_Rules_or_Rule_Bindings_are_Updated)

Use the ISA to:

1.  [Activate Users in a Project
    Distribution](Add_Users_to_a_Project_Distribution)
