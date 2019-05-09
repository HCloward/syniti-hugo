+++
title = 'Set up Connection Types'
solution = 'Platform'
+++

# Set up Connection Types

Connection Types require SQL Server to download the data dictionary from
the source database, a substring sample command and the windows driver
to embed in the package. Columns included in the download must be named
the same as the example in the database. The connection string in this
table must be fully populated or consequently, the database user ID and
password are ignored when using a user-defined ODBC connection.

**NOTE:** Collect is delivered with a list of connections used at a
majority of client sites. This step may be skipped in the connection is
already entered.

To add a connection type:

1.  Select **Administrative \> Connection Types** in *Navigation* pane.

2.  Click **Sources** for **SQL SERVER** Target Connection Type.
    
    **NOTE:** Collect only supports SQL Server Source databases.

3.  Click **Add**.
    
    [View the field descriptions for the Source Connection Types
    page](../Page_Desc/Source_Connection_Types_H)

4.  Enter the connection name in **SOURCE CONNECTION TYPE** field.
    
    **NOTE:** The SOURCE CONNECTION TYPE is the specific DBMS to which
    Collect connects. In order for the correct database transaction to
    called, the SOURCE CONNECTION TYPE must begin with “ODBC,”
    “SQLSERVER,” “ORACLE” or “OLE” followed by any combination of
    letters and numbers.

5.  Enter a provider in **OLE PROVIDER** field or enter a space if using
    an ODBC driver.

6.  Enter a driver in **ODBC DRIVER** field or enter a space if using an
    OLE provider.

7.  Click **Save**.

8.  Click **Vertical View** to further configure the Source Connection
    Type.

9.  Click **Edit**.
    
    [View the field descriptions for the Source Connection Types page's
    Vertical View](../Page_Desc/Source_Connection_Types_H)

10. Use the following table to populate the applicable connection
    settings based on DBMS
requirements:

|                           |                                                                                                                                                                                                                                                                                                                                                                                |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field                     | Description                                                                                                                                                                                                                                                                                                                                                                    |
| Fetchsize                 | Enter value for the number of records put into a buffer on the Windows server.                                                                                                                                                                                                                                                                                                 |
| Download SQL              | Enter SQL command used to read non-SAP databases to download table and column information from the source during the Build Package process. The data type conversions are performed during this load process and followed by Create Table and Create Keys/Indices.                                                                                                             |
| Download Table SQL        | Enter SQL called during the Fetch Table process. A list of tables that is available to download is pulled from the Source system.                                                                                                                                                                                                                                              |
| Download Primary Key SQL  | Enter SQL called during the Build Package process. SQL verifies the table built from SQL has a primary key. If this field is blank, the new table in SQL Server will not have any primary keys.                                                                                                                                                                                |
| Download Indices SQL      | Enter SQL called during the Build Package process. SQL verifies the table built from SQL has indices. This field is only used for non-SAP sources. If this field is blank, the new table in SQL Server will not have indices.                                                                                                                                                  |
| SAP Table Check SQL       | Enter SQL called during the Build Package process to verify if the table is Transparent, Pooled, Clustered or Other. Tables are not created for objects (views, structures, etc.) marked as “other.” Pooled or Clustered tables must use a package type of BOA RFC or SAP RFC. Transparent tables must use a package type of CranPort, SSIS or Data Services.                  |
| SAP Column Download SQL   | Enter SQL called during the Build Package process.  Downloads all column information from the SAP DD03L table.                                                                                                                                                                                                                                                                 |
| SAP Primary Key SQL       | Enter SQL called during the Build Package process to download all column information from SAP DD03L table.                                                                                                                                                                                                                                                                     |
| ODBC Driver               | Enter name of driver used in the Windows ODBC setup for the DSN. The driver is used inside packages when performing data downloads. Collect uses .Net connections for performing tasks, but the packages still use these drivers. The ODBC driver for Oracle and SQL Server can remain blank because the default drivers are pre-built in the systems for the applicable DBMS. |
| OLE Provider              | Enter OLE settings. Only used for OLE type of connections. Oracle and DB2 have better support for Unicode characters using OLE connection type.                                                                                                                                                                                                                                |
| Connection String Example | Enter an example of information for clients to reference.                                                                                                                                                                                                                                                                                                                      |
| Left Column Delimiter     | Enter character that wraps around special characters in column and table names. SAP uses slashes in table names, which need to be wrapped in delimiters to prevent SQL errors.                                                                                                                                                                                                 |
| Right Column Delimiter    | Enter character that wraps around special characters in column and table names. SAP uses slashes in table names, which need to be wrapped in delimiters to prevent SQL errors.                                                                                                                                                                                                 |

1.  Click **Save**.
2.  Close *Vertical* View.

### Data Type Conversions

When you create connection types in Collect, you can set and update data
type conversions using the Connection Type Data Conversion page. You can
apply validation rules that are used to ignore, error out, or accept
specific data type conversions from a Source to a Target.

Watch Video: Set Up and Update Data Type Conversions

To Set Up a Data Type Conversion:

1.  Click **Data Type Conversions** for the Source Connection Type to
    configure the data type conversions for the connection type.

2.  Click **Add**.
    
    [View the field descriptions for the Connection Type Data Conversion
    page](../Page_Desc/Connection_Type_Data_Conversion_H)

3.  Enter a sort value in **PROCESS ORDER** field to determine the order
    in which the Data Type validation rules are processed.
    
    **NOTE:** BackOffice recommends having all error conditions first
    followed by accept conditions. The default can be set to accept any
    other data type or to error out any data type not found in the data
    type condition process.

4.  Select a validation rule (coded within the DTS Build process) from
    **DATA VALIDATE CONTROL** list box to validate data. Values are:

<!-- end list -->

  - Any Scale Greater Than 0

  - Data Type and Length Match

  - Data Type and Scale Match

  - Data Type Match Only

  - Data Type, Length and Scale Match

  - Data Type, Precision and Scale Match

  - Default for any Data Type

  - Greater Than or Equal Maximum Length

<!-- end list -->

17. Select a flag from **PROCESS FLAG** list box to determine how data
    is processed. Values are:

<!-- end list -->

  - **Accept –**  accepts data validate controls

  - **Error – ** errors out process

  - **Ignore –** columns of defined data type are ignored when building
    a package.

<!-- end list -->

18. Enter a type (from source) in **DATA TYPE** field, e.g., Image,
    Text, Strg, or Any.

19. Enter a length (from source) in **DATA LENGTH** field. Enter 0 if
    the field does not require a length.

20. Enter a type format (from target) in **NEW DATA TYPE FORMAT** field.
     
    
    **NOTE:** The NEW DATA TYPE FORMAT is the format for the new type of
    data to be defined in the target. It is defined in SQL Server and
    must contain the length or the scale.

21. Click **Save**; the *Vertical* View displays.
    
    [View the field descriptions for the Connection Type Data Conversion
    page's Vertical
    View](../Page_Desc/Connection_Type_Data_Conversion_H)

22. Enter a precision, the total number of digits (from source), in
    **Data Precision** field. Enter **0** if the field is not a numeric
    field.
    
    **NOTE:** Data Precision only applies to numbers, but the total
    digit count of the number and this value match to the download data.

23. Enter a scale, the number of digits after decimal point (from
    source), in **Data Scale** field. Enter **0** if field is not a
    decimal field.
    
    **NOTE: Data Scale** applies to numbers containing decimals. This
    field must match the downloaded number of decimals.

24. Enter a type in **New Data Type** field for the field in target,
    e.g., Image, Text, Strg, or Any.

25. Enter a length in **New Data Length** field for the field in target.
    Enter **0** if the field does not require a length.

26. Enter a precision (total number of digits) in **New Data Precision**
    field for the field in target. Enter **0** if the field is not a
    numeric field.
    
    **NOTE:** **New Data Precision** only applies to numbers, but the
    total digit count of the number and this value matches to the
    download data.

27. Enter a scale (number of digits after decimal point) in **New Data
    Scale** field for the field in target. Enter **0** if field is not a
    decimal field.
    
    **NOTE:New Data Scale** is the scale of the decimal being created.

28. Enter a template in **Column Override Template** field.
    
    **NOTE:** The **Column Override Template** is used to convert a
    source column into a new format in the target database. Enter **0**
    if the field is not a decimal.

29. Click **Save**.

SQL commands used to read the DBMS tables for table and column
information are stored in Collect. The Data Types have been customized
for each DBMS in combination with SAP data types defined in DD03L. In
order to support loading data in the Target database, the packages must
be manually built for connections that do not have system tables. For
example, Access and Top Speed are file-based storage databases. Excel
spreadsheet data can be imported via a manual package. 

SQL Server and Oracle are connection types built into Collect. There is
a process to build customized ODBC connections against Sybase, Informix,
DB2, etc. A customized ODBC connection uses the connection string only
in the Connection table and must be completely populated with the user
ID and password.
