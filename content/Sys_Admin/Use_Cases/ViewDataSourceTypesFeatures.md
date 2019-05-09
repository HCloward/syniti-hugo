+++
title = 'View Data Source Types and Features'
solution = 'Platform'
+++

# View Data Source Types and Features

### Data Source Types

Data Source Types provide descriptions of the data source types in the
DSP. The DSP can use either databases (for example, SqlServer and
Oracle) or local and remote file types.

#### Database Data Sources

**ODBC**—Generally for databases other than Oracle and Microsoft SQL
Server, if the ODBC driver is available.

**OleDB**—Generally for databases other than Oracle and Microsoft SQL
Server, if the OleDB driver is available.

**Oracle**—Used for configuring connections to Oracle databases that use
native connection drivers.

**SqlServer**—Includes the following types of SQL Server Database
connections:

  - **Local Utility Database**—A SQL Server database hosted on the DSP
    database server.
  - **Migration Object Database**—A SQL Server database hosted on the
    DSP database server. BOA methodology states the db name must begin
    with 'dsw' and the database contains SQL objects for executing data
    transformation in a migration scenario.
  - **Migration Source Database**—A SQL Server database hosted on the
    DSP database server. BOA methodology states the db name must begin
    with 'sdb' and the database contains an image of a customer's legacy
    database in a migration scenario.
  - **Target System Database**— A SQL Server database hosted on the DSP
    database server. BOA methodology states the db name must begin with
    'dg' and the database contains an image of a customer's database. In
    a migration scenario, this is either a production database or one
    that mirrors production (for practice loads). In a
    governance/quality scenario, this is always a production database.

#### File Data Sources

File data source types cannot be registered in Common; they must be
registered in System Administration. They include the following file
types:

  - **Local File**—Points to a folder on the web server. Used for
    importing or exporting data to flat files: Excel, CSV, etc.
  - **Remote File (FTP)**—Similar to local file, but located on another
    machine and accessed through the File Transfer Protocol (FTP).
  - **Remote File (HTTP)**—Similar to local file, but located on another
    machine and accessed through the Hypertext Transfer Protocol (HTTP).
  - **Remote File (UNC)**—Similar to local file, but located on another
    machine and accessed through the Uniform Naming Convention (UNC).

Refer to [How the DSP Uses Data Source
Types](HowDSPUsesDataSourceTypes.htm) for more information.

### Data Source Type Features

Each file type has different features that may be used to support
certain functions in the DSP. Data Source Features are used to indicate
the support of certain functions of the DSP, like appending columns,
auditing and encryption. Certain features are available for specific
data sources. The *Data Source Features* page displays the various
feature names and descriptions of what DSP functions they support.

The only data source types that support data source features are Oracle
and SqlServer.

SqlServer includes the following available data source features:

  - Supports Append Columns
  - Supports Auditing
  - Supports Encryption
  - Supports Indexing
  - Supports Recompile Objects
  - Web App Data Source

Oracle includes the following available data source features:

  - Supports Append Columns
  - Supports Recompile Objects
  - Supports Sequences
  - Web App Data Source

To view data source types in System Administration:

1.  Click **Configuration \> Setup \> Data Source Types** in the
    *Navigation* pane.

2.  Click the **Features** icon for a data source type.
    
    **NOTE:** If the Protected check box is checked for a data source
    instance, data source features that make changes to the data source
    are hidden/disabled (for example, Recompile Objects, Append System
    Columns, building System Views, indexing, auditing, encryption, and
    building WebApps).

Refer to *[Data Source Features](../Page_Desc/DataSourceFeatures.htm)*
and *[Data Source Type
Features](../Page_Desc/DataSourceTypeFeatures.htm)* for more
information.
