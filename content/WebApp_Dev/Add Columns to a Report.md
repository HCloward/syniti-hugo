+++
title = 'Add Columns to a Report for a Report Group'
solution = 'Platform'
+++

# Add Columns to a Report for a Report Group

Each report group must have one or more columns. The columns indicate
where a group starts.

Report groups subdivide the columns within a view. It is therefore
important that columns appear in the correct order within the view. All
columns within a group must be placed to the right of the first report
group column. All columns belonging to the Customer group must be placed
to the right of CustomerID, but to the left of OrderID.

The following example does not produce the correct results because the
ProductName appears in the Customer group.

  - CustomerID
  - CustomerName
  - ProductName
  - OrderID
  - OrderDate
  - ProductID

The correct order is:

  - CustomerID
  - CustomerName
  - OrderID
  - OrderDate
  - ProductID
  - ProductName

In the example, the Customer group starts with a column named
CustomerID; the Orders group with OrderID; and the Products group with
ProductID.

To add columns to a report:

1.  Create a report group.

2.  Click the **Columns** icon on the *[Report
    Groups](../Sys_Admin/Page_Desc/Report%20Groups)* page. .

3.  Click **Add**.
    
    [View the field descriptions for the Report Group Columns
    page](../Sys_Admin/Page_Desc/Report%20Group%20Columns)
    
    **NOTE**: The PRIORITY field is not used.

4.  Select a name from **COLUMN NAME** list box.

5.  Select an order from **SORT ORDER** list box.

6.  Click **Save**.

7.  Repeat Steps 3 – 7 to add additional columns to the report.

If a report is not sorted at the report group level, sorting defaults to
standard page sorting mechanism including the Order By property on the
General tab of the *[Pages](../Sys_Admin/Page_Desc/Pages_H)* page's
*Vertical* View.
