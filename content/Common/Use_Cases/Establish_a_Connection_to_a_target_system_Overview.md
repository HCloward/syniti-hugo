# Establish a Connection in a Target System Overview

Used in Integrate and dspCompose™, a template defines how data is posted
into an ERP system. Templates are not tied to data, but rather act as an
independent guide for posting that can be assigned to many processes.

Integrate and dspCompose™ templates use connections to a data source to
download data from a target system. A process template posts data to the
target system instance.  

The connection allows for the set up and configuration of these
instances for Integrate and dspCompose™.

This instance is used for:

  - Posting data (Integrate, dspCompose™, dspConduct™)

  - Gathering metadata about templates (Integrate)

  - Recording a BDC Script or GUI Script (Integrate, dspCompose™)
    
    **NOTE:** This is used for SAP connections only.

  - Providing an RFC/BAPI to use to post data (Common)
    
    **NOTE:** This is used for SAP connections only.

  - Providing a data source for transfer of user defined files (Common)
    
    **NOTE:** The instance to post data to or transfer files to may be
    overridden at the process post level.
    
    **NOTE:** When establishing a connection, the Administrator can
    configure the connection to directly connect to the Application
    Server or use a Message Server. A Message Server uses load balancing
    to manage Server resources and connects dynamically to an
    Application Server. Once connected using either method, there is no
    difference in functionality. Only one type of connection, direct or
    through a Message Server, can be created for a connection.
    
    **NOTE:** The system can use other methods to obtain user
    credentials. Refer to [User Credentials in
    dspCompose™](../../../Data_Quality/dspCompose/Config/User_Credentials_in_dspCompose.htm)
    or [User Credentials in
    Integrate](../../Integrate/Config/User_Credentials_in_Integrate.htm)
    for more information.
    
    **NOTE:** If a user adds a request based on this template and does
    not select a connection ID, the default connection assigned to the
    Integrate Template is used for the request. Refer to [Establish a
    Connection to a Target
    System](Establish_a_Connection_to_a_target_system_Overview.htm) for
    more information.

To establish a target system connection:

  - [Establish a Connection via a Direct Connection to the Application
    Server](Establish_a_Connection_Direct_Connection.htm) or
  - [Establish a Connection via a Message
    Server](Establish_a_Connection_via_a_Message_Server.htm)
  - [Add Default User Credentials to a
    Connection](Add_Default_User_Credentials_to_a_Connection.htm)
  - [Add User Credentials to a Connection for a Specific
    User](Add_User_Credentials_to_an_SAP_Connection_for_a_Specific_Use.htm)
