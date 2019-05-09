+++
title = 'Build Index Objects'
solution = 'Platform'
+++

# Build Index Objects

An index is comprised of several SQL Server objects, including three
tables to store the index and four stored procedures to populate the
index. Before a table can be indexed, the objects must be built based on
the index configuration. Building the index objects is generally a
one-time event. If the index configuration changes, the objects must be
rebuilt.

To build the index objects:

1.  Select **Admin \> Data Sources** in the *Navigation* pane.
2.  Click the **Index** icon for a data source.
3.  Click the **Build** icon in the Page toolbar to build the selected
    index.

The build process creates three tables in the user database:
TableName\#SearchKey, TableName\#Search and TableName\#SearchWord, where
TableName is the name of the indexed table. The tables comprise a
reverse index of the records in the table.

  - The \#SearchKey Table: Because the source table may not have an
    optimal primary key structure, the primary keys for each record is
    stored in the \#SearchKey table. Each key is assigned a new ID using
    a SQL Server IDENTITY column, called boaKeyID.
  - The \#SearchWord Table: Every unique word in the source table
    contains a record in the \#SearchWord table. In addition to the
    word, a pre-computed SoundEx value is stored with the word. The word
    is assigned an ID, boaIndexID, which is a SQL Server IDENTITY
    column.
  - The \#Search Table: The \#Search table is the reverse index for the
    table and associates individual words with records. A word is paired
    to a record once. If the word appears in the record more than once,
    a count is reflected in the Occurrences column. The IsSynonym column
    designates whether the word appears in the record or whether a
    synonym of the word appears in the index.

In addition to the index tables, several stored procedures are created
for managing the index:

  - boaIndex\_TableName\_KeyFilterExecuteLoop
  - boaIndex\_TableName\_Loop.
  - boaIndex\_TableName\_NoFilterExecuteLoop
  - boaIndex\_TableName\_PartialExecuteLoop

These procedures are used by the internal indexing routines and should
not be modified directly.
