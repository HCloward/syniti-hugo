# Manage Targets

A Target is a copy of the ERP table definitions and contains the
destination tables for the Source data.

Use Target Design to add a Target to an object in a context (a Wave and
Process Area) and to assign a Source (or multiple Sources) to the
Target. Refer to [Create the Contexts for Migration
Project](../../Console/Use_Cases/Create_Contexts_for_Migration_Projects.htm)s
and [Add a
Target](../../Design/Use_Cases/Add_a_Target_in_Target_Design.htm) for
more information.

Use Transform to register Target Sources, Target rules, Target
remediation rules, and Target reports. Transform also creates Target
Source rules and Target Source reports.

**NOTE:** Map can be used to write Target rules, Target remediation
rules, Target reports, and Target Source report registrations to
Transform and to create the database objects that these rules and
reports use. SQL AutoGen can also create these objects automatically.
Refer to [SQL AutoGen](../../SQL_AutoGen/SQL_Automation.htm) for more
information.

<span style="font-weight: bold;">NOTE:</span> Data Services can be used
to create Target Data Services Rules. Refer to [Data Services
AutoGen](../../Data_Services_AutoGen/Data_Services_Automation.htm) for
more information.

**NOTE:** Timeout, wait and maximum number of process calls settings for
the execute and polling processes for Data Services AutoGen can be
configured to control access to Data Services Data Sources. Refer to the
[Process
Adapter](../../../Platform/Common/Page_Desc/Process_Adapter.htm) topics
in Common for more information.

To manage Targets, use Transform to:

  - [Edit the Priority and Publish
    Setting](Edit_the_Priority_and_Publish_Setting.htm)
  - [Assign Additional Target
    Sources](Assign_Additional_Target_Sources.htm)
  - [Add Target Rules](Add_Target_Rules.htm)
  - [Add Target Data Services Rules](Add_Target_DS_Rules.htm)
  - [Configure Target Data Services Rule Global
    Variables](Configure_Target_DS_Rule_Global_Var.htm)
  - [Add Target Audit Rules](Add_Target_Audit_Rules.htm)
  - [Add Target Reports](Add_Target_Reports.htm)
  - [Add Target Data Services Reports](Add_Target_DS_Rpts.htm)
  - [Register Target Remediation
    Rules](Register_Target_Remediation_Rules.htm)
  - [Register Target Data Services Remediation
    Rules](Register_Target_DS_Remediation_Rules.htm)
  - [Run Target Data Services Rules](Run_Target_Data_Services_Rules.htm)
  - [Correct Errors in Target Data with Fixed Remediation
    Rules](Correct_Errors_in_Target_Data_With_Fixed.htm)
  - [Correct Errors in Target Data Services Data with Fixed Remediation
    Rules](Correct_Errors_in_Target_DS_Data_With_Fixed.htm)
  - [View Remediation Rule
    Information](View_Remediation_Rule_Information.htm)
  - [View Data Services Remediation Rule
    Information](View_DS_Remediation_Rule_Information.htm)
  - [Add Target Exports](Add_Target_Exports.htm)
  - [Use an Integrate Process as an Export
    Type](Use_an_Integrate_Process_as_an_Export_Type.htm)

On the *[Targets](../Page_Desc/Targets_H.htm)* page, a user can also:

  - View all data for the Target by clicking the **View Target** icon.
  - Monitor any background processes running in the queue for the
    selected Target, including processes for Target reports, Target
    rules and Target exports, by clicking the **Queue** icon.
  - Process the selected Target by clicking the **Process** icon to run
    the entire Target in the background, which imports all data from all
    Sources and runs all Source rules and Source reports, Target rules,
    Target reports and Target exports (in that order).

**NOTE:** To process only Sources, Target rules, Target reports or
Target exports for the selected Target, access the **Process
Information** tab on the *Targets* page’s *Vertical* View.

  - Reset the processing status if a process fails for the Target,
    Target reports, Target rules, and Target exports for the selected
    Target by clicking the **Reset** icon
