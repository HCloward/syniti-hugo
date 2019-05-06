# Create a Combination Chart

A combination chart gives a page Designer the ability to combine
multiple chart types (pie, column, line, dotted line) on a single chart
page.

To add a combination chart page:

1.  Click the **Change Settings** icon on the Site toolbar while on any
    page.

2.  Select **Add Page**, the *Pages* page displays in a new window.

3.  Enter a description of the chart in the **DESCRIPTION** field.

4.  Select Chart from the **PAGE TYPE** list box.
    
    **NOTE:** It is not necessary to select a table when adding a Chart
    Page Type.

5.  Click **Save**; the *Vertical* View displays.

6.  Select the name of the view created in SQL from the **Report View**
    list box.

7.  Select **Combination** from the **Chart Type** list box.

8.  Click **Save**.
    
    **NOTE:** The page needs to be registered to the Configuration Menu
    so it can be accessed in the WebApp.

9.  Click the **Menu Name** link in the **Horizontal Menu ID**.

10. Click **Add**.

11. Enter a number in the **PRIORITY** field.

12. Select the Combination chart page from the **Link To PageID** list
    box.

13. Click **Save**.

14. Click the Back button on browser to return to the *Vertical* View
    for the *Pages* page.

15. Click **Chart Properties** to modify the chart properties, if
    needed.

Next, set the chart types to display on the combination chart page based
on a value for a page column.

To set the chart types to display on the combination chart page:

1.  Select **Admin \> WebApp** in the *Navigation* pane.

2.  Click **Pages** for the Webapp with the chart.

3.  Click **Column Properties** for the page; the *Page Columns* page
    displays.

4.  Click **Vertical View** for a Value page column.

5.  Click **Edit**.

6.  Enter a priority for the chart in the **Display Priority** field.
    
    **NOTE:** This setting determines how the charts are layered on the
    page. A chart with a priority of ‘1’ appears behind a chart with a
    higher priority of ‘2’.
    
    **NOTE:** As a best practice give line and dotted line charts a
    higher priority to display in front of column charts. This allows
    the user to hover over and access the data points on the line chart.

7.  Select a color from the **Color** list box.
    
    **NOTE:** This is an optional field. The color for the value control
    can be left blank to use default color.

8.  Click the **Show Values** check box to enable it.
    
    **NOTE:** This is an optional field.

9.  Select the marker type for a line chart from the **Marker** list
    box.
    
    **NOTE:** Use this option to change the shape of the marker on line
    charts where the data point is identified, such as a triangle or
    circle.

10. Select the type in the **Chart Type** list box.
    
    **NOTE:** Chart Type determines the chart type for the value
    control, such as line, dotted line, column, and pie.
    
    **NOTE:** Up to three value controls that do not use the pie chart
    type are allowed.
    
    **NOTE:** Only one value control can be assigned the pie chart type.
    
    **NOTE:** Pie charts display to the user on the top-left corner of
    the combination chart page.

11. Click **Save**.

To add another chart type to the chart page:

**NOTE:** Up to four charts can be added as long as one is a pie chart
type.

1.  On the *Page Columns* page, click **Add**.
2.  Select the column name from the **Column** list box.
3.  Select a value from the **Control** list box.
4.  Click **Save**.
5.  Repeat Steps 5 – 11 in the previous use case to update chart type
    and settings.

**NOTE:** The many options available for combination charts can result
in charts that are difficult for a user to interpret. As a best practice
when creating chart pages, make sure to review how the data displays
with the various options.
