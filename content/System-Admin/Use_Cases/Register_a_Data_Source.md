# Register a Data Source

<span style="font-weight: bold;">NOTE:</span> It is recommended that
data sources be registered in Common instead of System Administration. A
Data Services data source must be registered in Common and cannot be
registered in System Administration.

During the installation or implementation of the Data Stewardship
Platform (DSP®), additional Data Sources, other than what are provided
in the installation package, may be required. This use case provides
step-by-step instructions and requirements to configure database
connection settings for Data Sources utilized by the DSP®.

<span style="font-weight: bold;">NOTE:</span> If a data source is
deleted in Common, the corresponding data source is deleted in System
Administration. If a data source is deleted in System Administration,
the Common data source is not deleted.

Refer to [How the DSP Uses Data Source
Types](HowDSPUsesDataSourceTypes.htm) for more information.

To register a Data Source in System Administration:

1.  Navigate to **Admin \> Data Sources** in the *Navigation* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Data Sources
    page.](../Page_Desc/Data_Sources_HSysAdmi.htm)

3.  Enter the data source name in the **DATA SOURCE NAME** field.

4.  Select a data source type from the **DATA SOURCE TYPE** list box if
    the default value (SqlServer) is not applicable. Options are:
    
      - **Local File** – Points to a folder on the web server. Used for
        importing or exporting data to flat files: Excel, CSV, etc.
    
      - **ODBC** – Generally for databases other than Oracle and
        Microsoft SQL Server, if the ODBC driver is available.
    
      - **OleDB** – Generally for databases other than Oracle and
        Microsoft SQL Server, if the OleDBdriver is available.
    
      - **Oracle** – Used for configuring connections to Oracle
        databases that use native connection drivers.
    
      - **Remote File (FTP)** – Similar to local file, but located on
        another machine and accessed through the File Transfer Protocol.
    
      - **Remote File (HTTP)** – Similar to local file, but located on
        another machine and accessed through the Hypertext Transfer
        Protocol.
    
      - **Remote File (UNC)** – Similar to local file, but located on
        another machine and accessed through the Uniform Naming
        Convention.
    
      - **SqlServer** – Used to connect to a Microsoft SQL Server, using
        native connection drivers.

5.  Click **Save**; the *Vertical View* displays.
    
    **NOTE:** The configuration of the *Vertical* View depends on the
    Data Source Type selected on the *Horizontal* View. This example
    walks through the most common Data Source Type: SQL Server. For
    configuration options for other Data Sources Types, refer to the
    [Data Sources page’s Vertical
    View](../Page_Desc/Data_Sources_HSysAdmi.htm#Data_Sources_V_All_Tabs)
    field descriptions.

6.  Select an address from **Server Address** combo box.
    
    **NOTE:** The **Server Address** combo box contains the server
    address from existing data sources registered in the Platform. This
    list can be used as suggestions where an existing server address can
    be selected. To add a new server address, type the address in the
    **Server Address** field and click **Use this value**.

7.  Enter a name in **Database** field.
    
    **NOTE:** The **Database** name must be the name of the database
    <span style="font-weight: bold; color: #ff0000; text-decoration: underline;">exactly</span>
    as it appears in the database. For Oracle databases, the
    **Database** name appears in the TNS name file.

8.  Select a database user name from **User ID** combo box.
    
    **NOTE:** The **User ID** combo box contains the user IDs from
    existing data sources. This list can be used as suggestions where an
    existing user ID can be selected. To add a new user ID, enter the
    user in the **User ID** field and click **Use this value**.

9.  Enter the password associated with the User ID in **Password**
    field.
    
    **NOTE:** The **User ID** and **Password** fields are only available
    for Data Source Types of SQL Server, Oracle, OLE and ODBC.

10. Click the **Advanced Properties** tab.

11. Enter a value in the **Port** field.
    
    **NOTE:** Some databases can be configured to run on the non-default
    port. The **Port** field allows users to enter the server that uses
    a different port. Also, the **Port** field is used for FTP
    connections to define the target port.

12. Click the **Trusted Connection** checkbox to enable it.
    
    **NOTE:** If the Server is configured to connect using Windows
    Authentication, the connection will use the hosting machine’s
    information to authenticate the connection. If enabled, **Trusted
    Connection** bypasses the usage of the User ID and Password fields.

13. Enter a value in the **Connection Timeout** field.
    
    **NOTE:** The **Connection Timeout** field denotes how long to wait,
    in seconds, when connecting to the server before executing any
    commands. If the server does not reply within this time, the
    connection action will be cancelled.

14. Enter a value in the **Command Timeout** field.
    
    **NOTE:** The **Command Timeout** field denotes how long to wait for
    a command execution against the server to wait for a reply. If no
    reply returns in this number of seconds, the action will be
    cancelled.

15. Click **Save**.

16. Click the **Test Connection** icon to test the connection to the
    Data Source, which verifies the database User ID and Password are
    connected to the database.
    
    **NOTE:** Additional drivers must be installed for Oracle, DB2,
    Informix or any other ODBC Data Source. If the local database
    Administrator or data audit team does not have a list of the
    additional drivers required for the data source, contact BackOffice
    Support at <http://support.boaweb.com/>.

17. Click the **Recompile Objects** icon to verify the data is available
    in the database.
    
    **NOTE:** Objects should only be recompiled for SQL Server databases
    created for the project. Objects may need to be recompiled a few
    times. If the recompile fails after three attempts, submit an issue
    to BackOffice Support: <http://support.boaweb.com/>.
    
    **NOTE:** When recompiling a data source, SQL inline Table-Valued
    functions are not supported.

18. Click the **Append Columns** button to append the BackOffice
    reserved columns used by the Framework to all tables that do not
    already contain them, a confirmation message displays. Use this
    option when creating a WebApp on the data source.
    
    **NOTE:** The following are BackOffice reserved columns: AddedBy,
    AddedOn, ChangedBy, ChangedOn, AddedVia and ChangedVia. If the
    **Protect** field is enabled for the assigned server, the tables in
    the database are
    <span style="color: #ff0000; text-decoration: underline; font-weight: bold;">not</span>
    appended with the BackOffice reserved columns.

19. Click **OK**.
