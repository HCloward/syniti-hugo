+++
title = "Information Steward Accelerator (ISA) Overview"
weight = 3
layout = "single"
solution = "Data Quality"
+++

# Information Steward Accelerator (ISA) Overview

ISA extracts data that failed Information Steward (IS) rules, then
distributes the data to groups of users. These user groups, called
Project Distributions, can receive the data as an Excel file (.xlsx)
attached to an email or can view a summary of the rule’s data.

Project Distributions, along with users, have rules. These rules have
associated Quality Dimensions by which rules are grouped. Filters can be
applied at the [user](Use_Cases/Configure_User_Filters_ISA) or
[project
distribution](Use_Cases/Configure_Project_Distribution_Filters)
level to filter the data sets sent to specific user groups.

Once rules are processed in IS, ISA sends workflow emails to users who
are configured to receive them. These emails notify the user of failed
records. The email can contain an attachment in .xlsx format with all of
the failed records, or can contain a summary table with failed record
counts for each rule. The email also contains a link to the associated
IS scorecard and back to the DSP platform workflow.

A dashboard is also available in the ISA to visualize the project
distribution and user level statistics not available in the IS
scorecards. Refer to [View the ISA
Dashboard](Use_Cases/View_ISA_Dashboards) for more information.

## Workflow Frequency

The ISA depends on data that fails IS rules, written to a local database
to generate Excel files with reports of failed data. The ISA distributes
reports through workflow emails. The frequency that rules are run and
the frequency that failed data is updated in the database is set in IS.

Service pages in the ISA can be updated to increase the number of times
a day that the ISA checks for updated data sent from IS to the local
database. Updating this frequency in the ISA does not control how
frequently rules are run in IS.

## Setup and Configuration for ISA

Before working with ISA, configure settings and create objects in IS and
Central Management Console (CMC).

<span style="font-weight: bold;">NOTE:</span> All of these steps must be
performed for the ISA to work.

Refer to CMC documentation for information about working in the Central
Management Console.

Use CMC to:

  - Create projects
  - [Create a Database Connection to Store IS failed
    Data](Config/Create_a_Database_Connection_to_Store_IS_Failed_Data)

Use Information Steward to:

  - Create tables for connections
  - Import tables
  - Create views
  - Create rules
  - Bind the rules to tables or views
  - [Run the rules](Config/Run_Rules_in_IS)

Use the System Administration component of the Data Stewardship Platform
(DSP)® to:

1.  [Add
    Users](../../Platform/Sys_Admin/Use_Cases/Create_User_Accounts_in_System_Administration)
2.  [Create an ISA Security
    Role](Use_Cases/Create_an_ISA_Security_Role)
3.  [Assign a Key Value of Target -dgRepository\_IS to the Security
    Role](../../Platform/Sys_Admin/Use_Cases/Assign_Keys_to_Security_Role)
4.  [Add WebApp groups to the security
    role](../../Platform/Sys_Admin/Use_Cases/Assign_WebApp_Groups_to_Security_Role)
5.  [Add Users to the Security
    Role](../../Platform/Sys_Admin/Use_Cases/Assign_Users_to_Security_Roles)
6.  [Set the Connection information for the ISSAP data
    source](Use_Cases/SetconnectionISRepositorySysAdmin)

Use the Common component of the Data Stewardship Platform (DSP)® to:

1.  [Add an SAP Data Services
    Definition](../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common)

Use the Collect component of the Data Stewardship Platform (DSP)® to:

1.  Set Data Services ID for the dgRepository\_IS target.
    
    In Collect, select Targets \> Vertical view for dgRepository\_IS \>
    Edit \> select an option in the Data Services ID list box.

2.  [Set Data Services
    Connections](Config/Set_Data_Services_Connections)

3.  [Build and Refresh
    tables](../../Platform/Collect/Use_Cases/Build_Package_for_Table)

4.  [Refresh Tables if Projects, Rules, or Rule Bindings are
    Updated](Config/Refresh_Tables_if_Projects_Rules_or_Rule_Bindings_are_Updated)

Use the ISA to:

1.  [Activate Users in a Project
    Distribution](Use_Cases/Add_Users_to_a_Project_Distribution)
