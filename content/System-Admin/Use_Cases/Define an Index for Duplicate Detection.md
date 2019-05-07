+++
title = 'Define an Index for Duplicate Detection'
solution = 'Platform'
+++

# Define an Index for Duplicate Detection

By default, the Duplicate Detection validation rule uses the search
index. A page can be explicitly associated with an index for searching
and with another index for Duplicate Detection. This association is
useful when records are added to one table; however, duplicates need to
be checked for in another table.

**NOTE**: When performing Duplicate Detection against an index of
another table, the view must contain the primary key columns as defined
at the index level. If there are no keys defined at the index level,
then the view must contain the source table’s primary keys.

To define the index for Duplicate Detection:

1.  Click **Admin \> WebApps** on the *Navigation* pane.

2.  Click the **Pages** icon for a webapp.

3.  Click **Vertical View** for a page.

4.  Click the **Search Options** tab.

5.  Click **Edit**.
    
    [View the field descriptions for the Pages page Vertical
    View](../Page_Desc/Pages_H.htm)

<!-- end list -->

1.  Select an option from **Duplicate Detection Search ID** list box.
2.  Click **Save**.
