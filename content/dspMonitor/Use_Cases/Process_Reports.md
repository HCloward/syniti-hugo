+++
title = 'Process Reports'
solution = 'Data Quality'
+++

# Process Reports

Reports can be processed at the group level (for all reports and all
users) or at the user level for a single group or a report.  

This use case covers the following topics:

  - [Schedule Reports to Process](#Schedule_Reports_to_Process)
  - [Manually Process Group Reports](#Manually_Process_Group_Reports)
  - [Manually Process Single Report](#Manually_Process_Single_Report)
  - [Manually Process Single Application Table
    Report](#Manually_Process_Single_Application_Table_Report)
  - [Manually Process Single Application Table Column
    Report](#Manually_Process_Single_Application_Table_Column_Report)

## <span id="Schedule_Reports_to_Process"></span>Schedule Reports to Process

Reports can be scheduled to run at the group level. Reports can run on a
daily, weekly or monthly schedule, or a specific date and time can be
configured. Refer to [Create
Schedules](../../../Platform/Common/Use_Cases/Create_Schedules) for
detailed information.

<span style="font-weight: bold;">NOTE</span>: Only a Group Owner can
schedule reports to process for a group.

To schedule reports to process:

1.  Select **Configuration \> Groups** in *Navigation* pane.

2.  Click **Edit** for Group ID.
    
    [View the field descriptions for the Groups
    page](../Page_Desc/Groups_H)

3.  Select a schedule from **GROUP SCHEDULE ID** list box.
    
    **NOTE:** Schedules are maintained in Common. Refer to [Create
    Schedules](../../../Platform/Common/Use_Cases/Create_Schedules)
    for detailed information.

4.  Click
**Save**.

## <span id="Manually_Process_Group_Reports"></span>Manually Process Group Reports

Processing reports at the group level runs all reports for all users.
Only group owners can process reports at this level.

To manually process reports for a group:

1.  Click **Your Groups** in *Navigation* pane.

2.  Click **Process** to execute your reports within the group; a
    confirmation message displays.
    
    *Or*
    
    Click **Process For All Users** to execute all the reports within
    the group for all users who have access to the reports; a
    confirmation message displays.

3.  Click **Ok**; reports are placed in the queue for
processing.

## <span id="Manually_Process_Single_Report"></span>Manually Process Single Report

Users can manually process a single report if the entire report group
does not need to be processed. In order for a report to be manually run,
**Allow Manual Run** must be enabled by the Group Owner. Refer to the
[Register Reports to a Report
Repository](Register_Reports_to_a_Report_Repo) for detailed
information on the **Allow Manual Run** feature.

To manually process a report: 

1.  Click **Your Groups** in *Navigation* pane.

2.  Click the **Reports** or **Favorites** icon.

3.  Click **Execute** to process the report; a confirmation message
    displays.
    
    Or
    
    Click **Execute For All Users** to process the report for all users
    who have access to the report; a confirmation message displays.

4.  Click **OK**; reports are placed in the queue for
processing.

## <span id="Manually_Process_Single_Application_Table_Report"></span>Manually Process Single Application Table Report

Users can manually process a single report if the entire report group
does not need to be processed. In order for a report to be manually run,
Allow Manual Run must be enabled on the *[Repository
Reports](../Page_Desc/Repository_Reports_H)* page’s *Vertical* View.
Refer to the [Register Reports to a Report
Repository](Register_Reports_to_a_Report_Repo) for detailed
information on the Allow Manual Run feature.

To manually process a report:

1.  Select **dspMonitor \> Your Applications** in *Navigation* pane.

2.  Click the **Tables** icon.

3.  Click the **Report** icon.

4.  Click **Vertical View** for a Report.

5.  Click **Execute** to process the report; a confirmation message
    displays.
    
    Or
    
    Click **Execute for All Users** to process the report for all users
    who have access to the report; a confirmation message displays.

6.  Click **OK**; reports are placed in the queue for
processing.

## <span id="Manually_Process_Single_Application_Table_Column_Report"></span>Manually Process Single Application Table Column Report

Users can manually process a single report. if the entire report group
does not need to be processed. In order for a report to be manually run,
Allow Manual Run must be enabled on the *[Repository
Reports](../Page_Desc/Repository_Reports_H)* page’s *Vertical* View.
Refer to [Register Reports to a Report
Repository](Register_Reports_to_a_Report_Repo) for detailed
information on the Allow Manual Run feature.

To manually process a report:

1.  Click **dspMonitor \> Your Applications** in *Navigation* pane.

2.  Click the **Tables** icon.

3.  Click the **Columns** icon.

4.  Click the **Report** icon.

5.  Click **Vertical View** for a Report.

6.  Click **Execute** to process the report; a confirmation message
    displays.
    
    Or
    
    <span style="font-weight: normal;">Click </span>Execute For All
    Users<span style="font-weight: normal;"> to process the report for
    all users who have access to the report; a confirmation message
    displays.</span>

7.  Click **OK**; reports are placed in the queue for processing.
