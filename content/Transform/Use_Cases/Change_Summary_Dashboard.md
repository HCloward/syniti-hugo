# Change Summary Dashboard

<span style="font-weight: bold;">NOTE:</span> Before data displays on
the Trend Summary reports (Tracking \> Summary) and the Summary Type
charts (Process Area Launch \> Change Summary):

  - Trace must be turned on for the tables, views, functions and
    procedure counts. Refer to [Activate and Deactivate Data
    Sources](../../../Platform/Common/Use_Cases/Activate_and_Deactivate_Data_Source.htm)
    for more information. For Transform, trace must be activated for the
    databases beginning with “dsw."
  - A milestone must be captured. Refer to [Create
    Milestones](Create_Milestones.htm) for more information.

The summary charts displays the count of all Object types in Targets
from the Wave and Process Area level and from the Object level.

Object types include:

  - Tables
  - Procedures
  - Views
  - Functions
  - Other – additional SQL objects, such as synonyms, triggers and table
    functions

Other charts on the dashboard track changes by day, week, and month to
SQL code for each Object type for Targets.

**NOTE:** Charts that display changes to Object types only display data
for the Object types contained in the Targets that have been changed.
For example, if no changes were made to stored procedures, this Object
type does not display below the x-axis.

<span style="font-weight: bold;">NOTE:</span> Charts that display
summary type data only display data for Object types that exist in
Targets. For example, if Targets did not contain stored procedures, this
Object type does not display below the x-axis.

This dashboard contains the following charts:

  - [Summary Type By Wave & Process
    Area](Summary_Type_by_Wave_Process_Area.htm)
  - [Changes Daily By Wave & Process
    Area](Changes_Daily_by_Wave_and_Process_Area.htm)
  - [Changes Weekly By Wave & Process
    Area](Changes_Weekly_by_Wave_and_Process_Area.htm)
  - [Changes Monthly By Wave & Process
    Area](Changes_Monthly_by_Wave_and_Process_Area.htm)
  - [Summary Type By Object](Summary_Type_by_Object.htm)
  - [Changes Daily By Object](Changes_Daily_by_Object.htm)
  - [Changes Weekly By Object](Changes_Weekly_by_Object.htm)
  - [Changes Monthly By Object](Changes_Monthly_by_Object.htm)
