# User Credentials in dspCompose™

Integrate and dspCompose™ templates use connections to a data source to
download data from a target ERP system. A process template posts data to
the SAP instance. The user credentials for the connection can be
supplied using different methods, allowing greater flexibility when
setting security.

For Integrate and dspCompose™, user credentials for the SAP connection
can be set:

<span style="font-weight: bold;">At the system level.</span> By default,
when downloading data from or posting data to SAP, the platform uses the
default credentials added on Common's
<span style="font-style: italic;">[Data Source
Registry](../../../Platform/Common/Page_Desc/Data_Source_Registry_H.htm#SAP_Application_Server_____-_General)</span>
page’s <span style="font-style: italic;">Vertical</span> View for the
SAP connection (unless another method is configured).

  - <span style="font-weight: bold;">At the user level by an
    Administrator.</span> An Administrator can use the
    <span style="font-style: italic;">[Data Source
    Registry](../../../Platform/Common/Page_Desc/Data_Source_Registry_H.htm#SAP_Application_Server_____-_General)</span><span style="font-style: italic;"></span> page
    to manage credentials for a user. If no user-specific credentials
    exist, the platform uses the system-level credentials. Refer to [Add
    User Credentials to an SAP Connection for a Specific
    User](../../../Platform/Common/Use_Cases/Add_User_Credentials_to_an_SAP_Connection_for_a_Specific_Use.htm)
    for more information.
  - <span style="font-weight: bold;">At the user level by a user on a
    page.</span> On pages where user credentials are required (e.g.,
    Integrate’s
    [Template](../../../Platform/Integrate/Page_Desc/Template_H.htm#Template_V_All_Tabs)
    page’s <span style="font-style: italic;">Vertical</span> View), a
    user credentials link displays that allows users to enter their
    user-specific credentials for the target system. Refer to [Add
    Stored Credentials as a User on a Page in Integrate or
    dspCompose](Add_Stored_Credentials_as_a_User_on_a_Page_in_Integrate_or_dspCompose.htm)
    for more information.
  - <span style="font-weight: bold;">At the user level using a Quick
    Link.</span> An Administrator user can add the
    <span style="font-style: italic;">[Data Source Registry User
    Credentials](../../../Platform/Common/Page_Desc/Data_Source_Registry_User_Credentials_H.htm)</span>
    page as a Quick Link. Using this method, access to the page is
    provided in Integrate or dspCompose™ on any page because users can
    access the Quick Link through the Site toolbar. On this page, users
    can add or edit their own user credentials for each target system.
