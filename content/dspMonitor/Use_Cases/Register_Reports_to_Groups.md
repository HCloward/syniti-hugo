# Register Reports to Groups

Once a report is registered to a repository, it is then registered to a
group or to multiple groups. Since reports can be assigned to multiple
groups, configuration settings can be changed based on group
requirements. From there, users are registered to the group to access
the group reports.

To register a report to a group:

1.  Select **Configuration \> Groups** in *Navigation* pane.

2.  Click **Group Report** for Group.

3.  Click **Add**.
    
    <span>[View the field descriptions for the Group Reports
    page](../Page_Desc/Group_Reports_H.htm)</span>

4.  Select a repository from the **REPOSITORY** list box to indicate
    where the report is located.

5.  Select a report from the **REPORT** list box.
    
    **NOTE:** All reports in the data source are displayed. Select a
    report that is registered to the report repository. Refer to
    [Register Reports to a Report
    Repository](Register_Report_Repositories.htm) for more information.

6.  Click **METRICS** check box to enable it, allowing metrics for the
    group to display under the Dashboard menu.

7.  Click **Save**.

8.  Click **Vertical View** to configure additional fields for the user
    reports.

9.  Click **Edit**.
    
    [View the field descriptions for the Group Reports page's Vertical
    View](../Page_Desc/Group_Reports_H.htm)

10. Enter a schedule in **Schedule Group** field to run large reports in
    a single thread.
    
    **NOTE:** Running a report in a single thread prevents the system
    from being overloaded and allows reports to be built from cache
    tables. It also supports a new concept of building reports from
    Cache Tables to increase performance of a view that contains over 10
    joins on large source tables.

11. Update the **Schedule Priority** field if default value is not
    applicable.
    
     **NOTE:** If running reports in a single thread, the Schedule
    Priority determines the order in which reports are run.  This can be
    used to adjust the order of multithread processing if some reports
    should process first. If Schedule Priority is left blank, reports
    are run in alphabetical order.

12. Click **Save**.
