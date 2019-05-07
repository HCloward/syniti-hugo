+++
title = 'Parameters
/c/Users/Heather Cloward/Documents/frontMatter/Automate/Page_Desc/Parameters.md:# Parameters'
solution = 'Platform'
+++

# Parameters

<div class="use">

Use this page to [Configure Automate
Parameters](../Use_Cases/Configure_Automate_Parameters.htm).

</div>

To access this page, select **Configuration \> Parameters** in the
*Navigation* pane.

**NOTE:** It is recommended for only developers or system administrators
to edit Automate parameters.

**Field**

**Description**

Application

Displays the name of the application: InterfaceServer.

**NOTE:** Automate is formerly known as InterfaceServer.

Application Version

Displays the version number of the application.

Database Version

Displays the database version that the application is using.

Admin Role

Displays the name of the Admin Role. The email address configured to the
user assigned to the Admin role is used as the From address for the
interface notification emails.

History Retention Days

Displays the number of days the interface instance information is
saved/displayed on the *[Interface History](Interface_History.htm)*
page.

Instance

Displays the instance that all interfaces run against.

**NOTE:** The Instance selected MUST match the Instance field in 2
additional places for email notifications to properly work: on the
*[Role (Instance)](Role_Instance.htm)* page in Automate and on the
*[Parameters](../../Sys_Admin/Page_Desc/Parameters_All_TabsSysAdmin.htm)*
page in System Administration. Refer to [Set Up Notifications for an
Interface](../Use_Cases/Set_Up_Notifications_for_an_Interface.htm) for
more information.

Filter Info 

Workflow Filter

Displays the filter that is used for workflow. The default value is
%workflow.

Stored Procedure Filter

Displays the filter that is used for stored procedures.

Validation Filter

Displays the filter that is used for validation. The default value is
%Val

Logging

Storage Level

Displays lowest level of logging Severity that is written to the
*[Log](Log.htm)* page. For example, with a Storage Level set to
“40-Info,” all logging severities 40 and above are written to the log.

If Debug Mode is enabled for an interface, Storage Level is ignored and
only tasks with severities of Debug and higher are written to the
interfaces *[Log](Log.htm)* page.

Reporting By Importance Level

Displays the severity for which tasks are written to the interface’s
importance *[Log](Log.htm)* (History \> Important). Tasks with the
selected severity and above display in the importance log.

Modules

Click to open the *[Logging Modules](Logging_Modules.htm)* page. Storage
can be configured by module name. For example, by default store only
information, except where module name = ABC, then store starting at the
debug level.

Log Tasks

If checked, start and finish tasks for running events, the interface,
etc. are stored in the interface’s *[Log](Log.htm)* page.

If unchecked, start and finish tasks are not written to the interface’s
*[Log](Log.htm)* page.
