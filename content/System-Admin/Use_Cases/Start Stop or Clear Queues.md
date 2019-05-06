# Start, Stop, or Clear Queues

When troubleshooting issues related to job processing, an Administrator
can stop and start queues.

If a job is processing when the user clicks Stop, processing completes
but no new jobs are started in the queue.

The queue can also be cleared, which removes records from the log that
displays on the *[Recent Service
Activity](../Page_Desc/Recent%20Service%20Activity.htm)* page. If a job
is processing when the user clicks Clear Queue, an error results. It is
recommended to stop the service prior to clearing a queue. Queues can be
managed on the [Queues (Monitor)](../Page_Desc/Queues%20Monitor.htm) **
page,

An Administrator can also set the time when the jobs in a queue start or
end, which is useful when scheduling jobs that require extensive
resources to complete. Run these jobs at off peak times to have minimal
impact on performance. Any jobs still running after the end time has
passed will complete, but no new jobs in the queue will start until the
next start time.

View the completed jobs in a queue on the [Recent Service
Activity](../Page_Desc/Recent%20Service%20Activity.htm) page.

To set the start or end time for a queue manually:

1.  Select **Admin \> Configuration \> Service \> Queues** in the
    *Navigation* pane.

2.  Click **Edit** for a queue.
    
    *[View the field descriptions for the Queues
    page](../Page_Desc/Queues.htm)*

3.  Click the **START TIM**E field and use the time picker to set the
    time.

4.  Click the **END TIME** field and use the time picker to set the
    time.

5.  Click **Save**.
