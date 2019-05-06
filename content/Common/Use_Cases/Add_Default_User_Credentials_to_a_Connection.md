# Add Default User Credentials to a Connection

This task is performed by an Administrator.

Before performing this task:

  - Gather information about the instance, such as the application
    server name, system number and log in credentials.
  - Add an SAP connection. <span style="font-size: 11.0pt;">Refer to
    [Establish a Connection via a Direct Connection to the Application
    Server](Establish_a_Connection_Direct_Connection.htm)  and
    [Establish a Connection via a Message
    Server](Establish_a_Connection_via_a_Message_Server.htm) for more
    information. </span>

Integrate and dspCompose™ templates use connections to a data source to
download data from a target system. A process template posts data to the
instance. Refer to [Establish a Connection to a Target System
Overview](Establish_a_Connection_to_a_target_system_Overview.htm) for
general information.

**NOTE**: If a user adds a request based on a template and does not
select a connection ID, the default connection assigned to the Integrate
Template is used for the request.

When connecting to SAP, the default credentials are used for all users
except for those with user credentials set on the
<span style="font-style: italic;">[Data Source Registry User
Credentials](../Page_Desc/Data_Source_Registry_User_Credentials_H.htm)</span>
page. Refer to [Add User Credentials to a Target System Connection for a
Specific
User](Add_User_Credentials_to_an_SAP_Connection_for_a_Specific_Use.htm)<span> </span>for
more information.

To add default credentials in Common:

1.  Select <span style="font-weight: bold;">Configuration \> Data Source
    Registry </span>in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Vertical View</span> for the
    SAP Connection.

3.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Data Source Registry
    page.](../Page_Desc/Data_Source_Registry_H.htm#Data_Source_Registry_V)

4.  Enter the SAP client number in the **SAPCLIENT field**.

5.  Select the language used<span>when SAP interfaces with the platform
    and when logging in to SAP
    in</span><span style="font-size: 11.0pt;">the
    </span><span style="font-size: 11.0pt;font-weight: bold;">SAP
    Language</span> list box.

6.  Enter the user name the connection uses when logging in to SAP in
    the **SAP User ID** field.

7.  Enter the user password the connection uses when logging in to SAP
    in the <span style="font-size: 11.0pt;font-weight: bold;">SAP
    Password</span> field.

8.  Click <span style="font-weight: bold;">Save</span>.

9.  Click the <span style="font-weight: bold;">Test Connection</span>
    icon to attempt to connect to the SAP instance using the supplied
    credentials.
