# Build Indices for a Data Source for Search and Duplicate Detection

Indices enable keyword searching of tables and the pages that expose the
data in the tables. An index for a database table makes table rows with
specific column values easy to find, which helps queries find data
quickly and improves database performance.

When using an index, a search text box displays on the Filter Panel,
accessible when the user clicks the small gear icon on the Page toolbar
and selects Filter. Text entered in the search box is run through the
index and against various synonyms and stop lists to generate a
returning page with similar results to the search term.

Indices are used in the Duplicate Detection process and the Bulk
Duplicate Detection process. Duplicate Detection can be used for a
Validation rule, typically associated with an OnValidate event. An index
can also be used to increase search efficiency in the Duplicate
Detection process. The output from this process is located in the
\[tablename\]\#Duplicate table. It contains the keys for the duplicates
and a rank that indicates how close the records match. An index is added
to this table to perform the Duplicate Detection process.

Refer to Find Duplicates Overview in Common help for more information.

Any table in any data source can have an index. Views can be indexed to
match the search filter, web\*Search.

While indices can be beneficial, use them sparingly to avoid performance
degradation.

Indices added using the steps in this section are nonclustered, meaning
they are separate index tables. Additional storage space is required and
depends on the size of the table, and the number and types of columns
used in the index.

It is recommended that an index not be created for:

  - Small tables.
  - Tables that have frequent, large batch update or insert operations.
  - Columns that contain a high number of NULL values.
  - Columns that are frequently manipulated

**NOTE**: Indexing is performed on text fields only. Numeric, binary,
dates and other non-text fields are not indexed.

To create and build indices:

• [Create an Index](Create%20an%20Index.htm)

• [Configure an Index](Configure%20an%20Index.htm)

• [Add a Column to an Index](Add%20a%20Column%20to%20an%20Index.htm)

• [Create Column Dictionaries](Create%20Column%20Dictionaries.htm)
(optional)

• [Assign Key Columns](Assign%20Key%20Columns.htm)

• [Build the Index](Build%20the%20Index.htm)

**NOTE**: Views and tables without primary key constraints require
additional configuration. Refer to [Assign Key
Columns](Assign%20Key%20Columns.htm) for more information.

A user can also [Create Stop Lists](Create_Stop_Lists.htm) for an index.
