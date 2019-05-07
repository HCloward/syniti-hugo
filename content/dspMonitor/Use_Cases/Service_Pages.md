+++
title = 'Service Pages'
solution = 'Data Quality'
+++

# Service Pages

dspMonitor™ uses Service pages for background processing.  The schedule
of these Service pages can be adjusted to the client’s runtime and
dependencies to getting reports to users.

Service pages include:

  - [Build Group and Report Metrics](#Build_Group_and_Report_Metrics)
  - [Build Metric Data Aging](#Build_Metric_Data_Aging)
  - [Build Summary Workflow Report](#Build_Summary_Workflow_Report)
  - [Run Daily Maintenance Events](#Run_Daily_Maintenance_Events)
  - [Run File Deletion Maintenance](#Run_File_Deletion_Maintenance)
  - [Run Group Reports via Schedule](#Run_Group_Reports_via_Schedule)
  - [Run Recycle Failed Reports](#Run_Recycle_Failed_Reports)
  - [Send Attachment Workflow](#Send_Attachment_Workflow)
  - [Send Notifications WorkFlow](#Send_Notifications_WorkFlow)
  - [Send Summary
Workflow](#Send_Summary_Workflow)

## <span id="Build_Group_and_Report_Metrics"></span>Build Group and Report Metrics

**Description:** Calculates the report metrics by day, week and month.
The page also generates the summaries for groups by day, week and month.
There is a validation check to verify no reports are running in the
Platform job queue for dspMonitor™ before the Service page starts
running.

**Default Schedule:** Every weekday at 9:00 a.m.

## <span id="Build_Metric_Data_Aging"></span>Build Metric Data Aging

**Description:** Checks for reports that have finished processing and
that are marked to build Metric Data of report contents.  When reports
have completed processing each day, dspMonitor™ updates the Metric Data
table in a single thread process so the server does not get overloaded
running multithreaded events. 

**Default Schedule:** Every 30
minutes

## <span id="Build_Summary_Workflow_Report"></span>Build Summary Workflow Report

**Description:** Generates summary notifications for each user for all
reports they are assigned to receive. 

**Default Schedule:** Mondays and Fridays at 9:00
a.m.

## <span id="Run_Daily_Maintenance_Events"></span>Run Daily Maintenance Events

**Description:** Removes the following events:

  - Old Assemble packages after the report has been completed for 24
    hours

  - Old report metrics that exceed the retention period

  - Old workflows that exceed the retention period

  - User filters as a verification process

**Default Schedule:** Once daily at 9:00 p.m.

**NOTE:** This Service page should run when dspMonitor™ is not
processing other groups to reduce system
contention. 

## <span id="Run_File_Deletion_Maintenance"></span>Run File Deletion Maintenance

**Description:** Deletes old reports from the file system. The **Keep
File Duration** parameter (Configuration \> Parameters) controls how
many days old a report must be in order to be deleted.

**Default Schedule:** Once daily at 4:00
p.m.

## <span id="Run_Group_Reports_via_Schedule"></span>Run Group Reports via Schedule

**Description:** Processes a group when the system time is greater than
the **Next Group Process Time**, which is controlled at the group level.
The next runtime is calculated for the group and then the reports are
submitted to the Platform job queue for processing.

**Default Schedule:** Every 10
minutes

## <span id="Run_Recycle_Failed_Reports"></span>Run Recycle Failed Reports

**Description:** Attempts to re-run failed reports.

**Default Schedule:** Every hour

## <span id="Send_Attachment_Workflow"></span>Send Attachment Workflow

**Description:** Checks the report and group notification workflows that
have attachments and sends out all of the notifications that are ready.

**NOTE:** Every notification workflow with attachments is sent from this
service. Invalid email addresses or SMTP errors with attachments may
prevent other workflows from being processed. Select Configuration \>
User Reports/Filters \> Workflow to view workflow errors.

**Default Schedule:** Every 10
minutes

## <span id="Send_Notifications_WorkFlow"></span>Send Notifications WorkFlow

**Description:** Checks the report and group notification workflows that
do not have attachments and sends out all of the notifications that are
ready.

**NOTE:** Every notification workflow is sent from this service. Invalid
email addresses or SMTP errors with attachments may prevent other
workflows from being processed. Select Configuration \> User
Reports/Filters \> Workflow to view workflow errors.

**Default Schedule:** Every 10 minutes

## <span id="Send_Summary_Workflow"></span>Send Summary Workflow

**Description:** Checks the report and group notification workflows that
have attachments and sends out all of the notifications that are ready.

**NOTE:** Every notification workflow with attachments is sent from this
service. Invalid email addresses or SMTP errors with attachments may
prevent other workflows from being processed. Select Configuration \>
User Reports/Filters \> Workflow to view workflow errors.

**Default Schedule:** Every 10 minutes
