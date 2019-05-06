# View SQL Server Health Charts

These charts display current data used to monitor system performance, to
troubleshoot memory issues, or to assist in performance tuning.  
This dashboard contains the following charts:

  - [Database: Current
    Connections](../Page_Desc/DatabaseCurrentConnections.htm)
  - [Database: Current
    Requests](../Page_Desc/DatabaseCurrentRequests.htm)
  - [Database: File Sizes](#View)
  - [Database: File Reads](#View2)
  - [Database: File Writes](#View3)
  - [Database: Memory Overview](#View4)

## View the Database: Current Connections Chart

Use the [Database: Current
Connections](../Page_Desc/DatabaseCurrentConnections.htm) page to view
databases currently connected to the DSP because of file reads, writes,
executing processes or other factors.

To access this chart in System Administration, select **Admin \>
Resources \> SQL Server Health \> Database: Current Connections** in the
*Navigation* pane.

## View the Database: Current Requests Chart

Use the *[Database: Current
Requests](../Page_Desc/DatabaseCurrentRequests.htm)* page to view
information about each database request per session ID that is executing
within the SQL server environment.

To access this chart in System Administration, select **Admin \>
Resources \> SQL Server Health \> Database: Current Requests** in the
*Navigation* pane.

## <span id="View"></span>View the Database: File Sizes Chart

Use the *Database: File Sizes* page to view the size in kilobytes of the
database file and database log file for each database associated with a
data source in the platform. This information can help track file size
growth that can impact system performance.

To access this chart in System Administration, select **Admin \>
Resources \> SQL Server Health \> Database: File Sizes** in the
*Navigation* pane.

## <span id="View2"></span>View the Database: File Reads Chart

Use the *Database: File Reads* page to view the percentage of total
files read, broken out by database, since the SQL Server database was
last active. Hover over a section for a record count. Each section lists
log reads and file reads for the selected database. Restarting SQLServer
will reset these values.

To access this chart in System Administration, select **Admin \>
Resources \> SQL Server Health \> Database: File Reads** in the
*Navigation* pane.

## <span id="View3"></span>View the Database: File Writes Chart

Use the *Database: File Writes* page to view the percentage of total
file writes being performed to data or log files, broken out by
database, since the SQL Server database was last active. Hover over a
section for a record count. Each section lists log writes and file
writes for the selected database. Restarting SQLServer will reset these
values.

To access this chart in System Administration, select **Admin \>
Resources \> SQL Server Health \> Database: File Writes** in the
*Navigation* pane.

## <span id="View4"></span>View the Database: Memory Overview Chart

Use the *Database: Memory Overview* page to view a breakdown of memory
usage (in megabytes) on the application server by available RAM and
Total RAM, page and available page. Since a lack of available memory
will cause locking and slowdown in performance, this data can be used to
monitor system performance and assist in performance tuning and
troubleshooting.

To access this chart in System Administration, select **Admin \>
Resources \> SQL Server Health \> Database: Memory Overview** in the
*Navigation* pane.
