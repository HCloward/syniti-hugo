+++
title = 'Parameters – Collect'
solution = 'Platform'
+++

# Parameters – Collect

<div class="use">

Use this page to [Configure Collect
Parameters](../Use_Cases/Configure_Collect_Parameters.htm).

</div>

To access this page, select <span style="font-weight: bold;">Common \>
Configuration \> Modules \> Parameters-Collect</span> in the
<span style="font-style: italic;">Navigation</span> pane.

This page contains the following tabs:

  - [General tab](#General_Tab2)
  - [General Settings tab](#General_Settings_Tab)
  - [Package Info tab](#Package_Info_Tab)
  - [Data Services Settings tab](#Data_Services_Settings)
  - [DBMoto Settings tab](#DBMoto_Settings_Tab)
  - [Workflow Settings tab](#Workflow_Settings_Tab)

## <span id="General_Tab2"></span>General tab

Field

Description

Application Information

Version

Displays current release version of the component, Collect.

Release Date

Displays date when the component version was released.

Filters

Action Filter

Displays prefix used for action stored procedures. Default value is
**asp%.**

Rule Filter

Displays prefix used for rule stored procedures. Default value is
**ir%**.

Connection Info

Server Name

Displays name of server where application resides

DB2Time Out

Displays time, in milliseconds, for an idle transaction in DB2. Default
value is **180**.

Oracle Time Out

Displays time, in milliseconds, for an idle transaction in Oracle.
Default value is **180**.

SQLSERVER Time Out

Displays time, in milliseconds, for an idle transaction in SQL Server.
Default value is **180**.

## <span id="General_Settings_Tab"></span>General Settings tab

Field

Description

Job Settings

Queue ID

Displays queue used for table downloads when a Collect service is used
to distribute the load on the server. Default value is General.

Recycle Job Max

Displays number of times the download process is recycled. If the job
fails, the table is recycled into the job queue at the end of the
current cycle. This feature is designed to monitor network problems. If
set to 0, the job isn’t recycled. Default value is 3.

Duration Warning Limit

Displays limit (in seconds) for long-running tables. These tables
display in the Duration Warning List report, which is available in
Collect under Reports \> Duration Warning List.

Run Jobs Metrics

Displays a value that captures run and duration times for data downloads
and conversions.

Values are:

  - **No Metrics** – Disables metric process
  - **Build Job Metrics** – Stores duration for the job to complete all
    events
  - **Build Event and Job Metrics** – Stores duration of each event and
    total for the job

Default value is Build Job Metrics.

Job Metrics Retention

Displays number of days to store Table Download Runtime processing data.
Default value is 1 day.

Misc. Settings

Scheduled Downloads

If checked, Collect service jobs run in the background. Default is
Enabled.

Test Source Before Delete

If checked, the ability to log in to the source system is tested before
the current data is deleted and before the creation of the download.
Default value is Enabled.

Max Tracing Count

Displays maximum value of how large the DebugLog table can get before
logging for Collect turns off.

Default Collation Type

Displays the language option for text data in the database.

Values are: General Latin Case-insensitive, General Latin Case-sensitive

Default value is General Latin Case-insensitive, which means the
collation uses Latin characters and is case-insensitive.

Max Record Sources For Union View

Display the threshold for the number of sources that can be registered
for the Record Count on the
*[Tables](../../Collect/Page_Desc/Tables_H.htm)* page’s *Vertical* View
to be calculated.

If the number of sources registered exceeds the threshold set by this
parameter, no Record Count is calculated and the Record Count field on
the *Tables* page’s *Vertical* View is 0.

## <span id="Package_Info_Tab"></span>Package Info tab

Field

Description

General Package Settings

Build Package Default

Displays default setting for building tables. Default value is CranPort.

Package Extension

Displays characters appended to the package name. Default value is
**imp**.

SSIS Settings

Sleep Timer

Displays number of milliseconds to pause before building the next
package. Parameter is used to slow down the build process. Default value
is **100** milliseconds (1 second)

Commit Size

Displays number of records committed in a single SQL Server Transaction
when running table downloads. Default value is **1000**.

SSIS File Path

Displays folder on the component server that stores SSIS packages.

RFC Settings

Rfc Name Space Option

Displays option for RFC name.

Values are:

  - NAMESPACE - uses the namespace version of the BOA Function Module
  - NONNAMESPACE – uses non-namespace version of the BOA Function
    Module.

 

**NOTE:** The namespace concept describes how customers and partners
name their development objects to avoid overlapping when SAP software is
upgraded. BDC Function Modules and BAPI Function Modules can be
namespace or non-namespace objects.

Default value is NONNAMESPACE.

Rfc Type

Displays type of RFC used.

Values are:

  - **SAP RFC** – Uses SAP’s Remote Function Call
  - **BOA RFC** – Uses custom Remote Function Call developed by
    BackOffice
  - **BOA RFC using Options** – Uses custom Remote Function Call
    developed by BackOffice with options applied as a Where Clause to
    limit data read from tables

Default value is BOA RFC.

Rfc Records Per Call

Enter number of records to pull per block from SAP. Default value is
**5000**.

## <span id="Data_Services_Settings"></span>Data Services Settings tab

Field

Description

Datastore Settings

Source Datastore Name Format

Displays the format for a Datastore object created for a source
connection when building a SAP Data Services package. Default value is
**\#SOURCE\#.**

Target Datastore Name Format

Displays the format for a Datastore object created for a target
connection when building an SAP Data Services package. Default value is
**\#TARGET\#.**

Collect Datastore Name Format

Displays the format for a Datastore object created for a collect
connection when building a SAP Data Services package. Default value is
**dgDataGarage**.

Download Job Settings

Download Job Name Format

Displays name format for the job that executed a download of source
table to a target table. Default value is
**\#SOURCE\#\_\#TARGET\#\_\#SOURCETABLE\#\_imp**.

Download Job Data Flow Name Format

Displays the format for the Data Flow object in a Download job. Default
value is **DF\_\#SOURCE\#\_\#TARGET\#\_\#SOURCETABLE\#**.

Download Job Source Table Data Flow Display Name Format

Displays the format for the source table display name in a Data Flow
object of a Download job. Default value is
**\#SOURCETABLE\#\_\#SOURCE\#**.

Download Job Target Table Data Flow Display Name Format

Displays the format for the target table display name in a Data Flow
object of a Download job. Default value is
**\#TARGETTABLE\#\_\#TARGET\#**.

Download Job Source Table Description Format

Displays the format of the source table description in a Download job.
Default value is **\#SOURCETABLE\# table from \#SOURCE\#**.

Download Job Target Table Description Format

Displays the format of the target table description in a Download job.
Default value is **\#TARGETTABLE\# table from \#TARGET\#**.

Download Job Schema Name Format

Displays the format of the Schema Name object in a Download job. Default
value is **TFM\_\#TARGETTABLE\#**.

Query Job Settings

Query Job Name Format

Displays name format for the job that executes a schema query on a
Datastore. Default value is **Collect staging table
dg\#JOBTYPE\#Query\_\#SOURCE\#**.

Query Job Data Flow Name Format

Displays name format for a DataFlow object in a Query job. Default value
is **DF\_dg\#JOBTYPE\#Query\_\#SOURCE\#**.

Query Job SQL Query Name Format

Displays name format for a SQLQuery object in a Query job. Default value
is **SQL\_dg\#JOBTYPE\#Query\_\#SOURCE\#**.

Query Job Target Table Data Flow Display Name Format

Displays format for the target table display name in a Data Flow of a
Query job. Default value is **\#QUERYJOBTARGETTABLE\#(Collect)**.

Query Job Target Table Description Format

Displays format of the target table description in a Query job. Default
value is **Collect staging table \#QUERYJOBTARGETTABLE\#.**

## <span id="DBMoto_Settings_Tab">DBMoto Settings tab</span>

Field

Description

Application Settings

Server Name

Displays the server name where DBMoto® is installed on.

Group Size

Displays number of tables in each monitoring group – to be determined by
the client. Groups are table sets that share the same log reader thread.
It is more efficient to check for changes once for a group of tables
than to log in for each table individually. Also, the changes for all
the tables in a group are processed in the same order as they appear in
the transaction log. This is useful when there are referential
constrains between tables. Each group runs in a single thread mode with
one table refreshing at a time. Default value is **50**.

Maximum Connections

Displays limit of simultaneous connections to the source system. Default
value is **8**.

Mirror Interval

Displays number of seconds between checking the system log for changes.
Recommended value is no less than 60 seconds. Default value is **300**
seconds.

Start Replicator

If enabled, DBMoto® Replicator is started after each build package
process completes. If disabled, DBMoto® Replicator must be manually
restarted in the DBMoto® Management Center on the application server.
Default value is Disabled.

Enable Group

If disabled, the DBMoto® packages do not automatically run after the
build process is complete. The package stays in a Replication Status of
Disabled and an Initialization Status of Pending. The user must manually
enable the replication in the DBMoto® Management Center.

If enabled, the DBMoto® packages automatically start executing after the
build process completes.

Metric Time

Displays date when all tables without rules will have boaDBMotoInd set
back to zero and daily change count insert into Metric log. Default
value is **11:00 pm**.

## <span id="Workflow_Settings_Tab"></span>Workflow Settings tab

Use this tab to [Update the Retention Expiration Warning
Period](../Use_Cases/Update%20Retention%20Expiration%20Warning%20Period.htm).

Field

Description

Retention Date Notification

Retention Expiration Date Notification

Displays the number of days before data is purged (the retention
expiration date) that a warning workflow email is sent to the Data
Controller.

The email contains a list of objects whose data will be purged and a
link to access the objects in the DSP.

The DSP sends this email daily when an object is scheduled to be purged
during this time.

Retention Warning Email

Click to open the Collect *[Retention Expiration
Email](../../Collect/Page_Desc/Retention_Expiration_Email.htm)* page to
configure the subject line and body of the workflow email sent when an
object’s retention date is within the number of days set in the
Retention Expiration Date Notification field.

Email Contents

Collect Work Flow From Email

Displays email address of account that sends workflow emails.

Collect Work Flow Failure Body

Displays text for body of failed table workflow emails.

Collect Work Flow Failure Table Vertical

Displays the header definition for failed table workflow emails.

Collect Work Flow Summary Body

Displays text for body of summary workflow emails.

Collect Work Flow Summary Table Header

Displays table header row in summary workflow emails.

Collect Work Flow Summary Table Line

Displays the row definition for summary workflow emails.
