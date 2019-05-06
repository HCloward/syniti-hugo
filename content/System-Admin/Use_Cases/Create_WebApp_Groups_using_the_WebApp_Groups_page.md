# Create WebApp Groups using the WebApp Groups page

WebApp Groups can be designed depending on specific business
requirements. Any number of groups can be created. Users must then be
assigned to a WebApp Group.

Only users assigned to the Security and PowerUser WebApp Groups in
System Administration have authority to create a WebApp Group. However,
adding a user to PowerUser is not recommended. As new pages are created
for a WebApp, they are automatically added to the PowerUser WebApp
Group. Therefore, members of this group always have access to all pages,
unless otherwise configured. The ability to create WebApp Groups via the
*WebApp Groups* page is provided for the Security Administrator who
generally only has access to the security pages.

If using this method to create WebApp Groups, page access to the group
must be assigned under the WebApp Groups menu (Admin \> Security \>
WebApp Security \> Groups \> Users), which may not be available to the
Security Administrator.<span> </span>

<span style="font-weight: bold;">NOTE:</span> The Security Administrator
is a user who belongs to the System Administration Security WebApp
Group.

To create a WebApp Group using the *WebApp Groups* page:

1.  Select to **Security \> WebApp Security** in *Navigation* pane.

2.  Click **Groups** for a WEB APP NAME.

3.  Click **Add**.
    
    [View the field descriptions for the WebApp Groups
    page](../Page_Desc/WebApp_Groups_H.htm)

4.  Enter a unique name for the group in **GROUP NAME** field.

5.  Click **Save**.
    
    **NOTE**: The new Group name is synched with the list maintained on
    the *Groups* page (Admin \> WebApps \> Groups).

6.  Assign pages and page access to the group. Refer to [Set Page
    Security for WebApp
    Groups](Set%20Page%20Security%20for%20WebApp_Groups.htm) for
    detailed information.
