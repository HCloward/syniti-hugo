# Log Events and Access to Personal Data

The DSP® assists clients with corporate or regulatory compliance by
logging all events related to processing personal data. The logs are
created daily as .CSV files.

The DSP creates a log entry every time an event executes in DSP in any
application, including each page load. By default, events on all pages
are tracked; however, a System Administrator can [set which pages are
not tracked](Disable%20and%20Enable%20Logging%20for%20Pages.htm).

The log entry contains all information necessary to understand what was
executed and by whom, including:

  - Current Time
  - User ID
  - WebAppID
  - PageID
  - Page name
  - Event name
  - Primary Keys (if available)
  - DrillDownKeys (if available)

A System Administrator enables or disables logging as needed. By
default, logging is disabled.

Before logging can be enabled, a data source to store the logs must be
defined.

To define the data source:

1.  Create a local file data source. Refer to [Register a Data
    Source](Register_a_Data_Source.htm) for more information.
    
    **NOTE:** This data source’s path can be local on the web server or
    on a network. It is highly recommended that the logs be stored on a
    remote server.

2.  Test the connection to the data source.
    
    **NOTE:** The DSP must have read and write permissions to the data
    source.

If the logs cannot be written to the data source specified because of a
network or permissions issue, the logs are written to the installation
directory logs folder. BackOffice does not recommend writing these
events to a local file on the application server. The logs should be
written to a remote location, so as not to impact DSP performance, and
log size should be monitored using log management software. A warning
message displays in the DSP every hour that logs are written to the
installation directory logs folder.

To enable logging:

1.  Select **Admin \> Configuration \> Parameters** on the *Navigation*
    pane.

2.  Click the **Logging Options** tab.

3.  Click **Edit**.
    
    *[View the field descriptions for the Logging Options
    tab](../Page_Desc/Parameters_All_TabsSysAdmin.htm#Logging_Options)*

4.  Select the data source in the **Logging Data Source ID** list box.

5.  Click **Save**.

6.  Click the **Enable Page Logging** button.

7.  Set the **Logging Retention Days**, which is the number of days
    before the logs are deleted
    
    **NOTE:** The default value, 0, indicates that the logs are not
    deleted.

**NOTE:** The daily log also tracks when logging is enabled or disabled
and by whom.
