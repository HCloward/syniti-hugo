+++
title = 'Import a Data Source'
solution = 'Platform'
+++

# Import a Data Source

An Administrator performs this task to add data source metadata for
System Types. This process updates existing fields, adds new tables and
fields to the System Type, and loads the table and field data from the
tables into the selected data source so that they appear in Target
Design. By adding only the new data, customizations to the System Type
are not lost.

Before this task can be performed, the data source should be populated
in the SQL databases with all the required tables. This is usually done
through [the fetch tables process in
Collect](../../Collect/Use_Cases/Create_Groups_from_the_Fetch_Process.htm).

To import a data source:

1.  Click **System Types** in the *Navigation* pane.

2.  Click **Vertical View** for System Type.

3.  Click **Import From Data Source or Model** on the Page toolbar.

4.  Click **Edit**
    
    [View the field descriptions for the System Type Import
    page](../Page_Desc/System_Types_Import.htm)

5.  Select the data source from **Data Source ID** list box.
    
    **NOTE:** The data source selected must be a database on the local
    SQL server (i.e., a dg\* or sdb\* data source).

<!-- end list -->

1.  Select the System Type model from the System Type Model list box.
    
    **NOTE:** JDE and SAP are pre-delivered with the product.

2.  Select a language from the **Language ID** list box.
    
    **NOTE:** If the Language ID is not set, the default value defined
    in the platform is used.

3.  Click **Save.**

4.  Click **Import**.

The following actions are completed:

  - A list of Tables and corresponding fields is imported into a System
    Type.
  - The descriptions of those tables and fields is imported.
  - Fields are flagged as key fields.
  - Check Tables are assigned to fields.
  - The table and field data from the tables found in the selected data
    source is loaded; a confirmation message displays.

10\. Click **Ok**.
