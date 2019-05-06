# Create an Index

An Administrator can add index tables to a database for a Microsoft SQL
Server data source.

**NOTE**: If a data source is protected, (i.e., if the Protected check
box on the *Vertical* View of the *[Data
Sources](../Page_Desc/Data_Sources_HSysAdmi.htm)* page is enabled),
indices cannot be added.

Refer to [Build Indices for a Data
Source](Build%20Indices%20for%20a%20Data%20Source%20for%20Search%20and%20Duplicate%20Detection.htm)
for general information.

To create indices for a table:

1.  Select **Admin \> Data Sources** in the *Navigation* pane.

2.  Click the **Index** icon for a data source.

3.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.
    
    *[View the field descriptions for the Index (Specification)
    page](../Page_Desc/Index%20Specification%20H.htm)*

4.  Click the **ACTIVE** check box to enable it.

5.  Select the table to build the index for in the **TABLE** list box.

6.  Click **Save**; *Vertical* View displays.

7.  Click **Save**; A warning message displays: “No searchable columns
    in this search table.”
    
    **NOTE**: This message displays because the table has not yet had a
    searchable column designated and serves as a reminder to add at
    least one column to the index.

8.  Click **Yes**.

When creating an index, the default specifications display. Adjusting
these settings changes the way the compare engine operates. Continue
with [Configure an Index](Configure%20an%20Index.htm) if the settings
must be updated.

If the default configuration options for the index do not need to be
updated, continue with [adding a column to an
index](Add%20a%20Column%20to%20an%20Index.htm).
