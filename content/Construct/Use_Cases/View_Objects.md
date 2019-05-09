+++
title = 'View Objects'
solution = 'Migration'
+++

# View Objects

The SQL code for the following object types is tracked for any given
data sources:

  - Tables
  - Procedures
  - Views
  - Functions
  - Other – additional SQL objects, such as synonyms, triggers and table
    functions

To view objects:

1.  Click **Analyze** in *Navigation* pane.
    
    **NOTE:** The *Analyze* page displays data source registered in
    System Administration. Data sources are analyzed for database object
    changes, table statistics and duplicate records.

2.  Click **Trace** for Data Source ID.

3.  Click an applicable icon to view tracked objects.

Two icons are available:

  - Click **SQL** icon to view the original SQL code, which is captured
    at the time an object is registered.
  - Click **History** icon to view an audit trail of the object.

**NOTE:**  If the database is refreshed and a change has been made to
the object, the audit trail of the modified SQL code is recorded. Refer
to [View Object History](View_Object_History) for detailed
information.
