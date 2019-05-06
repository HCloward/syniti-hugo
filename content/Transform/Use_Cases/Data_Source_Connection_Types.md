# Data Source Connection Types

In Transform, Sources and exports are associated with a CranPort or SSIS
package to either import or export data. These imports/exports can be
from comma-separated text files, Excel files, Access databases, SQL
Server databases or ODBC databases, such as DB2 and Oracle.

The CranPort or SSIS package contains two connections: Connection 1 and
Connection 2. For imports, Connection 1 is the data source database or
file and Connection 2 is the Transform object’s working SQL Server
database. For exports, Connection 1 is the Transform object’s working
SQL Server database and Connection 2 is the data source database or
file.

When Transform executes a CranPort or SSIS package, the package is
modified dynamically. As a result, Z-packages are created. For imports,
Connection 2 is changed to the DSP® data source that is associated with
the object. Therefore, if the data source for the object is changed, the
user does not have to recreate all the CranPort or SSIS packages; vice
versa for exports.

The Data Source Connection Type determines what happens with Connection
1 (for imports) and Connection 2 (for exports). There are four types:

  - **None** – Instructs Transform that there is not a CranPort or SSIS
    package and no import/export occurs.
  - **Protected Package** – Instructs Transform to leave the connection
    as it is. This is primarily used for ODBC data sources; however, it
    also works for flat files and SQL Server, in most cases. Protected
    Package requires the user to change the CranPort or SSIS package
    manually if conditions change, such if as the database name or the
    file directory are modified.
  - **Local File** – Assumes the Connection is a file path and remaps it
    to the naming convention. If it is assumed that the CranPort or SSIS
    package is built with an Excel file in My Documents, the connection
    contains the value C:\\Documents and Settings\\user name\\My
    Documents\\myimportfile.xls. Since the CranPort or SSIS package is
    executed by Transform and the platform, the file or a copy of it
    must be on the web server. The convention is that it should be
    located in a folder called C:\\Transform\\Sources\\Teams\\Target\\,
    where C:\\Transform\\Sources is a parameter. When executing a Local
    File, Transform looks for the file
    C:\\Transform\\Sources\\Team\\Target\\myimportfile.xls.
  - **Database** – Indicates the connection should be mapped to a data
    source registered in Common. This works for SQL Server connections.
    It allows the user to change the connection in one central location
    instead of in all the CranPort or SSIS packages. Refer to [Register
    a Data Source in
    Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
    for more information.
