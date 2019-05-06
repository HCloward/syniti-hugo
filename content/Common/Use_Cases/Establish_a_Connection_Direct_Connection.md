# Establish a Connection via a Direct Connection to the Application Server

This task is performed by an Administrator.

Before performing this task, gather information about the target system
instance, such as the application server name, system number and log in
credentials.

The connection allows for the set up and configuration of the target
system instances for Integrate and dspCompose™.

A connection can also be established through a Message Server. Refer to
[Establish a Connection via a Message
Server](Establish_a_Connection_via_a_Message_Server.htm) or more
information.

Refer to [Establish a Connection to a Target System
Overview](Establish_a_Connection_to_a_target_system_Overview.htm) for
general information.

<span style="font-weight: bold;">NOTE</span>: The steps below are used
when establishing an SAP connection. Information about connection types
to other target systems is available on the
<span style="font-style: italic;">[Data Source
Registry](../Page_Desc/Data_Source_Registry_H.htm#Data_Source_Registry_V)</span>
page’s Vertical View.

To establish a connection that directly connects to the Application
Server:

1.  Select <span style="font-weight: bold;">Configuration \> Data Source
    Registry </span>in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Data Source Registry
    page.](../Page_Desc/Data_Source_Registry_H.htm)
    
    **NOTE:** Though they are not marked as required on the page, the
    following fields are required when adding an SAP Application Server
    data source.

3.  Enter the data source name in
    <span style="font-weight: bold;">NAME</span> field.

4.  Select <span style="font-weight: bold;">SAP Application Server
    (%)</span> from the <span style="font-weight: bold;">APPLICATION
    DATA SOURCE TYPE</span> list box.

5.  Click <span style="font-weight: bold;">Save</span>; the
    <span style="font-style: italic;">Vertical</span> View displays.

6.  Enter a value in the <span style="font-weight: bold;">SAP System
    ID</span> field.
    
    **NOTE:** The SAP System ID is a three-character alpha-numeric
    identifier for the SAP system.

7.  Enter the name of the SAP server in the
    <span style="font-weight: bold;">SAP APPLICATION SERVER</span>
    field.

8.  Enter the SAP system number in the
    <span style="font-weight: bold;">SAP SYSTEM NUMBER</span> field.
    
    **NOTE:** The System Number is a two character integer that
    identifies the SAP instance. It is used as a parameter in the SAP
    GUI Logon client for the SAP connection. The SAP System Number
    displays in SAP on the SAP GUI Change Item screen.

9.  Enter a value in the **SAPMAX POOL SIZE**<span>field, if
    needed</span>.
    
    **NOTE**: Max Pool Size is a value to specify how many RFC
    connections are left open for the current user, even if the
    connections are not being used actively. A pooled RFC connection is
    allocated much faster than a new connection. Therefore, increasing
    the pool size minimizes the time needed to get a new connection.  
    However, if a connection is pooled, it is not available for other
    users. Typically, ABAP backend systems define an upper limit for the
    number of RFC connections. If this number has been fully allocated
    by pooled connections, then new users requesting a new connection
    may not succeed because the maximum number of connections allowed by
    the ABAP system has already been allocated.  
    Typically, the maximum pool size is kept very low and may even be
    set to 0. If there are substantially fewer concurrent users than the
    number of concurrent RFC connections to an ABAP system, then
    increase the pool size to improve performance.  
    The recommended setting for Max Pool Size is **10** in highly
    parallel environments.

10. Click <span style="font-weight: bold;">Save.</span>

Continue with [Add Default User Credentials to a
Connection](Add_Default_User_Credentials_to_a_Connection.htm) or [Add
User Credentials to a Connection for a Specific
User](Add_User_Credentials_to_an_SAP_Connection_for_a_Specific_Use.htm).
