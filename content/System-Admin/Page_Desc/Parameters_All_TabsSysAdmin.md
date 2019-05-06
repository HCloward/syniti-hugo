# Parameters (All Tabs)

<div class="use">

Use this page to:

  - [Mark Target and Source
    Instances](../Use_Cases/Mark_Target_and_Source_Instances.htm)
  - [Configure CTS Passwords](../Use_Cases/Configure_CTS_Passwords.htm)
  - [Configure Authentication
    Settings](../Use_Cases/Configure%20Authentication%20Settings.htm)
  - [Configure Warning Message Timing for License
    Expiration](../Use_Cases/Config_WarnMessage_Lic_Expir.htm)

</div>

This page contains the following tabs:

  - [Site Parameters tab](#Site_Parameters_Tab)
  - [Security Settings tab](#Security_Settings_Tab)
  - [Workflow Parameters tab](#Workflow_Parameters_Tab)
  - [Timeouts tab](#Timeouts_Tab)
  - [Page Parameters tab](#Page_Parameters_Tab)
  - [Search Options tab](#Search_Options_Tab)
  - [Language Support tab](#Language_Support_Tab)
  - [Service Options tab](#Service_Options_Tab)
  - [Naming Conventions tab](#Naming_Conventions_Tab)
  - [System Chart Options](#System_Chart_Options_Tab)
  - [Logging Options](#Logging_Options)

## <span id="Site_Parameters_Tab"></span>Site Parameters tab

Use this tab to:

  - [Mark Target and Source
    Instances](../Use_Cases/Mark_Target_and_Source_Instances.htm)
  - [Set a Default Style for
    Users](../Use_Cases/Set_a_Default_Style_for_Users.htm)

To access this page:

1.  Log in to the DSP®  source instance.

2.  Select **Admin \> Configuration \> Parameters** in
    the *Navigation* pane.

|                                 |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field                           | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Application Name                | Displays name of the application: CranSoft.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Instance                        | Displays the logical application instance (e.g., Dev, QA, Production) that this physical instance of the application represents.                                                                                                                                                                                                                                                                                                                                                                                         |
| Web Site Root                   | Displays URL of the home directory. If the field is not populated, any workflow emails sent that contain links will fail.                                                                                                                                                                                                                                                                                                                                                                                                |
| Email Server                    | Displays outgoing email server name that the Platform uses to send email (e.g., workflow notifications).                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Default Email Address           | Displays email address used when sending a test email (i.e., clicking Test Email button). This email address is also used when the From field on a workflow is not specified AND the current user does not have an email address defined.                                                                                                                                                                                                                                                                                |
| Default Style ID                | Displays the default style that is applied to the site for users that do not have a style specified.                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Default Language ID             | Displays the default language that is applied to the site for users that do not have a language specified.                                                                                                                                                                                                                                                                                                                                                                                                               |
| Test Email                      | Click to send a test email to the current user.                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| License Expiration Warning Days | Displays the number of days prior to license expiration that the user receives a notification of the expiration date.                                                                                                                                                                                                                                                                                                                                                                                                    |
| Clear Cache                     | Click to clear various data caches maintained by the Platform from the time of its last startup. These caches exist to aid performance, but can become “stale” due to errors or database operations that can cause issues, such as newly created views not showing up in page design lists or new WebApps not showing up on the Site menu. These issues are often stale cache problems that can be fixed by using the Clear Cache button, which avoids the need to restart the Platform or obtain additional assistance. |

## <span id="Security_Settings_Tab"></span>Security Settings tab

Use this tab to:

  - [Configure Password
    Options](../Use_Cases/Configure_Password_Options.htm)
  - [Configure Authentication
    Settings](../Use_Cases/Configure%20Authentication%20Settings.htm)

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Maximum Password Age</p></td>
<td><p>Displays number of days before user account passwords expire. Enter 0 for the password to never expire. Default value is 30 days.</p></td>
</tr>
<tr class="odd">
<td><p>Support Anonymous</p></td>
<td><p>If enabled, anonymous users can access the Platform. When an anonymous user first enters the Platform, instead of a login page, the user is automatically logged in as an anonymous user. A user is <em>anonymous</em> when the Anonymous checkbox is enabled for the user (Security &gt; Users).</p></td>
</tr>
<tr class="even">
<td><p>Support Basic Authentication</p></td>
<td><p>If enabled, only Platform user IDs are used to log into the Platform. No reference to corporate system user IDs is used.</p></td>
</tr>
<tr class="odd">
<td><p>Support Integrated Authentication</p></td>
<td><p>If enabled, corporate system user IDs are permitted by the Platform. For example, after a user has successfully been authenticated by the corporate system and logged into a computer, the Platform can be started without an additional login. This requires: 1) IIS Enable Anonymous Access is disabled, 2) IIS Integrated Windows Authentication is enabled, and 3) Platform User ID includes the user’s corporate ID (as entered in the Windows User Name field on the <span style="font-style: italic;">Users</span>page's Vertical View). The Platform uses the corporate ID and cross-references it with the local Platform ID.</p></td>
</tr>
<tr class="even">
<td><p>Integrated Authentication Variable Name</p></td>
<td><p>Displays variable used to authenticate the user by User ID. Support Integrated Authentication must be enabled.</p></td>
</tr>
<tr class="odd">
<td><p>Support Custom Authentication</p></td>
<td><p>If enabled, the CustomAuthentication.dll is used to authenticate the user. This library is not shipped by BackOffice and allows the client to define any authentication routine they choose.</p></td>
</tr>
<tr class="even">
<td><p>Support Workflow Authentication</p></td>
<td><p>If enabled, workflow messages contain disclaimer text to inform the email recipient that any user who clicks the workflow link is automatically authenticated based on the email recipient’s user account. Users are automatically logged into the DSP when the workflow link is clicked.</p>
<p>If disabled, users who click the workflow link must log into the DSP.</p>
<p>It is checked by default.</p></td>
</tr>
<tr class="odd">
<td><p>Secure URL</p></td>
<td><p>Displays SSL URL to which the Platform directs the user when Force Secure Connection is enabled.</p></td>
</tr>
<tr class="even">
<td><p>Force Secure Connection</p></td>
<td><p>If enabled, the site automatically redirects to the HTTPS protocol, securing the transmission of data between the client and the web server. This selection requires that an SSL certificate is installed on the web server.</p></td>
</tr>
<tr class="odd">
<td><p>CTS Password</p></td>
<td><p>Displays masked password used to secure the connection between two Platform instances when exporting a CTS package.</p></td>
</tr>
<tr class="even">
<td><p>Maximum Login Attempts</p></td>
<td><p>Displays number of login attempts before the user ID is locked and is therefore unable to log in to the DSP®.</p></td>
</tr>
<tr class="odd">
<td><p>Login Attempt Lockout Period</p></td>
<td><p>Displays number of minutes to wait before user can re-try to login after password lockout is activated. Default value is 300 minutes.</p></td>
</tr>
<tr class="even">
<td><p>Disable Inactive User Period</p></td>
<td><p>Displays the number of days a user account will remain active if the user has not authenticated, i.e., logged in. Once the period has passed, the user account is set to inactive. The user cannot log in until the account is unlocked by an Administrator. For example, the Disable Inactive User Period is set to 10. The user TJones is added in the platform, but does not log in for 10 days. The user account for TJones is set as inactive.</p></td>
</tr>
<tr class="odd">
<td><p>Min Password Length</p></td>
<td><p>Displays minimum password length accepted for new or changed passwords. Zero allows any password length. Default value is 0.</p></td>
</tr>
<tr class="even">
<td><p>Password Require Alpha</p></td>
<td><p>If enabled, users' passwords to log in to the DSP® require an alpha character.</p></td>
</tr>
<tr class="odd">
<td><p>Password Require Numeric</p></td>
<td><p>If enabled, users' passwords to log in to the DSP® require a numeric value.</p></td>
</tr>
<tr class="even">
<td><p>Password Require Special</p></td>
<td><p>If enabled, users' passwords to log in to the DSP® require a special character.</p></td>
</tr>
<tr class="odd">
<td><p>Password History</p></td>
<td><p>Displays the number of user passwords retained. During the password rename process, the Platform compares history names – no duplicates are allowed.  Zero retains no passwords except current one. Default value is 0.</p></td>
</tr>
<tr class="even">
<td><p>Suppress User ID</p></td>
<td><p>If enabled, the current user’s ID does not display in various places where it would normally display (for example on the <em>Electronic Signature</em> page or when the use hovers over the Gear icon on the Toolbar).</p></td>
</tr>
</tbody>
</table>

## <span id="Workflow_Parameters_Tab"></span>Workflow Parameters tab

|                                    |                                                                                                                                       |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| Field                              | Description                                                                                                                           |
| Workflow Continue On Error         | If enabled, the Platform does not fail events due to SMTP errors that occur when sending workflows. Errors can be viewed in the logs. |
| Workflow Log Retention Days        | Displays number of days that records in the User Workflow Log are retained. Default value is 2 days.                                  |
| Default Workflow Expire Days       | Displays number of days a workflow link is active for the receiver of the email. Default value is 14 days.                            |
| Maximum Email Attachment File Size | Displays the maximum file size (in bytes) allowed for email attachments. Default value is 5000000 bytes.                              |

## <span id="Timeouts_Tab"></span>Timeouts tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Session Timeout</p></td>
<td><p>Displays the number of minutes with no activity from the logged in user before the session times out. Once the minutes have passed, the session ends and the user is logged out. For example, the Session Timeout is set to 5 minutes. A user navigates in the DSP for 2 hours then stops using the keyboard and mouse. After 5 minutes, the user is logged out. Recommended default is 20 minutes.</p>
<p><strong>NOTE</strong>: When a user re-authenticates, i.e., logs back in, the page the user was on when the session timed out displays, if that page is available.</p></td>
</tr>
<tr class="odd">
<td><p>Request Timeout</p></td>
<td><p>Displays number of seconds before request times out. This field represents the time for a web page to render the results after a request. Recommended default is 30 seconds.</p></td>
</tr>
<tr class="even">
<td><p>Full Page Record Lock Timeout</p></td>
<td><p>Displays time (in seconds) that a page is locked when full page edit mode is invoked. When a user edits a record, a lock icon displays to all other users, preventing them from modifying records on the page. The recommended default is 1200 seconds.</p></td>
</tr>
<tr class="odd">
<td><p>Record Lock Timeout</p></td>
<td><p>Displays time (in seconds) that a record is locked when being edited. When a user edits a record, a lock icon displays to all other users, preventing them from modifying the record. Default value is 90 seconds.</p></td>
</tr>
</tbody>
</table>

## <span id="Page_Parameters_Tab"></span>Page Parameters tab

Field

Description

Records Per Page

Displays number of records per page before additional pages are added.
Default value is 16 pages.

Maximum Hint Length

Feature is deprecated.

Number Of Page Range Characters

Displays number of characters to include in the range portion of the
page selection menu. Enter 0 to use the entire field. Recommended value
is 3.

Page Trace Retention Days

Displays the number of days in which trace logs are retained. After the
retention days are reached, the trace logs are deleted from the
Platform. Default value is 5 days.

Quick Panel Resource Allocation

Displays the number of milliseconds of processing time allocated,
per-second, for each Quick Panel Resource. This can be used in
conjunction with the Quick Panel Performance Monitor to balance server
performance versus Quick Panel count refresh frequency.

**NOTE:** This field is not relevant to Bulk Execution or Excel
Integration.

Bulk Execution Limit

Displays the number of records which a user can Bulk Execute against on
any page. If this value is exceeded, a message will be displayed to
indicate the result set needs to be filtered to reduce the number of
records visible before a Bulk Execution can be performed. This is to
reduce load on the server when under load while remaining highly
responsive while not under heavy usage. Note: Serialized events will
always run in 1 thread.

**NOTE:** This is the number of concurrent threads that can process Bulk
Execution logic. Each invocation of Bulk Execution will use half of the
remaining threads with a minimum of 1.

Bulk Execution Thread Limit

Displays the number of multi-threads available for the use of Bulk
Execution. When performing a Bulk Execution, if asynchronicity is
supported, half of the available threads will be allocated for the job.
Meaning, if the limit is 32, the first Bulk Execution will be given 16
threads. If another Bulk Execution is invoked during this, it will be
allocated 8, and so on. There will always be at least 1 thread granted
to ensure the job is processed.  
  
This logarithmic trend is to ensure the Server processes as quickly as
possible during low usage and can distribute load when under heavy
usage.

Excel Import Record Limit

Displays the maximum number of records that can be inserted per
worksheet upload. This may be useful when page designers know that
either the OnValidate event is very resource intensive or the data set
can be very dense.

Auto Refresh

Auto Refresh Min

Displays minimum or starting refresh rate in seconds. Default value is
999 seconds.

Auto Refresh Max

Displays maximum or ending refresh rate in seconds. Default value is 30
seconds.

Auto Refresh Increment

Displays number of seconds to increment the refresh rate until the Auto
Refresh Max is reached. Default value is 5
seconds.

## <span id="Search_Options_Tab"></span>Search Options tab

|                                  |                                                                                                                                                                                                                                                   |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                            | Description                                                                                                                                                                                                                                       |
| Display Record Limit             | Displays number of records available in a web view before the filter option is activated.  Recommended value is 1000.                                                                                                                             |
| Download Record Limit            | Displays number of records allowed in a download before the filter option is activated.  Recommended value is 10000.                                                                                                                              |
| Report Record Limit              | Displays number of records displayed in a report before the filter option is activated.  Recommended value is 1000.                                                                                                                               |
| List Record Limit                | Displays upper limit on the number of records that can be displayed in a list box. If this limit is reached, the list box reports an error and fails to populate. The Designer should change the column to use a combo box instead of a list box. |
| Full Page Edit List Record Limit | This feature is obsolete. Refer to List Record Limit.                                                                                                                                                                                             |
| Search String Wildcard           | Displays wildcard character used when performing text-based searches. Default value is \*.                                                                                                                                                        |
| Default Search Word Limit        | Displays number of words to index out of each column during search indexing. Default value is 64.                                                                                                                                                 |

## <span id="Language_Support_Tab"></span>Language Support tab

|                      |                                                                                                                                                                                                               |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                | Description                                                                                                                                                                                                   |
| System Catalog ID    | Displays custom catalog name used throughout the DSP® for all translations. In typical page translation, this is the lowest priority catalog. In Platform translations, this is the highest priority catalog. |
| Support Translation  | If enabled, the Language field is available on the <span style="font-style: italic;">Settings</span> page, providing users with the option of selecting the language that is used for their session.          |
| Support Localization | If enabled, the Locale field is available on the <span style="font-style: italic;">Settings</span> page, providing users with the option of selecting the local that is used for their session.               |

## <span id="Service_Options_Tab"></span>Service Options tab

|                               |                                                                                                                                                           |
| ----------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                         | Description                                                                                                                                               |
| Service User ID               | Displays Platform user ID that the service uses to log into the Platform.                                                                                 |
| Service Record Limit          | Displays number of records on which the service page operates. If this record count is exceeded, the service page is not executed and an error is logged. |
| Default Queue ID              | Displays the default queue to be used in background events.                                                                                               |
| Default Service Page Queue ID | Displays the default queue to be used by service pages.                                                                                                   |

## <span id="Naming_Conventions_Tab"></span>Naming Conventions tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Table Filter</p></td>
<td><p>Displays filter applied in the table combo box when selecting a table. Default value is * indicating there is no filter for a table name.</p></td>
</tr>
<tr class="odd">
<td><p>Horizontal Filter</p></td>
<td><p>Displays filter used to reduce the number of elements shown in <em>Horizontal</em> View combo boxes.  Default value is <strong>web*Hor</strong>, where the view name begins with “Web” and ends with “Hor.”  </p>
<p><em>Horizontal</em> Views must be named in the database following this naming convention or they do not display as options in combo boxes in the DSP®.</p></td>
</tr>
<tr class="even">
<td><p>Vertical Filter</p></td>
<td><p>Displays filter used to reduce the number of elements shown in Vertical View combo boxes. Default value is <strong>web*Ver</strong>, where the view name begins with “Web” and ends with “Ver.”</p>
<p><em>Vertical</em> Views must be named in the database following this naming convention or they do not display as options in combo boxes in the DSP®.</p></td>
</tr>
<tr class="odd">
<td><p>Report Filter</p></td>
<td><p>Displays filter used to select views shown in report page views. The default registered value is <strong>usr*</strong>, where the view name begins with “user” and the remaining text may be any character.</p>
<p>Report views must be named following this naming convention or they do not display in the DSP®.</p></td>
</tr>
<tr class="even">
<td><p>Chart Filter</p></td>
<td><p>Displays filter used to select views shown in chart page views. The default registered value is <strong>web*Chart</strong>.</p>
<p>Chart views must be named following this naming convention or they cannot be selected when adding a chart in the DSP®.</p>
<p>Refer to <a href="../../WebApp_Dev/Create_a_Chart.htm">Add a Chart</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>List Filter</p></td>
<td><p>Displays filter used to reduce the number of elements shown in Value fields or the Descriptive fields when building a list box with Column Properties.  Default value is <strong>web*List</strong>, where the view name begins with “Web” and ends with “List.”</p>
<p>Refer to <a href="../../WebApp_Dev/Add_List_Boxes_and_Combo_Boxes.htm">Add List Boxes and Combo Boxes</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>System List Filter</p></td>
<td><p>Displays the filter used to reduce the number of elements shown in search combo box. The default registered value is web*Search, where the view name begins with &quot;Web&quot; and ends with &quot;Search&quot;.</p></td>
</tr>
<tr class="odd">
<td><p>Procedure Filter</p></td>
<td><p>Displays filter used to help identify procedures.  Default value is <strong>web*</strong>, where the filter name begins with “web&quot; and the remaining text may be any character. Due to the complexity in naming a procedure, only the prefix is defined.</p></td>
</tr>
<tr class="even">
<td><p>Validation Filter</p></td>
<td><p>Displays filter used to reduce the number of elements shown in Validation combo boxes. Default value is <strong>web*Val</strong>, where the view name begins with “Web” and ends with “Val.”</p>
<p>Refer to <a href="../../WebApp_Dev/ValidationRules.htm">Register a Validation Rule</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Workflow Filter</p></td>
<td><p>Displays filter used to reduce the number of elements shown in workflow combo boxes. Default value is <span style="font-weight: bold;">web*Flow</span>, where the view name begins with “Web” and ends with “Flow.”</p>
<p>Refer to <a href="../Use_Cases/Register_Workflow_Views.htm">Register Workflow Views</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Event Parameter Filter</p></td>
<td><p>Displays filter used to select views applicable to event parameters. Default value is <strong>web*Evt</strong>, where the filter begins with &quot;web&quot; and ends with &quot;Evt.&quot;</p></td>
</tr>
<tr class="odd">
<td><p>Defaults Filter</p></td>
<td><p>Displays filter used to define the naming convention for Default Views, and is used to populate the Default View list box on the Pages page. Default value is <strong>web*Def,</strong> where the filter begins with &quot;web&quot; and ends with &quot;Def.&quot;</p></td>
</tr>
<tr class="even">
<td><p>Search Filter</p></td>
<td><p>Displays filter used to reduce the number of elements shown in search combo boxes. Default value is <span style="font-weight: bold;">web*Search</span>, where the view name begins with “Web” and ends with “Search.”</p></td>
</tr>
<tr class="odd">
<td><p>Index Filter</p></td>
<td><p>Displays filter to search registered table names. Default value is <strong>*#Search</strong>, where * is a wildcard prefix. For each search initiated, the table selected becomes the prefix, e.g., Employee table search = Employee#search. During user selection, table is populated with records and indexed.</p></td>
</tr>
<tr class="even">
<td><p>Service Filter</p></td>
<td><p>Displays filter used to select views for service pages. Default value is <strong>web*Ser</strong>, where the filter begins with &quot;web&quot; and ends with &quot;Ser.&quot;</p></td>
</tr>
<tr class="odd">
<td><p>Hover Filter</p></td>
<td><p>Displays filter used to define the naming convention for Hover Views, and is used to populate the HoverView list box on the Pages page. Default value is <strong>web*Hov</strong>, where the filter begins with &quot;web&quot; and ends with &quot;Hor.&quot;</p></td>
</tr>
<tr class="even">
<td><p>User Control Filter</p></td>
<td><p>Displays filter used to define the naming convention for User Control Views, and is used to populate the User Control View list box on the <span style="font-style: italic;">Pages</span> page in System Administration (on the Vertical View &gt; Control Views tab, where the Page Type is &quot;Dynamic&quot;). Default value is <strong>web*Ucv</strong>, where the filter begins with &quot;web&quot; and ends with &quot;Ucv.&quot; </p>
<p>Refer to <a href="../../WebApp_Dev/User_Control_Views.htm">User Control Views</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Page Control Filter</p></td>
<td><p>Displays filter used to define the naming convention for Page Control Views, and is used to populate the Page Control View list box on the <span style="font-style: italic;">Pages</span> page  in System Administration (on the Vertical View &gt; Control Views tab, where the Page Type is &quot;Dynamic&quot;). Default value is <strong>web*Pcv</strong>, where the filter begins with &quot;web&quot; and ends with &quot;Pcv.&quot;</p>
<p>Refer to <a href="../../WebApp_Dev/Page_Control_View.htm">Page Control Views</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Data Control Filter</p></td>
<td><p>Displays filter used to define the naming convention for Data Control Views, and is used to populate the Data Control View list box on the <span style="font-style: italic;">Pages</span> page  in System Administration (on the Vertical View &gt; Control Views tab, where the Page Type is &quot;Dynamic&quot;). Default value is <strong>web*Dcv</strong>, where the filter begins with &quot;web&quot; and ends with &quot;Dcv.&quot;</p>
<p>Refer to <a href="../../WebApp_Dev/Data_Control_Views.htm">Data Control Views</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>List Control Filter</p></td>
<td>Displays filter used when selecting list control views. Default value is <strong>web*Lcv</strong>, where the filter begins with &quot;web&quot; and ends with &quot;Lcv.&quot;</td>
</tr>
<tr class="even">
<td><p>Parameter Filter</p></td>
<td><p>Displays filter used when selecting page parameter views. Default value is <strong>web*PV</strong>, where the filter begins with &quot;web&quot; and ends with &quot;PV.&quot;</p></td>
</tr>
<tr class="odd">
<td><p>Tooltip Filter</p></td>
<td><p>Displays filter used when using the tooltip feature.</p>
<p>Refer to <a href="../../WebApp_Dev/Add_a_Tooltip.htm">Add a Tooltip</a> for more information.</p>
<p><strong>NOTE:</strong> This field is hard coded to limit the number of characters displayed to 32.</p></td>
</tr>
<tr class="even">
<td><p>Watermark Filter</p></td>
<td><p>Displays filter used when using the watermark feature.</p>
<p>Refer to <a href="../../WebApp_Dev/Add_a_Watermark.htm">Add a Watermark f</a>or more information.</p></td>
</tr>
<tr class="odd">
<td><p>Control View Field Prefix</p></td>
<td><p>Field is deprecated.</p></td>
</tr>
</tbody>
</table>

## <span id="System_Chart_Options_Tab"></span>System Chart Options tab

|                     |                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------- |
| Field               | Description                                                                             |
| Metric Report Hours | Displays the number of hours to display on the hourly reports in System Administration. |
| Metric Report Days  | Displays the number of daysto display on the daily reports in System Administration.    |

## <span id="Logging_Options"></span>Logging Options tab

Use this tab to [Log Events and Access to Personal
Data](../Use_Cases/Log%20Events%20and%20Access%20to%20Personal%20Data.htm).

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Enable Page Logging</p></td>
<td><p>Click to turn on logging of all events. The logs are created daily as .CSV files.</p></td>
</tr>
<tr class="odd">
<td><p>Disable Page Logging</p></td>
<td><p>Click to stop logging all events in the DSP.</p></td>
</tr>
<tr class="even">
<td><p>Logging Retention Days</p></td>
<td><p>Displays the number of days logs are kept before they are deleted.</p>
<p>The default value, 0, indicates that the logs will never be deleted.</p>
<p>These logs track all events related to personal data, and are written to the data source configured by the user in the Logging Data Source ID field.</p></td>
</tr>
<tr class="odd">
<td><p>Logging Data Source ID</p></td>
<td><p>Displays the data source where logs are written.</p>
<p><strong>NOTE:</strong> Though this data source's path can be local on the web server or on a network, it is highly recommended that the logs be stored on a remote server.</p></td>
</tr>
<tr class="even">
<td><p>Enable Logging By Page</p></td>
<td><p>Click to open the <em><a href="../Use_Cases/Enable%20Logging%20By%20Page.htm">Enable Logging By Page</a></em> page to enable or disable logging for specific pages.</p></td>
</tr>
<tr class="odd">
<td><p>Download Most Recent Log File</p></td>
<td><p>Click to download the log file for the current day.</p></td>
</tr>
</tbody>
</table>
