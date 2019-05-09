+++
title = 'Identify SQL Performance Issues'
solution = 'Platform'
+++

# Identify SQL Performance Issues

If you are running a 6.5.X version of the DSP® or above, you can employ
a framework utility called the Page Performance Monitor.

The Page Performance Monitor is a utility included with the DSP intended
for technical users (those who are responsible for debugging SQL
performance issues). Use it on custom pages to troubleshoot performance
issues and to determine which portions of the page run slowly when the
record set (or user set) increases dramatically.

Generally, there are two metrics that can help troubleshoot delays in
load time: the 'dgResponse' and the 'RuntimeUtils.' The 'dgResponse'
portion has a long and variable duration, while the 'RuntimeUtils'
portion has an average and consistent duration.

The 'RuntimeUtils' portion consistently correlates with the number of
columns displayed on the *Horizontal* View of a page. The more columns
you have on the Horizontal View of a page, the longer the page will take
to load.

The 'dgResponse' portion is a result of the performance of the page's
underlying '%hor' view (*Horizontal* View). When there are too many
columns in the %hor view of an underlying table, or complex logic
embedded within the view (aggregations, etc), it prolongs the times it
takes to complete queries, which affects the page's performance.

To access this utility, click **Ctrl + Shift + K**.

![](../../../Resources/Images/inline1238732101.png)

**NOTE:** If the Debug Mode option is enabled for a user’s profile, that
user can access the Page Performance Monitor by selecting the Metrics
option in the Settings menu. Refer to [Configure User
Settings](../../../Configure%20Your%20User%20Settings.htm) for more
information.
