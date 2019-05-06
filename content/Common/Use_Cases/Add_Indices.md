# Add Indices

Indices are a way for the database system to find records efficiently.
Indices must be manually added to System Types.

To add indices:

1.  Click **Common \> System Types** in *Navigation* pane.

2.  Click **Tables** icon for a System Type.

3.  Click **Indices** icon for a table.

4.  Click **Add**.
    
    [View the field descriptions for the System Types Table Indices
    page](../Page_Desc/System_Types_Table_Indices.htm)

5.  Enter a name in **INDEX NAME** field.

6.  Click **UNIQUE INDEX** check box to build a unique index.
    
    OR
    
    Click **PRIMARY KEY** check box to build the index as a primary key
    for the table.

<!-- end list -->

1.  Click **CLUSTERED INDEX** check box to mark the index as clustered,
    which is a special index type in SQL Server. Refer to Microsoft SQL
    documentation on details for clustered indices.
    
    **NOTE:** **CLUSTERED INDEX** can be used with **PRIMARY KEY** to
    create a clustered or non-clustered primary key.

2.  Click **Save**.

3.  Click **Index Fields** for table index.
    
    <span style="font-weight: bold;">NOTE:</span> If no records exist,
    the page displays in Add mode. Otherwise, click Add on the Page
    toolbar.
    
    [View the field descriptions for the System Types Index Fields
    page](../Page_Desc/System_Types_Index_Fields.htm)

4.  Select field in column that exists in index from **SYSTEM TYPE TABLE
    FIELD ID** list box.

5.  Enter order of field in index in **COLUMN ORDER** field.

6.  Click **Save**.
