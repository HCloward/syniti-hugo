# Configure Job Status Types

The DSP® is delivered with Job Status Types that indicate where a job is
in the execution process. Job Status Types are:

  - Cancelled
  - Executed
  - Failed
  - Initializing
  - Processing
  - Ready

A user cannot delete or add Job Status Types, but can update settings as
indicated below.

To configure Job Status Types:

1.  Select **Admin \> Configuration \> Setup \> Job Status Types** in
    the *Navigation* pane.

2.  Click **Edit** for a job status type.
    
    *[View the field descriptions for the Job Status Types
    page](../Page_Desc/Job%20Status%20Type.htm)*

3.  Enter a description of the type in the **DESCRIPTION** field.

4.  Enter a number in the **RETENTION DAYS** field.
    
    **NOTE:** This field sets the number of days jobs with this job
    status type are retained. After the retention date has passed, the
    job is deleted from the DSP® tables. Generally, the default value is
    appropriate; however, if DSP® performance is slow because a table is
    large, users may set the value lower to keep the table smaller.
    Users may also lower the value to prevent the database from growing
    too large.

<!-- end list -->

1.  Enable or disable the **SHOW ON JOBS SCREEN** check box as needed.
    
    **NOTE:** This setting determines whether jobs in this status
    display on the *[All Jobs](../Page_Desc/All_Jobs_H.htm)* page.

2.  Click **Save**.
