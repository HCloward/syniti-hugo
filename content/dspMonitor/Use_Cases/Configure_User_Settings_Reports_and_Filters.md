+++
title = 'Configure User Settings, Reports and Filters'
solution = 'Data Quality'
+++

# Configure User Settings, Reports and Filters

Once users are added to a group to gain access to reports, workflow and
report settings can be configured to meet the user’s preference. Some
settings are configured for the group or report, but can be overwritten
at the user level.

This use case covers the following topics:

  - [Customize User Settings](#Customize_User_Settings)

  - [Customize Report Settings](#Customize_Report_Settings)

  - [Define Where Clauses](#Define_Where_Clauses)

  - [Define Filters](#Define_Filters)

## <span id="Customize_User_Settings"></span>Customize User Settings

Users can configure settings specific to their user profile.

To customize user settings:

1.  Select **Configuration \> User Reports/Filters** in the *Navigation*
    pane.
    
    **NOTE:** All users with security to dspMonitor™ display. Refer to
    [Security](../Config/Set_Up_Security_for_dspMonitor) for
    detailed information on granting user security to dspMonitor™.

2.  Click the **Edit** icon for a USER ID row.
    
    [View the field descriptions for the Users Reports/Filters
    page](../Page_Desc/Users_Reports_Filters)

3.  Select an option in the **REPORT HEADER ID** list box if default
    value is not applicable.
    
    **NOTE:** The REPORT HEADER ID controls how the report headers
    display for the user. By default, the reports display the original
    header names, which in most cases are Target ERP header names. A
    user can choose to display the Translated value, leave it
    Untranslated or display both values.
    
    **NOTE**: When a group report is run, dspMonitor™ uses the Group
    Owner’s **Report Header ID** for the unfiltered users’ report. This
    is done because only one copy of the unfiltered report is generated.

4.  Click **SEND ATTACHMENT** check box to enable it, which sends
    reports as an attachment to this user's workflow email.
    
    **NOTE:** If SEND ATTACHMENT is disabled, the user must log in to
    dspMonitor™ to manually download a copy the report.

5.  Click **SEND NOTIFICATION** check box to enable it. The user
    receives a notification when a report has been run.
    
    **NOTE:** If the report contains more records than what is specified
    in the Workflow Attach Record Limit parameter (Configuration \>
    Parameters), a notification is sent instead of the actual report
    file.

6.  Click **SUMMARY NOTIFY** check box to enable it. The user receives a
    single email with all reports for the day instead of receiving an
    individual email for each report.

7.  Click **THRESHOLD NOTIFY** check box to enable it. The user receives
    a group threshold notification workflow for Groups that are at
    critical or warning thresholds.
    
    <span style="font-weight: bold;">NOTE</span>: These check boxes are
    not available if a user does not have a valid email address included
    with the user account information.

8.  Click **Save**.

## <span id="Customize_Report_Settings"></span>Customize Report Settings

Group Owners are able to configure report-level parameters for all
reports registered to their groups. Settings defined at the group level,
such as how frequently workflows are emailed, can be overwritten at the
user level for individual reports.

To customize report settings:

1.  Select **Configuration \> User Reports/Filters** in *Navigation*
    pane.

2.  Click **Reports** for User ID.

3.  Click **Edit**.
    
    [View the field descriptions for the User (Reports)
    page](../Page_Desc/User_Reports_H)

4.  Update the **WORKFLOW SCHEDULE ID** list box to change the frequency
    of workflow emails if the default value is not applicable.
    
    **NOTE:** Schedules are maintained in Common. Refer to [Create
    Schedules](../../../Platform/Common/Use_Cases/Create_Schedules)
    for detailed information.

5.  Click **Save**.

6.  Click **WHERE CLAUSE MANUAL** check box to enable it, indicating a
    Where clause is to be specified for the report.
    
    **NOTE:** A Where clause limits report data displayed to the user
    and overrides user filters. Refer to [Define Where
    Clauses](#Define_Where_Clauses) for detailed information.
    
    **NOTE:** Workflow email settings are controlled at the user level. 

7.  Click **NOTIFY FOR EMPTY REPORTS** check box to enable it, sending a
    workflow email when the report contains no records.
    
    **NOTE:** Reports with zero records are not sent; however, on some
    critical reports, users may like to receive an email if a report
    does not contain records.

8.  Click **Save**.

9.  Click **Vertical View** to further configure the user report.

10. Click **Edit**.
    
    [View the field descriptions for the User (Reports) page's Vertical
    View](../Page_Desc/User_Reports_H)

11. Enter a filter in **Where Clause** field, if **WHERE CLAUSE MANUAL**
    check box is enabled.

12. Enter a sort value in **User Report Order By** field to override the
    SQL Order By field for the user’s specific report file.
    
    **NOTE:** The User Report Order By field is used for users that have
    filters and/or would like the data to display in a specific order.

13. Click **Save**.

## <span id="Define_Where_Clauses"></span>Define Where Clauses

Add a Where clause to a user report if the filtering requirements are
more complex than those supported by the user filter options.

When **Where Clause Manual** is enabled, user filters are ignored and
only the Where clause defined on the
<span style="font-style: italic;">Vertical</span> View of the *[*User
(Reports)*](../Page_Desc/User_Reports_H)* page is used. If the
**Where Clause Manual** field is not enabled, it is assumed that there
is no Where clause and the report is not filtered.

To define a Where clause for a report:

1.  Select **Configuration \> User Reports/Filters** in *Navigation*
    pane.

2.  Click **Reports** for User ID.

3.  Click **WHERE CLAUSE MANUAL** check box to enable it.

4.  Click **Vertical View** for User ID.

5.  Click **Edit**.
    
    [View the field descriptions for the User (Reports) page's Vertical
    View](../Page_Desc/User_Reports_H)

6.  Enter a filter in **Where Clause** field.

7.  Click **Save**.

## <span id="Define_Filters"></span>Define Filters

Filters are customized at the user level to limit data contained in
reports. User filters apply to
**<span class="underline"><span style="color: #ff0000;">all</span></span>**
reports that include the specified field(s) unless otherwise configured.
Multiple values entered for a field display results from a report for
**<span class="underline"><span style="color: #ff0000;">all</span></span>**
values.

To define a filter for a user:

1.  Select **Configuration \> User Reports/Filters** in *Navigation*
    pane.

2.  Click **Filters** for User ID.

3.  Click **Add**.
    
    [View the field descriptions for the User (Filters)
    page](../Page_Desc/User_Filters)

4.  Enter a filter field in **FIELD** field.

5.  Select a value used to filter by constant from **OPERATOR** list
    box.

6.  Enter the value to be compared to FIELD using OPERATOR in
    **CONSTANT** field.

7.  Click **Save**.
