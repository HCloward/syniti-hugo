# View Reports

Business users view their migration reports on the Report Delivery
pages.

An Administrator must
<span id="User Report Access" class="popUpLink">grant a user
access</span> to the Report Delivery pages. The following reports are
available on the Report Delivery pages:

  - [All Reports](../Page_Desc/All_Reports.htm)
  - [Target All Errors
    Report](../Page_Desc/Target_All_Errors_Report.htm)
  - [All Business Reports - All Waves/Process
    Areas](../Page_Desc/All_Business_Reports_All_Wave_Process_Areas.htm)
  - [All Actionable Reports](../Page_Desc/All_Actionable_Reports.htm)

This section contains the following topics.

  - [View All Reports](#View_All_Reports)
  - [View all Reports for an Object, Target or
    Source](#View_all_Reports_for_an_Object_Target_or_Source)
  - [View the Target All Errors
    Report](#View_the_Target_All_Errors_Report)
  - [View All Reports Across Waves and Process
    Areas](#View_All_Reports_Across_Waves_and_Process_Areas)
  - [View Actionable Reports and Historical Record
    Count](#View_Actionable_Reports_and_Historical_Record_Count)

## <span id="View_All_Reports"></span>View All Reports

A user can view all reports to which they have access on the *[All
Reports](../Page_Desc/All_Reports.htm)* page.

To view all reports and their contents in Transform:

1.  Select **My Reports \> All Reports** in the *Navigation* pane.

2.  Click the **All Reports** icon for an Object.

3.  Select the report and click the **Access Report** icon to view the
    records.

4.  Click **View Report**.
    
    **NOTE:** If the View Report icon is disabled, click the **Access
    Report** icon to activate it. Clicking the Access Report icon
    assigns the current date and time to the GENERATED field. The
    PUBLISHED date and time must precede the GENERATED date and time so
    that the contents can be viewed.
    
    **NOTE:** A user cannot see the contents of a report if it is a
    sensitive report and all access has not been granted to the user. In
    this case, the View Report and Download a file icons are inactive.
    The View Report and Download a file icons are in sync with each
    other. When one is inactive, the other is inactive.

**NOTE:** All reports that the user is assigned to are displayed in
PRIORITY sort order with Critical being at the top.

**NOTE:** The user can drill down through the *[All
Reports](../Page_Desc/All_Reports.htm)* page (by object) to see report
groupings by Targets and
Sources.

## <span id="View_all_Reports_for_an_Object_Target_or_Source"></span>View all Reports for an Object, Target or Source

A Business user can view reports grouped by object, target or source.

To view all reports for an object in Transform, click **My Reports \>
All Reports** in the *Navigation* pane.

To view all reports for a target, click the **Targets** icon for an
object on the *[All Reports (By
Object)](../Page_Desc/All_Reports_By_Object.htm)* page.

To view all reports for a source, click the **Sources** icon on the [All
Reports (By Target)](../Page_Desc/All_Reports_By_Target.htm)
page.

## <span id="View_the_Target_All_Errors_Report"></span>View the Target All Errors Report

The Target All Errors report (sometimes called the Summary Report) is a
summary of errors on a target.

The report is not registered but is automatically generated, and
aggregates the primary key information from every error report (Error,
Target Readiness and Business Readiness report types) that is registered
to the target.

There is one Target All Errors report per target.

**NOTE:** If a report does not contain primary key information, no data
from that report displays on the Target All Errors report.

To view the Target All Errors Report for an object in Transform:

1.  Select **My Reports \> All Reports** in the *Navigation* pane.
2.  Click the **Errors By Target** icon.
3.  Click the **Generate Report** icon for the desired Wave.
4.  Click the **View Target All Errors Report** icon.

To view the Target All Errors Report for a target in Transform:

1.  Select **My Reports \> All Reports** in the Navigation pane.
2.  Click the **Targets** icon.
3.  Click the **Errors By Target** icon.
4.  Click the **Generate Report** icon for the desired Wave.
5.  Click the **View Target All Errors Report**
icon.

## <span id="View_All_Reports_Across_Waves_and_Process_Areas"></span>View All Reports Across Waves and Process Areas

Users can view all the reports that they are assigned to across waves
and process areas.

An Administrator must
<span id="User Report Access" class="popUpLink">grant a user
access</span> to the Report Delivery pages.

To view the *[All Business Reports – All Wave/Process
Areas](../Page_Desc/All_Business_Reports_All_Wave_Process_Areas.htm)*
page:

1.  Select **My Reports \> All Business Reports (All Wave/Process
    Areas)** in the *Navigation* pane.

2.  Click the **Access Report** icon for a report to generate the latest
    version.
    
    **NOTE:** Clicking the Access Report icon generates the latest
    version of the report and updates the GENERATED field. For the
    report to display, the PUBLISHED date and time must precede the
    GENERATED date and time.

3.  Click the **View Report** icon to view the records.

4.  Click the **Download a File** icon to download the report in .xlsx
    format.
    
    **NOTE:** A user cannot see the contents of a report if it is a
    sensitive report and all access has not been granted to the user. In
    this case, the View Report and Download a file buttons will be
    disabled. The View Report and Download a file buttons are in sync
    with each other, when one is disabled the other is
disabled.

## <span id="View_Actionable_Reports_and_Historical_Record_Count"></span>View Actionable Reports and Historical Record Count

Actionable reports are reports that represent errors. The report types
included in the actionable reports list are: *Business Readiness*,
*Target Readiness* and *Error*. The errors in these reports need to be
remedied in order to properly load the data in to the target system.

Non-actionable reports are reports that do not represent errors and have
the report type of *Business Relevancy*, *Info* and *Pre Load*.

To view all actionable reports in Transform:

1.  Select **My Reports \> All Reports** in the *Navigation* pane.

2.  Click the **Actionable Reports** icon for the desired object.

3.  Click the **Access Reports** icon for a report to generate the
    latest version.
    
    **NOTE:** Clicking the Access Report icon generates the latest
    version of the report and updates the GENERATED field. For the
    report to display, the PUBLISHED date and time must precede the
    GENERATED date and time.
    
    **NOTE:** The Report Run Historical Record Count chart displays the
    record count for each report run (represented by the RunID). The
    last 100 runs are displayed.

4.  Click the **View Report** icon to view the records returned in the
    child pane.
    
    **NOTE:** After a user clicks the View Report icon, the results that
    display contain the records from the most recent report generation.
    After a user clicks the Generate Report icon then the View Target
    All Errors Report icon, the report records display on a page that is
    also named Target All Errors Report. The fields on this page update
    based on the errors on the target reports.

5.  Click the **Download a File** icon to download the report in .xlsx
    format.
    
    **NOTE:** A user cannot see the contents of a report if it is a
    sensitive report and all access has not been granted to the user. In
    this case, the View Report and Download a file buttons will be
    disabled. The View Report and Download a file buttons are in sync
    with each other. When one is disabled the other is disabled.
