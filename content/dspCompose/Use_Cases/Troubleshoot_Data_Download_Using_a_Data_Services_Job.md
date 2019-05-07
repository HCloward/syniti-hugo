+++
title = 'Troubleshoot Data Download Using a Data Services Job'
solution = 'Data Quality'
+++

# Troubleshoot Data Download Using a Data Services Job

A Role Processor can troubleshoot issues related to the data download
during the Final Finish process using a Data Services job.

Refer to [Register Tables for Download through Data
Services](Register_Tables_for_Download_through_Data_Services.htm) for
general information.

To troubleshoot Data Services jobs,
select<span style="font-weight: bold;"> dspCompose \> Configuration \>
Data Services Job Executor</span> in the
<span style="font-style: italic;">Navigation</span> pane.

On the [Data Services Job
Executor](../Page_Desc/Data_Services_Job_Executor.htm) page, a user can:

  - Click the Execution Logs icon for a job name and request ID to view
    the job status.
  - Click the Execute icon to run the job again.
  - Click the Global Variables icon to enter Global Variables,
    name/value pairs that can be passed into the execution job,
    similarly to how variables are passed into a function. For example,
    if a job must download data for a specific company code, configure
    the Data Services job to take in a global variable called
    "$CompanyCode" with a company code value. Only data pertaining to
    that company code’s value is passed in to the job and only data for
    that company code is downloaded during the final finish process.
