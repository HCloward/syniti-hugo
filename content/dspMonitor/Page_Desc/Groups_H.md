+++
title = 'Groups H'
solution = 'Data Quality'
+++

# Groups H

[Groups V (All Tabs](#Groups_V_All_Tabs))

<div class="use">

Use this page to:

  - [Assign a Group Owner to a
    Report](../Use_Cases/Assign_Group_Owner_to_a_Report.htm)
  - [Create Groups](../Use_Cases/Create_Groups_dspMonitor.htm)
  - [Configure Workflow Schedules for
    Groups](../Use_Cases/Manage_Workflow_Emails.htm#Configure_Workflow_Schedules_for_Groups)
  - [Schedule Reports to
    Process](../Use_Cases/Process_Reports.htm#Schedule_Reports_to_Process)

</div>

To access this page, select **dspMonitor \> Configuration \>
Groups** in *Navigation* pane.

|                            |                                                                                                                                                                                                     |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                      | Description                                                                                                                                                                                         |
| GROUP ID                   | Displays name of report group.                                                                                                                                                                      |
| GROUP DESCRIPTION          | Displays description of report group.                                                                                                                                                               |
| GROUP OWNER                | Displays individual whose task is to manage reports registered to the group and to define the report-level parameters. Only users with security to dspMonitor™ display in the GROUP OWNER list box. |
| GROUP SCHEDULE ID          | Displays schedule that indicates the frequency the group is run.                                                                                                                                    |
| NEXT GROUP PROCESS TIME    | Displays the next date and time the group is scheduled to run.                                                                                                                                      |
| WORKFLOW SCHEDULE ID       | Displays schedule that indicates the frequency of workflow emails.                                                                                                                                  |
| NEXT WORKFLOW PROCESS TIME | Displays the next date and time the group is scheduled to run.                                                                                                                                      |
| Group Report               | Click to manage reports assigned to group.                                                                                                                                                          |
| User                       | Click to manage users assigned to group.                                                                                                                                                            |
| Workflows                  | Click to view workflow emails that were sent for the group reports.                                                                                                                                 |

## <span id="Groups_V_All_Tabs"></span>Groups V (All Tabs)

[Groups H](Groups_H.htm)

<div class="use">

Use this page to:

  - [Assign a Group Owner to a
    Report](../Use_Cases/Assign_Group_Owner_to_a_Report.htm)
  - [Create  Groups](../Use_Cases/Create_Reports.htm)
  - [Configure Workflow Schedules for
    Groups](../Use_Cases/Manage_Workflow_Emails.htm#Configure_Workflow_Schedules_for_Groups)
  - [Schedule Reports to
    Process](../Use_Cases/Process_Reports.htm#Schedule_Reports_to_Process)
  - [Change Frequency of User
    Workflows](../Use_Cases/Tips_and_Troubleshooting.htm#Change_Frequency_of_User_Workflows)

</div>

This page contains the following tabs:

  - [General tab](#General_Tab1)
  - [Report Scheduling tab](#Report_Scheduling_Tab)
  - [Workflow Scheduling tab](#Workflow_Scheduling_Tab)
  - [Action tab](#Action_Tab)

## <span id="General_Tab1"></span>General tab

[Groups H](Groups_H.htm)

Field

Description

Group ID

Displays name of report group.

Group Description

Displays description of report group.

Group Owner

Displays individual whose task is to manage reports registered to the
group and to define the report-level parameters. Only users with
security to dspMonitor™ display in the Group Owner  list box.

Display Error Metric

If checked, error metrics for the group display under Dashboard in the
<span style="font-style: italic;">Navigation</span> pane.

Data Quality Scoring Threshold

Threshold ID

Displays the threshold ID used for data quality scoring.

**NOTE:** If a Threshold ID is not populated at the Object level, the
provided set on the *Parameters* page is used to calculate data quality
score status on the *Your Groups* page. Refer to [Register Data Quality
Score
Thresholds](../Use_Cases/Populate_Configuration_Tables.htm#Register_Data_Quality_Score_Thresholds)
for more information.

## <span id="Report_Scheduling_Tab"></span>Report Scheduling tab

[Groups
H](Groups_H.htm)

|                         |                                                                  |
| ----------------------- | ---------------------------------------------------------------- |
| Field                   | Description                                                      |
| Group Schedule ID       | Displays schedule that indicates the frequency the group is run. |
| Next Group Process Time | Displays the next date and time the group is scheduled to run.   |

## <span id="Workflow_Scheduling_Tab"></span>Workflow Scheduling tab

<div class="use">

Use this tab to [Configure Workflow Schedules for
Groups](../Use_Cases/Manage_Workflow_Emails.htm#Configure_Workflow_Schedules_for_Groups).

</div>

[Groups
H](Groups_H.htm)

|                      |                                                                    |
| -------------------- | ------------------------------------------------------------------ |
| Field                | Description                                                        |
| Workflow Schedule ID | Displays schedule that indicates the frequency of workflow emails. |

## <span id="Action_Tab"></span>Action tab

[Groups
H](Groups_H.htm)

|                             |                                                                                   |
| --------------------------- | --------------------------------------------------------------------------------- |
| Field                       | Description                                                                       |
| Process                     | Click to execute the reports within the group.                                    |
| Send Group Summary Workflow | Click to send a summary email of all reports within the group to all group users. |
