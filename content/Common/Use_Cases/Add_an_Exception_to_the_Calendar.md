+++
title = 'Add an Exception to the Calendar'
solution = 'Platform'
+++

# Add an Exception to the Calendar

Calendars are used in dspTrack™ and dspConcut™ components. Refer to [Use
a Calendar](Use_a_Calendar.htm) for more information.

When the users assigned to a calendar should work different hours than
on a regularly scheduled work day, add a calendar exception.  For
example, if regular work hours are 9:00 AM to 5:00 PM for all of the
work days on a calendar, but work hours are 9:00 AM to 12:00 PM on
December 24, add an exception to the calendar for this date.

To add an exception:

1.  Select **Common \> Tools \> Calendar** in the *Navigation* pane.

2.  Click **Exceptions** for a calendar.
    
    **NOTE:** If no exceptions exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    [View the field descriptions for the Calendar Exception
    page](../Page_Desc/Calendar_Exception.htm)

3.  Enter a date in the format MM/DD/YYYY or click a date on the
    calendar.

4.  Click **Save**.

5.  Click **ExceptionHours** for the date.

6.  Use the sliders to indicate hour, minute and second, or click
    **Now** to set the exception start time to the current time.

7.  Click **Done**.

8.  Click the **FINISH TIME** field.

9.  Use the sliders to indicate hour, minute and second, or click
    **Now** to set the exception finish time to the current time.

10. Click **Done**.

11. Click **Save**.

A Calendar Exception Date can have multiple sets of work hours. However,
a set of work hours cannot:

  - Overlap the hours of any other set of work hours
  - Start during hours already specified
  - Have a finish time that is earlier than its corresponding
    <span> </span>start time

The finish time for one set of work hours can be identical to the start
time of another set.

The following start and finish times are valid work hours for a Calendar
Exception Date:

|             |             |
| ----------- | ----------- |
| Start Time  | Finish Time |
| 12:00:00 AM | 9:00:00 AM  |
| 9:00:00 AM  | 5:00:00 PM  |
| 5:15:00 PM  | 11:59:00 PM |
