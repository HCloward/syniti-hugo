# Create Tables in SQL

The majority of the pages in a WebApp are Dynamic page types and require
an underlying table and a view.

Refer to [Create Views in SQL](Create_Views_in_SQL.htm) for more
information.

Well-designed tables allow for an efficient and easy to develop WebApp.
Both naming conventions and standard SQL design practices can contribute
to the longevity and extensibility of an application.

Refer to [Table Naming Conventions](Table_Naming_Conventions.htm) for
more information.

When creating tables.

  - Capitalize field names in such a way that DSP® correctly displays
    the label. For example, for the column name **ProductHistory**, DSP®
    automatically inserts a space between Product and History.
  - Consider a naturally occurring and meaningful primary key.
  - [Add BOA reserved columns to every table
    manually](Add%20Reserved%20Columns%20%20to%20Tables.htm), or use the
    Append Columns feature to automatically include BOA reserved columns
    to all tables. Refer to [Append BOA Reserved Columns to
    Tables](Append_BOA_Reserved_Columns_to_Tables.htm) for more
    information, including a list of BOA reserved columns. 
  - Use default field sizes or common field sizes as much as possible
    unless the exact size of the field contents is known, e.g.,
    NVARCHAR(50) instead of  NVARCHAR(45) or NVARCHAR(255) instead of
    NVARCHAR(200).
  - Normalize data:
      - Avoid tables that have common keys; put all the data in one
        table.
      - Avoid repeating data groups in tables.

Data Types

Data types are an important characteristic from both a back end and
front end perspective. Minimizing data types to their smallest relevant
size can improve performance and reduce database bloat. One example of
appropriate size limiting is within the System Administration WebApp in
the DSP®. Fields that contain SQL View Names (e.g. *Horizontal* View)
will only ever contain view names directly from SQL Server. Since SQL
Server object names are limited to 128 characters, this field can and
should be limited to 128 characters.

Character data types are important for application behavior as well.
Most times, nvarchar is preferred over varchar due to the Unicode
support of nvarchar. Names and descriptive fields should be nvarchar to
ensure they support the widest range of character sets.

Column Collation

Column collation allows for overriding the database's default collation
with a custom one, which can impact behaviors like case-sensitive
comparisons. This can be considered during application design to
determine if a field’s case sensitivity is relevant at a business logic
level.

Optimization

Indexes and data type minimization can both lead to a high performing
table even with millions of records. Everything else in the application
will be built on these tables, so if this foundation is rushed or not
given enough thought, the result may be excessive technical debt in the
future.
