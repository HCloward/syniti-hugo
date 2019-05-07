+++
title = 'Target Source Rule Audit H <span id="Target_Source_Rule_Audit_H"></span>'
solution = 'Migration'
+++

# Target Source Rule Audit H <span id="Target_Source_Rule_Audit_H"></span>

[Target Source Rule Audit V (All Tabs)](#Target_Source_Rule_Audit_V)

<div class="use">

Use this page to [Add Source Audit
Rules](../Use_Cases/Add_Source_Audit_Rules.htm).

</div>

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).
2.  Click the **Targets** icon on the *[Process Area
    Launch](Process_Area_Launch.htm)* page.
3.  Click the **Sources** icon for a Target.
4.  Click the **Rules** icon for a Target Source.
5.  Click the **Vertical View** icon for a rule.
6.  Click the **Documentation** tab.
7.  Click the **Audit**
icon.

|               |                                                                                                                                               |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| Field         | Description                                                                                                                                   |
| STATUS        | Displays the <span id="Status" class="popUpLink">status</span> of the Target Source audit report.                                             |
| AUDIT REPORT  | Displays the name of the Target Source audit report after the rule has been processed.                                                        |
| SAMPLE METHOD | Displays the sample method used by the audit rule to select data from the audit report for the audit.                                         |
| RECORD COUNT  | Displays the number of records used in the audit.                                                                                             |
| DURATION      | Displays the amount of time Transform took to process the selected source rule. If the field is empty the source rule has not been processed. |
| ACTION ON     | Displays the date Transform processed the selected Target Source rule.                                                                        |
| DOWNLOAD      | Click to download the sampled data once the Target Source audit rule has been processed.                                                      |

 

## <span id="Target_Source_Rule_Audit_V"></span>Target Source Rule Audit V

[Target Source Rule Audit H](Target_Source_Rule_Audit.htm)

<div class="use">

Use this page to [Add Source Audit
Rules](../Use_Cases/Add_Source_Audit_Rules.htm).

</div>

This page has the following tabs:

  - [General tab](#General_Tab)
  - [Process Information
tab](#Process_Information_Tab)

## <span id="General_Tab"></span>General tab

|              |                                                                                          |
| ------------ | ---------------------------------------------------------------------------------------- |
| Field        | Description                                                                              |
| Source Rule  | Displays the name of the Target Source rule.                                             |
| Audit Report | Displays the name of the audit report. Click to view the SQL definition of the view.     |
| Download     | Click to download the sampled data once the Target Source audit rule has been processed. |

## <span id="Process_Information_Tab"></span>Process Information tab

Field

Description

Record Count

Displays the number of records on the audit report.

Duration

Displays the number of seconds it took to run the audit report. If the
field is blank, the Target Source audit rule has not been run.

Action On

Displays the date when the audit report last ran.

Sample Record Count

Displays the number of sampled records returned using the Sample Method.
If the field is blank, the Target Source audit rule has not been run.

Advanced

Report Format

Displays whether the audit report will translate the column headings,
list field names for column headings, or display both. Field names in
SAP are abbreviations in German.

Sample Method

Displays the sample method used to select data for the audit report.

Sample Only

Click to view the sample records only.

Sample File Location

Click to download the file that was sampled. This file contains all the
records before the sample was taken.

Database Name

Displays the name of the database that stores the audit report.
