+++
title = 'Create Schedules'
solution = 'Platform'
+++

# Create Schedules

Schedules added in Common can be used across all dspMigrate™ components
that have schedules, such as refreshing a source in Collect. Schedules
can recur on several intervals, including every few minutes, every
Tuesday and Thursday, or every October 19<sup>th</sup>.

**NOTE:** If using a schedule to send workflow notifications from ISA,
update the ISA parameter Days to Retain Files (ISA
*[Parameters](../../../Data_Quality/ISA/Page_Desc/ISA_Parameters.htm)*
page Basic Settings tab) so that it is at least equal to the number of
days in the longest schedule registered to a Project Distribution. Refer
to [Schedule Workflow
Notifications](../../../Data_Quality/ISA/Use_Cases/Schedule_Workflow_Notifications.htm)
for more information.

To create a schedule:

1.  Select **Tools \> Schedules** in the *Navigation* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Schedules
    page](../Page_Desc/Schedules_H.htm)

3.  Enter the name of schedule in the **Name** field.
    
    **NOTE:** Schedules must have a unique name.

4.  Enter a description of schedule in the **Description** field.

5.  Select a recurrence schedule from the **Recurrence ID** list box to
    determine the pattern of the schedule.

6.  Select a time for the **Black Out Time Start** to specify a start
    time for when the schedule does not apply.

7.  Select a time for the **Black Out Time End** to specify an end time
    for when the schedule does not apply.

8.  Select blackout days to determine which days the schedule does not
    run.

9.  Click **Save**.

10. Click the link for the **Recurrence ID**.
    
    [View the field descriptions for the Schedule – Configure
    page](../Page_Desc/Schedule_Configure.htm)
    
    **NOTE:** The fields available to configure the schedule vary
    according to the Recurrence ID.

11. Click <span style="font-weight: bold;">Edit</span>.

12. Populate the recurrence fields using the following table.

13. Click **Save**.

Recurrence ID

Field

Description

Minutes – Every \#\# minutes – Example: Every 30 minutes

Interval

Enter an occurrence of schedule in minutes. Interval must be at least
10.

Hourly – Every \#\# hour(s) – Example: Every 2 hour(s)

Interval

Enter an occurrence of schedule in hours.

Daily – Every \#\# day(s) – Example: Every 2 day(s)

 

Interval

Enter an occurrence of schedule in days.

Set time

Select a time of day for the schedule.

Daily – Every weekday

 

Set Time

Select a time of day for the schedule.

Weekly – Recur every \#\# week(s) on specific weekdays – Example: Recur
every 3 week(s) on Tuesday, Thursday, Saturday

 

Interval

Enter an occurrence of schedule in weeks.

Set time

Select a time of day for the schedule.

Sunday

Click check box for the schedule to run on Sundays.

Monday

Click check box for the schedule to run on Mondays.

Tuesday

Click check box for the schedule to run on Tuesdays.

Wednesday

Click check box for the schedule to run on Wednesdays.

Thursday

Click check box for the schedule to run on Thursdays.

Friday

Click check box for the schedule to run on Fridays.

Saturday

Click check box for the schedule to run on Saturdays.

Monthly – Fixed date – Example: Day 1 of every 3 month(s)

 

Interval

Enter an occurrence of the schedule in months.

Set time

Select a time of day for the schedule.

Fixed Date

Select a day within the month.

Monthly – Variable date – Example: The third weekday of every 2 month(s)

 

Interval

Enter an occurrence of the schedule in months.

Set time

Select a time of day for the schedule.

Recurrence Day

Enter a recurrence day within the month.

Yearly – Fixed date – Example: Every October 19

 

Set Time

Select a time of day for the schedule.

Fixed Day

Select a day within the month.

Recurrence Month

Select a recurrence month within the year.

Yearly – Variable date – Example: The third Sunday of March

 

Set Time

Select a time of day for the schedule.

Recurrence Day

Select a recurrence day within the month.

Recurrence Month

Select a recurrence month within the year.
