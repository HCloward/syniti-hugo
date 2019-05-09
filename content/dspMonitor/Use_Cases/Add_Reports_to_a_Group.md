+++
title = 'Add Reports to a Group'
solution = 'Data Quality'
+++

# Add Reports to a Group

Add reports to the group and configure report-level settings.

To add reports to a group:

1.  Click **Your Groups** in *Navigation* pane.
    
    <span style="font-weight: bold;">NOTE</span>: The group must have at
    least one report assigned for data to display on this page.

2.  Click **Vertical View** for Group ID.

3.  Click **Group Reports** .
    
    **NOTE:** The <span style="font-weight: bold;">Group Reports</span>
    is only available if the current user is the group owner for the
    group.

4.  Click **Add**.
    
    [View the field descriptions for the Group Reports
    page](../Page_Desc/Group_Reports_H)

5.  Select a repository from the **REPOSITORY** list box to indicate
    where the report is located.

6.  Select a report from the **REPORT** list box; only the reports
    within the Repository display.

7.  Click **METRICS**<span style="font-weight: bold;">STATUS</span>
    check box to enable it, allowing metrics for the group to display
    under the Dashboard menu.

8.  Click **Save**.

9.  Click **Cancel**.
    
    <span style="font-weight: bold;">NOTE</span>: Clicking Cancel closes
    persistent insert mode and allows the user to edit the report.

10. Click **Vertical View** for Report.

11. Click **Edit**.
    
    [View the field descriptions for the Group Reports page's Vertical
    View](../Page_Desc/Group_Reports_H)

12. Enter a schedule in **Schedule Group** field to run large reports in
    a single thread.
    
    **NOTE:** Running a report in a single thread prevents the system
    from being overloaded and allows reports to be built from cache
    tables. It also supports a new concept of building reports from
    Cache Tables to increase performance if a view that contains over 10
    joins on large source tables.

13. Update the **Schedule Priority** field if the default value is not
    applicable. 
    
    **NOTE:** If running reports in a single thread, the Schedule
    Priority determines the order in which reports are run.  This can be
    used to adjust the order of multithread processing if some reports
    should process first. If Schedule Priority is left blank, reports
    are run in alphabetical order.

14. Click **Save**.
