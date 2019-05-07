+++
title = 'Configure Report Generation for Linked Pages'
solution = 'Platform'
+++

# Configure Report Generation for Linked Pages

A report can contain data from multiple pages. When a report is
generated, the generator starts by collecting data from the current page
and pulls data from any linked pages.

By default, the Report Follows Link column property is disabled for all
page links.

To instruct the report generator to follow a link:

1.  Select **Admin \> WebApps** in the *Navigation* pane.
2.  Click the **Pages** icon for a WebApp.
3.  Click the **Column Properties** icon.
4.  Click the link under **LINK TO PAGE** column.
5.  Click the **Report Follows Link** check box.

**NOTE**: If the Column Property is for the boaReport Reserved column,
the Report Follows Link check box is also available on the *Vertical*
View of the *[Page Columns](../Sys_Admin/Page_Desc/Page_Columns_H.htm)*
page. Refer to [Configure boaReport Reserved
Column](Configure%20boaReport%20Reserved%20Column.htm) for more
information.

The Report Follows Link column property can be used to create
multi-level reports. An example of a multi-level report is one that
contains data such as order headers and order line items. This column
property serves as an alternative to selecting the data with a
denormalized view and organizing the data set with report groups. This
method does not require the creation of additional pages or views, but
it can be much slower for large or complex data sets.

The following is an example of how a Page Designer could build a
multi-level report using the Report Follows Link option.

Add a link from a *Customers* page to an *Orders* page and a second link
from an *Orders* page to an *Order Details* page as follows:

1.  Click the **Column Property** icon for the *Customers* page.
2.  Complete the fields to add a **Link to Page** Column property that
    points to the *Orders* page.
3.  Click **Vertical View** for the *Page Columns* page for the property
    just added.
4.  Enable the **Report Follows Link** check box.
5.  Repeat this process to link the *Orders* page to the *Order Details*
    page.

When the report generator collects data for the *Customers* page, the
report contains links to the order information. The report generator
gathers each customer’s orders and follows the links to the order line
items. The final report contains data from all three pages.

It is possible for a Page Designer to create circular relationships.
Some circular relationships are legitimate. One example is an Employees
table where one employee can report to another employee. A restriction
is not imposed on circular relationships, which is why the Report
Follows Link column property is disabled by default. When this property
is enabled, the relationships among all pages involved must be taken
into consideration. Otherwise, clicking Report in the Page Options
drop-down can trigger an infinite loop.
