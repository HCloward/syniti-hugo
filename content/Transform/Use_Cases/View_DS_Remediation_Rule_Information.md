# View Data Services Remediation Rule Information

The *Target Data Services Remediation Overview* pages are centralized
reporting locations for Remediation-based operations. Depending on how
the user accesses the pages, Transform displays rule information for a
selected Target report or for all reports for a Target with either an
active fixed Data Services remediation rule or at least one active Data
Services remediation rule.

**NOTE:** For the Data Services options and pages to be available, the
Data Services repository must be defined on the AutoGen \> Configuration
\> *[Data Services
Repositories](../../Data_Services_AutoGen/Page_Desc/Data_Services_Repositories_H.htm)*
page. Refer to [Configure a Data Services
Repository](../../Data_Services_AutoGen/Use_Cases/Configure_a_DS_Repository.htm)
and [Data Services
AutoGen](../../Data_Services_AutoGen/Data_Services_Automation.htm) for
additional details on setting up Data Services for the DSP®.

**NOTE:** For the Data Services options and pages to be available, the
Data Service Repository must also be registered in Common. The Data
Services check box must be checked in Console for the Process Area:
Object. Refer to [Register a Data Source in
Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
and  [Create the Context by Adding a Wave and Creating
Elements](../../Console/Use_Cases/Add_a_Wave_and_Create_Elements.htm)
for more information.

To access the *Target Data Services Remediation Overview* page, click
the **Data Services Remediations** icon for the selected Target on the
*[Targets](../Page_Desc/Targets_H.htm)* page's *Horizontal* View.

To access the *Target Data Services Remediation Overview* page for a
specific Target report, click the **Data Services Reports** icon for the
Target, and click the **Data Services Remediations** icon for the report
on the *Target Data Services Reports* page.

**NOTE:** The Data Services Remedations icon displays active when
remediation rules exist for the Target.

The Remediation page contains information about the Target report’s
Remediation metrics for both remediation rules and fixed remediation
rules.

*[View the field descriptions for the Target Data Services Remediation
Overview page.](../Page_Desc/Target_DS_Remediation_Overview.htm)*

On this page:

  - Click **Edit** to access the *Target Data Services Remediation
    Setup* page to view and configure the Target data services report’s
    remediation rule or fixed remediation rule settings. Refer to
    [Register Target Data Services Remediation
    Rules](Register_Target_DS_Remediation_Rules.htm) and [Correct Errors
    in Target Data Services Data with Fixed Remediation
    Rules](Correct_Errors_in_Target_DS_Data_With_Fixed.htm) for more
    information.

  - In the FIXED REMEDIATION column, view information related to the
    fixed remediation rule, including the number of records affected by
    the rule. If the fixed remediation rule has not been run, the count
    displays the number of records on the report. Click the **Count**
    button to view all remediated records.

  - In the REMEDIATION RULES column, view information including the name
    of the stored procedure and the number of records remediated. Record
    Count displays the number of records affected by the remediation
    rule’s execution. Records Remediated displays the number of records
    that were remediated. These counts will not necessarily be the same
    value.
