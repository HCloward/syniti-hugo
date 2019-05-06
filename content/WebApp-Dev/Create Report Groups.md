# Create Report Groups

The view used to render a report can contain denormalized data. Such
data can be organized into a hierarchically structured report using
Report groups. Report groups can be defined at the page level for
Dynamic and Report page types.

To demonstrate, a view that joins the Customers, Order and Order Details
tables produces a denormalized data set. This data set contains
redundant information as shown in the following table:

|            |          |         |             |           |         |
| ---------- | -------- | ------- | ----------- | --------- | ------- |
| CustomerID | Name     | OrderID | OrderNumber | ProductID | Product |
| 42         | John Doe | 1001    | 2007010201  | 00099     | T-Shirt |
| 42         | John Doe | 1001    | 2007010201  | 00202     | Shoes   |
| 24         | Jane Doe | 1002    | 2007010202  | 00099     | T-Shirt |

This example contains two customers, each with a single order. John
Doe’s order contains two line items. Consequently, the customer and
order information has been repeated for the second line item. Only the
ProductID and Product fields are different for the second row.

The advantage to a denormalized data set is that much, if not all, of
the relevant data can be retrieved with a single query. Otherwise,
building a multi-level report requires several page requests. The total
processing time can be greatly reduced by combining related data into a
single view.

If the report generator obtains this data from the *Customers*, *Orders*
and *Order Details* pages separately, a request to the *Customers* page
is created to retrieve the customer information. Then two requests to
the *Orders* page to retrieve the order headers for each customer are
created and two requests to the *Order Details* page to retrieve the
order line items for the two orders are created. This approach does not
scale well when adding a customer with a single order results in two
additional page requests, one request for the order header information
and one for the order’s line items.

In most cases, the overhead of processing many additional page requests
outweighs the overhead incurred from loading the duplicate data and
organizing the data set with report groups.

To create a report group:

1.  Select **Admin \> WebApps** in the *Navigation* pane.

2.  Click the **Pages** icon for a WebApp.

3.  Click **Vertical View** for a Dynamic or Report page type.

4.  Either
    
    For a Dynamic page type, click the **Report Options** tab, and then
    click the **Report Groups** icon.
    
    Or
    
    For a Report page type, click the **Report Groups** icon.

5.  Click **Add**.
    
    [View the field descriptions for the Report Groups
    page](../Sys_Admin/Page_Desc/Report%20Groups.htm)

6.  Enter a report name in **NAME** field.

7.  Enter a title in **TITLE** field.
    
    **NOTE**: Title is not a required field. The Title displays above
    each occurrence of the group in the report.

8.  Select a view from **VIEW** list box.
    
    **NOTE**: Report Groups support a Horizontal and Vertical View Type.
    In the previous example, customer information and order headers are
    rendered in a vertical fashion with fields stacked on top of one
    another. Order line items are rendered horizontally with each record
    on its own line.

9.  Click **PAGE BREAK BEFORE** check box, if applicable.

10. Click **PAGE BREAK AFTER** check box, if applicable.
    
    **NOTE**: Page breaks force a break either before or after a given
    report group. For example, to force each customer onto its own page,
    click Page Break Before check box for the Customer group.

11. Click **HIDE EMPTY FIELDS** check box, if applicable.
    
    **NOTE**: Hide Empty Fields controls which fields are omitted from
    the rendered report. Fields that are null or contain zero length
    strings are hidden. Enabling this field can cut down report space.
    This option only applies to vertical report groups, those report
    groups with a VIEW of Vertical on the *Report Groups* page.

12. Click **Save**.

Next, [Add Columns to a Report](Add%20Columns%20to%20a%20Report.htm).
