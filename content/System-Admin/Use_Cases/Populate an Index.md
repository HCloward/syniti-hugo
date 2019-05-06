# Populate an Index

Once an index has been built, it can be populated with data. This step
is required before users can search the index or before duplicate
detection can take place. Once the index has been fully populated,
incremental populations are performed as records are modified.

To populate an index:

1.  Select **Admin \> Resources \> Indices** in the *Navigation* pane.

2.  Click **Start**, a confirmation message displays.

3.  Click **OK**.
    
    **NOTE:** Once the table has been submitted to be indexed, a
    confirmation message displays.

4.  Click **OK**.

The job itself can be monitored by clicking **All Jobs**. The duration
of the job depends on the amount of data in the table.

The first stage of the full index process queues up records to index.
The records are then indexed in batches. Each batch is treated as a
step. The total number of steps is determined by the number of records.

To monitor the individual indexing process’s steps, click **Vertical
View**.

Full index population can occur on a schedule. A schedule is important
if data in the source table is re-imported nightly by an external
source. Only Active indices receive a full index. The ACTIVE check box
on the Indices page indicates the index is active.

A service page in the DSP® performs full indices. By default, the
service page executes once a day.
