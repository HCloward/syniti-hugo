# Configure boaReport Reserved Column

When the boaReport reserved column is included in a *Horizontal* or
*Vertical* View, a Report icon displays. If the value of boaReport is 1,
the icon is enabled; if 0, the icon is disabled.

When generating a report on a page, the report is filtered down to a
single record. If the record links to any other pages and the Report
Follows Link column property is enabled, the report generator follows
the link and includes the downstream pages in the report.

For example, assume a *Customers* page links to an *Orders* page which
is linked to an *Order Details* page. The Report Follows Link option is
enabled on all linked pages. The *Customers* page has a boaReport
column. When the user clicks **Report** on the Page Options drop down on
the *Customers* page, a report for a single customer displays. The
report contains information for that customer, including orders and
order line items.

To implement the boaReport Reserved Column:

1.  Select **Admin \> WebApps** in the *Navigation* pane.

2.  Click the **Pages** icon for a WebApp.

3.  Click the **Column Properties** icon for a page.

4.  Click **Add**.
    
    [View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H.htm)

5.  Select **Reports** from **COLUMN** list box.
    
    **NOTE**: The Reports option is the boaReport reserved column.

6.  Select **All Views** from **VIEW TYPE** list box.

7.  Select **Image** from **CONTROL** list box.

8.  Select a page from **LINK TO PAGE** list box.
    
    **NOTE**: The Link To Page is the page that DSP navigates to when
    the page link is clicked.

9.  Verify **Enabled** is selected from **CONTROL STATUS** list box.

10. Click **Save**; the *Vertical* View displays.

11. Select **Report** from **Image ID** list box.
    
    **NOTE**: Any Image ID can be used; however, Report is the
    commonly-used icon.

12. Click **Report Follows Link** check box to include linked-to pages
    as sub-reports for each record.
    
    **NOTE**: Refer to [Configure Report Generation for Linked
    Pages](Configure%20Report%20Generation%20for%20Linked%20Pages.htm)
    for more information.

13. Click **Link to Report** check box to immediately run a report on
    the linked-to pages instead of displaying the page.
    
    **NOTE**: Refer to [Link To Report
    Pages](Link%20to%20Report%20Pages.htm) for more information.

14. Click **Save**.
