+++
title = 'Create Report Views'
solution = 'Platform'
+++

# Create Report Views

The first step in creating a report is to create a report view in SQL
Server. If a page has a report view, the report view is registered to
the page instead of the *Horizontal* or *Vertical* View. Therefore,
reports generated from Dynamic pages can display data for both the
*Horizontal* and *Vertical* View.

**NOTE**: Report views are optional on Dynamic page reports. Refer to
[Enable Dynamic Page Reporting](Enable%20Dynamic%20Page%20Reporting.htm)
for more information.

Filter, drill-down and sort criteria are applied to the report view. The
report view must have the following elements:

  - Primary key columns as defined at the source table or at the column
    property level.
  - All columns that can be used to filter the *Horizontal* View.
  - All columns that can be used when drilling down to the page.

**NOTE**: If the Dynamic page has been accessed via drill down, it may
be filtered on the page to reduce the data being shown to the user. The
preceding columns are required in the report so that the same filter can
be applied on report generation.

  - All sortable columns on the *Horizontal* View.
  - All columns referenced by the Order By page property. Refer to
    [Assign Page Properties to a Dynamic
    Page](Assign_Page_Properties.htm) for more information about the
    Order By property.

**NOTE**: The developer must take dynamic views into account. If a
single report view is designed for the page, it should contain all the
columns meeting the previously outlined criteria for all dynamic views.
The dynamic report views can correspond to the dynamic *Horizontal* and
*Vertical* Views.

To create a report view:

1.  Log in to Management Studio.
2.  Create the view based on the outlined criteria.
3.  Add each column to display in the final report.
4.  Save the view with prefix usr and suffix Sel.

**NOTE**: For example, a report containing Customers, Orders and
OrderDetails might be named usrCustomerOrderDetailSel.
