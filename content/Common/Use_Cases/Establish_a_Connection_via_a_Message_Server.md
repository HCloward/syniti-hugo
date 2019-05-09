+++
title = 'Establish a Connection via a Message Server'
solution = 'Platform'
+++

# Establish a Connection via a Message Server

Connecting to a target system  via a Message Server uses load balancing
to manage server resources. Load Balancing dynamically distributes the
SAP users to application server instances when connecting to the
Application Server. Load Balancing is used to download tables from the
source.

A connection can also be established directly with the Application
Server. Refer to [Establish a Connection via a Direct Connection to the
Application Server](Establish_a_Connection_Direct_Connection) for
more information.

<span style="font-weight: bold;">NOTE</span>: The steps below are used
when establishing an SAP connection. Information about connection types
to other target systems is available on
the<span style="font-style: italic;"> [Data Source
Registry](../Page_Desc/Data_Source_Registry_H#Data_Source_Registry_V)</span>
page’s Vertical View.

To establish an SAP connection that connects to the Application Server
through a Message Server in Common:

1.  Select <span style="font-weight: bold;">Configuration \> Data Source
    Registry </span>in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Data Source Registry
    page.](../Page_Desc/Data_Source_Registry_H)

3.  Enter the data source name in the
    <span style="font-weight: bold;">NAME</span> field.

4.  Select <span style="font-weight: bold;">SAP Application Server
    (%)</span> from the <span style="font-weight: bold;">APPLICATION
    DATA SOURCE TYPE</span> list box.

5.  Click <span style="font-weight: bold;">Save</span>; the
    <span style="font-style: italic;">Vertical</span> View displays.

6.  Enter a value in the <span style="font-weight: bold;">SAP System
    ID</span> field.
    
    **NOTE:**  The SAP System ID is a three-character alpha-numeric
    identifier for the SAP system.

7.  Enter the server name in the <span style="font-weight: bold;">SAP
    MESSAGE SERVER</span> field.

8.  Enter the group name in the <span style="font-weight: bold;">LOGON
    GROUP</span> field.

9.  Enter a value in the **SAPMAX POOL SIZE**field, if
needed.

<span style="font-size: 11.0pt;font-family: Arial, sans-serif;">**NOTE**:
Max Pool Size is a value to specify how many RFC connections are left
open for the current user, even if the connections are not being used
actively. A pooled RFC connection is allocated much faster than a new
connection. Therefore, increasing the pool size minimizes the time
needed to get a new connection.  
However, if a connection is pooled, it is not available for other users.
Typically, ABAP backend systems define an upper limit for the number of
RFC connections. If this number has been fully allocated by pooled
connections, then new users requesting a new connection may not succeed
because the maximum number of connections allowed by the ABAP system has
already been allocated.  
Typically, the maximum pool size is kept very low and may even be set to
0. If there are substantially fewer concurrent users than the number of
concurrent RFC connections to an ABAP system, then increase the pool
size to improve performance.  
The recommended setting for Max Pool Size is **10** in highly parallel
environments.</span>

1.  Click <span style="font-weight: bold;">Save</span>.

Continue with [Add Default User Credentials to a
Connection](Add_Default_User_Credentials_to_a_Connection) or [Add
User Credentials to a Connection for a Specific
User](Add_User_Credentials_to_an_SAP_Connection_for_a_Specific_Use).
