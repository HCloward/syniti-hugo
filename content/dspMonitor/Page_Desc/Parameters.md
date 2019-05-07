+++
title = 'Parameters'
solution = 'Data Quality'
+++

# Parameters

Use this page to [Configure dspMonitor™
Parameters](../Config/Configure_dspMonitor_Parameters.htm).

<div class="use">

This page contains the following tabs:

  - [General tab](#General_Tab2)
  - [Metric Parameters tab](#Metric_Parameters_Tab)
  - [Workflow Parameters tab](#Workflow_Parameters_Tab)
  - [Misc Parameters tab](#Misc_Parameters_Tab)

</div>

To access this page, select **dspMonitor \> Configuration \>
Parameters** in *Navigation* pane.

### <span id="General_Tab2"></span>General tab

Field

Description

Application Information

Application Name

Displays name of DSP® component: dspMonitor™.

Version

Displays current version of DSP component.

Date

Displays date when DSP component was released.

Properties

Report Directory Path

Displays path on the file system (NOT the root of a disk drive) where
reports are stored.

Report Autogenerate Size

Displays unique value limit for a field, so when the unique value count
is less than or equal to this limit, the report is automatically
generated. Default value is **50,000**.

Workflow Attach Record Limit

Displays report threshold size to determine when a workflow link to a
report is emailed instead of the actual report file. Default value is
**20,000**.

Zip Record Count

Displays minimum number of rows a report must contain in order to be
automatically zipped before it is attached to the workflow message. If
the report does not exceed this record count, the file is not zipped.
Default is **30,000**.

Zip Delete Original File

If enabled, original report is deleted from the file system after it’s
zipped.

Keep File Duration

Displays number of days a file is kept on the file system before it is
automatically deleted. Default value is **60**.

Default Report Filter

Displays report filter used by default when registering reports to a new
report repository.

Default Opportunity View Filter

Displays the view that filters the selection options in Opportunity View
list box on the *[Repository Reports](Repository_Reports_H.htm)* page.

**NOTE:** The recommended value is tv\*OptSel. If this value is entered,
when configuring reports on the *[Repository
Report](Repository_Reports_H.htm)* page, only views that follow the
naming convention of tv\*OptSel are available to choose as an
Opportunity View from the drop down list.

Default Output File Type

Displays type of file generated for reports. Values are: File Excel and
File Delimited. Default value is **File Excel**.

Default Output Delimiter

Displays default extension (as in, type of Excel file) for generated
reports.

Build Xlsx Reports

If checked, reports are generated using Excel 2007 and higher. If
unchecked, reports are generated using Excel 97-2003. The **Default
Output File Type** must be set to **File Excel** in order for **Build
Xlsx Reports** to be used.

Remove Date From File Path

If checked, one copy of the report is stored for each user. If
unchecked, a folder is created for reports and a file is generated for
each date for each user. Check this field to control disk space usage
when there are many users with large reports. Default value is Disabled.

Delete Cache For Manual Rpts

If enabled, Cache Tables are deleted and rebuilt based on information
provided in the report view. This feature is useful to provide users
with real-time reporting of the most recent information when groups of
reports or individual reports are manually processed. Default value is
Disabled.

Process Filter Background

If checked, filters are processed in the background to increase
performance when creating Groups (Configuration \> Groups).

Cache Database Name Suffix

Displays the suffix used for cache databases. Default value is
**\_Cache**.

### <span id="Metric_Parameters_Tab"></span>Metric Parameters tab

Use this tab to:

  - [Register Data Quality Score
    Thresholds](../Use_Cases/Populate_Configuration_Tables.htm#Register_Data_Quality_Score_Thresholds).
  - [Customizing Group Metric
    Graph](../Use_Cases/Populate_Configuration_Tables.htm#Customize_Group_Metric_Graph)
  - [Use Data Quality
    Dashboard](../Use_Cases/Use_Data_Quality_Dashboard.htm)
  - [Configure the Business Value
    Dashboard](../Use_Cases/Configure_the_Business_Value_Dashboard.htm)

Field

Description

Metrics Settings

Display Metrics Duration

Displays number of days report metrics are displayed in dspMonitor™. 

Keep Metrics Duration

Displays number of days report metrics are stored in the database. This
value also displays the maximum number of days metrics could potentially
display in dspMonitor. Default value is **365**.

Keep Metrics Data Duration

Displays number of days to maintain report metrics after an error has
been corrected on the report. Default value is **20**.

Keep Workflow Duration

Displays number of days to maintain workflow history. Default value is
**20** days.

Metric Report Day

Displays number of days that display on the Report Day (Metrics) report.
Default value is **10**.

Metric Report Week

Displays how many weeks display on the Report Week (Metrics) report.
Default is **5**.

Metric Report Month

Displays how many months display on the Report Month (Metrics) report.
Default is **12**.

Graph Directory Path

Displays the path file to store the Excel report on the
<span style="font-style: italic;">Group Metric Graph</span> page. The
path must be a valid directory on the WebApp server and is the same
location where DSP® is stored.

Data Quality Scoring Threshold

Enable Sigma Level

If checked, sigma levels are displayed to the user in the threshold list
box options on any page that contains a Threshold ID field. The list box
will also contain Critical and Warning percentage values. In addition,
the Sigma Level based on data quality score calculation is display on
the *Your Groups*, *Your Objects*, and *Your Targets* summary and report
pages.

If unchecked, sigma levels are not displayed on any page that contains a
Threshold ID field. Only percentage values are displayed for Critical
and Warning values. Sigma Level is not displayed on the *Your Groups,
Your Objects*, and *Your Targets* summary and report pages.

Whether checked or unchecked, the threshold list box options are
supplied from the thresholds that have been created on the *Data Quality
Score Thresholds* page.

Refer to [Register Data Quality Score
Thresholds](../Use_Cases/Populate_Configuration_Tables.htm#Register_Data_Quality_Score_Thresholds)
for more information.

Threshold ID

Displays the threshold ID used for data quality scoring. An initial
default threshold is supplied at the Parameters level. The default
Threshold ID may be changed to any custom threshold. Custom thresholds
are added on the *Data Quality Score Thresholds* page. Refer to
[Register Data Quality Score
Thresholds](../Use_Cases/Populate_Configuration_Tables.htm#Register_Data_Quality_Score_Thresholds)
for more information.

Business Value Parameters

 

Currency

Displays the currency used in the Cost per Failure calculations on the
Business Value dashboard.

**NOTE:** If this field is updated, calculations at the report level are
not automatically updated. A user must manually update the Cost Per
Failure value set at the report level.

### <span id="Workflow_Parameters_Tab"></span>Workflow Parameters tab

Use this tab to [Configure Workflow
Content](../Use_Cases/Manage_Workflow_Emails.htm#Configure_Workflow_Content).

Field

Description

Workflow Content

Subject

Displays subject line of email notifications.

Email From

Displays email address from which email notifications are sent.

Email Attachment Body

Displays email body template for workflow emails with attachments. Do
not change any values with a \# prefix and suffix (for example,
\#SWAPNAME\#). 

Email Notification Body

Displays email body template for workflow emails sent as notifications.
Do not change any values with a \# prefix and suffix (for example,
\#SWAPNAME\#). 

Email Summary Body

Displays email body template for workflow summary emails. Do not change
any values with a \# prefix and suffix (for example, \#SWAPNAME\#). 

Email Empty Body

Displays email body template for workflow emails sent as notifications
for empty reports. Do not change any values with a \# prefix and suffix
(for example, \#SWAPNAME\#). 

Table Header

Displays HTML for table header row in workflow emails that contain a
summary table.

Table Line

Displays HTML for each summary report line within workflow emails that
contain a summary table.

Email Threshold Body

Displays email body template for threshold workflow emails sent as
notifications. Do not change any values with a \# prefix and suffix (for
example, \#SWAPNAME\#).

Threshold Table Header

Displays HTML for table header row in threshold workflow emails that
contain a summary table.

Threshold Table Line

Displays HTML for each summary report line within threshold workflow
emails that contain a summary table.

Odd Row BG Color

Displays color code for background of odd rows on the summary report.

Even Row BG Color

Displays color code for background of even rows on the summary report.

### <span id="Misc_Parameters_Tab"></span>Misc Parameters tab

Use this tab to [Configure SAP Client Name for dspMonitor™
Reports](../Config/Configure_SAP_Client_Name_for_dspMonitor_Reports.htm).

Field

Description

SAP Parameters

SAP Client

Displays name of SAP client in which dspMonitor™ interacts. Default
value is **0**, which must be updated before reports can be processed.

SAP Language

Displays language used when SAP interfaces with dspMonitor. Default
value is **E** (English).

Dashboard

Max Report Count

Displays the acceptable number of error records for reports listed on
the dashboard pages for the Status to be green. Default value is 10.

Report Parameters

Max AUSCH

Displays the maximum component of scrap (in percent) allowable on a Bill
of Material. Default value is **0**.

Min Mat Desc

Displays the minimum length of a material description for the
description to be considered valid. Default value is **4**.

Min Cust Name

Displays the minimum length of a customer name for the description to be
considered valid. Default value is **4**.

Min Vend Name

Displays the minimum length of a vendor name for the description to be
considered valid. Default value is **4**.
