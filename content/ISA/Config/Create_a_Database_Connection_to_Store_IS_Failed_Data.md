# Create a Database Connection to Store IS Failed Data

**NOTE:** Refer to the *Administrator Guide for Information Steward* for
additional information.

Set up the connection for the database that will store the data that
fails the IS rules.

Once data is extracted from the source and IS runs the rules on this
data, it is then written to this database.

To create a connection to the database that will store the failed data:

1.  At the CMC home page, click **Information Steward**.

2.  Select the **Connections** node in the tree panel at left.

3.  Click **Manage \> New \> Connection.**

4.  Enter the name of the database connection in the **Connection Name**
    field.
    
    **NOTE:** This is a free-form text field. There are no naming
    conventions for database connection names.

5.  Select **Database Connection** from the **Connection Type** list
    box.

6.  Select **For data that failed rules** from the **Purpose** list box.

7.  Select **Microsoft SQL Server** from the **Database Type** list box.

8.  Select the version of SQL the database instance is running on from
    **Database Version** list box.
    
    **NOTE:** The DSP® supports Microsoft SQL Server 2012 and Microsoft
    SQL Server 2014.

9.  Enter the IP address\\name of the server where ISA is installed in
    the **Server Name** field.

10. Enter **IsFailedData** in **Database Name** field.
    
    **IMPORTANT:** Enter this name exactly as it appears:
    **IsFailedData**
    
    **NOTE:** The connection must use this database name.

11. Enter the user name and password for the ISA server.

12. Retain the default values in the remaining fields
    (**UnsupportedDataTypes**, **VARCHARsize**, **Language**,
    **ClientCodePage**, and **ServerCodePage**).

13. Click **Save**.

14. Click **Test Connection** to confirm the connection.

Once rules are run in IS, the data that fails the rules are sent to the
IsFailedData database. The IsFailedData database is created in SQL
server when ISA is installed.

Two other databases, dspMonitor\_AccPak, the application database, and
dgRepository\_IS, which contains metadata information about IS, are also
created with ISA is installed.
