+++
title = 'Configure Service Pages'
solution = 'Platform'
+++

# Configure Service Pages

A service page is a non-interactive page configuration that allows
events to be configured and executed on a configured time-based Unit of
Measure (UOM). Service pages are commonly used for automating a process
to execute business logic against a specific record set. This could
range from executing public WebApp events (for instance, running
Assemble packages) to trimming log tables in a custom application.

Since these pages are non-interactive, the user configured as the
“Service” user (Configuration \>Parameters \> Service Options \>
Service User ID) must have permissions to this page. This is to ensure
the events on the page can be executed.

A Page Designer creates a service page. Refer to [Create a Service
Page](../../WebApp_Dev/Create%20a%20Service%20Page.htm) for more
information.

**NOTE**: No shipped application service pages should be updated
directly. Some applications may provide options within their own
application that can affect the service page as a way of indirectly
configuring service page behavior.

To configure services pages:

1.  Select **WebApps** in *Navigation* pane.

2.  Click **Pages** for the **WEB APP NAME**.

3.  Click *Vertical* View for a page with a **PAGE TYPE** of Service.

4.  Click **Service Properties** tab.

5.  Click **Edit**.
    
    [View the field descriptions for the Pages Vertical
    View.](../Page_Desc/Pages_H.htm#Pages_V)

6.  Select **Service Pages** from the **Queue ID** list box.

7.  Enter a date for **Next Service Date**.
    
    **NOTE**: The **Next Service Date** field does not normally need to
    be completed unless the user wants the service page to run on a
    particular date at a particular time and not interval X from now as
    stated in the **Service Qty** and **Service UOM**.

8.  Enter a value for **Service Qty**.
    
    **NOTE**: There is no limit to the value entered in the **Service
    Qty** field.

9.  Select an option from the **Service UOM** list box.
    
    **NOTE**: This is a required field. The **Service UOM** field uses
    the Qty value. For example, if the service page is to run once every
    24 hours, enter 1 for **Service Qty** and select Day(s) for
    **Service UOM**.
    
    **NOTE**: The **Service Qty** and **Service UOM** are used to
    compute the **Next Service Date**. If the **Next Service Date**
    field is populated, then the service page will override these
    values. If the **Next Service Date** field is NULL, then the service
    page will run immediately.
    
    **NOTE**: When the interval is set, the OnValidate event will run
    against the data provided in the Horizontal View. This means, if the
    view returns N records, the OnValidate will run against each of the
    N records.

10. Click the **Active** check box to enable it.

11. Click **Save**.

12. If a copy of the service page is required, click **Copy**.
