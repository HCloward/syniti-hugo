+++
title = 'Create a Service Page'
solution = 'Platform'
+++

# Create a Service Page

A Service page is a non-interactive page configuration that allows
events to be configured and executed on a time-based Unit of Measure
(UOM). Service pages are commonly used for automating a process to
execute business logic against a specific record set. This could range
from executing public WebApp events (for instance, running CranPort
packages) to trimming log tables in a custom application.

Since these pages are non-interactive, the user configured as the
“Service” user (Configuration \> Parameters \> Service Options \>
Service User ID) must have permissions to this page. This is to ensure
the events on the page can be executed.

A Service page requires a table, but is not displayed in the DSP®. The
OnValidate event for a Service page runs for every record that appears
in its table on a regularly scheduled basis based on the page
properties. A Service page can be as simple as a view. The view could
point to all records in a table where an OnValidate event sends an email
for each record in the table.

Refer to [Stop and Start Service
Pages](../Sys_Admin/Use_Cases/Stop_and_Start_Service_Pages) and
[Configure Service
Pages](../Sys_Admin/Use_Cases/Configure_Service_Pages) for more
information.

To create a Service page:

1.  Select **Admin \> WebApps** in the *Navigation* pane.
2.  Click the **Pages** icon for a WebApp and click **Add**.

OR

1.  Click the WebApp name in the *Navigation* pane.

2.  Click the **Change Settings** icon on the Site toolbar, click
    **Design**, and click **Add**.
    
    [View the field descriptions for the Pages
    page](../Sys_Admin/Page_Desc/Pages_H)

3.  Enter the page name in the **DESCRIPTION** field.

4.  Select Service in the **PAGE TYPE** list box.

5.  Select the table where the service page data is to be stored in the
    **TABLE** list box.

6.  Click **Save**.

7.  Click **Vertical View**.

8.  Click the **Service Properties** tab.

9.  Click **Edit**.
    
    [View the field descriptions for the Page page's Vertical
    View](../Sys_Admin/Page_Desc/Pages_H)

10. Select **Service Pages** from the **Queue ID** list box.
    
    **NOTE:** A Service page must be assigned to a queue to be executed
    by the service.

11. Enter a date for **Next Service Date**.
    
    **NOTE:** The Next Service Date field does not normally need to be
    completed unless the user wants the Service page to run on a
    particular date at a particular time and not interval X from now as
    stated in the Service Qty and Service UOM.

12. Enter a value for **Service Qty**.

13. Select an option from the **Service UOM** list box.
    
    **NOTE:** The Service UOM field uses the Qty value. For example, if
    the service page is to run once every 24 hours, enter 1 for Service
    Qty and select Day(s) for Service UOM.
    
    **NOTE:** The Service Qty and Service UOM are used to compute the
    Next Service Date. If the Next Service Date field is populated, then
    the service page overrides these values. If the Next Service Date
    field is NULL, then the service page runs immediately.
    
    **NOTE:** When the interval is set, the OnValidate event runs
    against the data provided in the *Horizontal* View. This means, if
    the view returns N records, the OnValidate event runs against each
    of the N records.

14. Click the **Active** check box to enable it.

15. Click **Save**.
