# Add a Column to an Index

While adding an index, an Administrator adds at least one searchable
column.

Before performing this task, [Create an Index](Create%20an%20Index.htm)
and [Configure an Index,](Configure%20an%20Index.htm) if needed.

Refer to [Build Indices for a Data
Source](Build%20Indices%20for%20a%20Data%20Source%20for%20Search%20and%20Duplicate%20Detection.htm)
for general information.

To add a column to an index.

1.  Select **Admin \> Data Sources** in the *Navigation* pane.

2.  Click the **Index** icon for a data source.

3.  Click **Columns**.

4.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.
    
    [View the field descriptions for the Index Columns
    page](../Page_Desc/Index%20Columns.htm)

5.  Select a field from **Column** list box.

6.  Select an ID from **Dictionary ID** list box.
    
    **NOTE:** Dictionaries are used to associate a synonym or
    abbreviation with a word. Refer to [Create Column
    Dictionaries](Create%20Column%20Dictionaries.htm) for more
    information.

7.  Click the **Searchable** check box to mark the column as searchable.
    
    **NOTE:** At least one column must be searchable to build the index.

8.  Click the **Duplicate Detection** check box if the column is
    searched when looking for duplicates.

9.  Click the **Key** check box if this column is the table key.
    
    **NOTE:** If the table does not have a key, one must be manually
    defined. Refer to [Assign Key Columns](Assign%20Key%20Columns.htm)
    for more information.

10. Click **Save**.

Continue with [Build the Index](Build%20the%20Index.htm).
