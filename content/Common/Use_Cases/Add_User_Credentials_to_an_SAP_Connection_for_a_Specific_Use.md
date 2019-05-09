+++
title = 'Add User Credentials to an SAP Connection for a Specific User'
solution = 'Platform'
+++

# Add User Credentials to an SAP Connection for a Specific User

An Administrator can add SAP Login credentials for specific users to
track that user’s updates posted to SAP.

If no user credentials have been added for the current user, the
platform uses the default credentials entered on the
<span style="font-style: italic;">Vertical</span> View of the [Data
Source
Registry](../Page_Desc/Data_Source_Registry_H#SAP_Application_Server_____-_General)
 page for an SAP Application Server connection type.

Before performing this task, gather information about the SAP instance,
such as the SAP application server name, system number and log in
credentials.

When downloading data from or posting data to SAP, the platform uses the
default credentials added on the <span style="font-style: italic;">[Data
Source Registry
p](../Page_Desc/Data_Source_Registry_H#Data_Source_Registry_V)</span>age’s
<span style="font-style: italic;">Vertical</span> View when connecting
to SAP. Refer to [Add Default User Credentials to an SAP
Connection](Add_Default_User_Credentials_to_a_Connection) for more
information.

To add credentials for a specific user in Common:

1.  Select <span style="font-weight: bold;">Configuration \> Data Source
    Registry</span> in the Navigation pane.

2.  Click <span style="font-weight: bold;">Vertical View</span> for the
    data source with an <span style="font-weight: bold;">APPLICATION
    DATA SOURCE TYPE</span> of SAP Application Server..

3.  Click the <span style="font-weight: bold;">User Credentials</span>
    icon.

4.  If no records exist, the page displays in add mode. Otherwise, Click
    <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Data Source Registry User
    Credentials
    page](../Page_Desc/Data_Source_Registry_User_Credentials_H)

5.  Select the user name in the
    <span style="font-weight: bold;">USER</span> list box.

6.  Click <span style="font-weight: bold;">Save</span>;
    <span style="font-style: italic;">Vertical</span> View displays.

7.  Select the language of the SAP instance if other than English in the
    <span style="font-weight: bold;">Language</span> list box.
    
    **NOTE:** The language is used when SAP interfaces with the platform
    and is used when logging in to SAP for the selected user.

8.  Enter the user name specific to this user the connection uses when
    logging in to SAP in the <span style="font-weight: bold;">SAP User
    ID</span> field.

9.  Enter the password specific to this user the connection uses when
    logging in to SAP in the <span style="font-weight: bold;">SAP
    Password</span> field.

10. Click <span style="font-weight: bold;">Save</span>.

11. Click the <span style="font-weight: bold;">Test Connection</span>
    icon to attempt to connect to the SAP instance using the supplied
    credentials.
