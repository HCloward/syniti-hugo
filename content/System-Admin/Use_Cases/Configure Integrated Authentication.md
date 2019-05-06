# Configure Integrated Authentication

If the Support Integrated Authentication check box is enabled on the
*[Parameters](../Page_Desc/Parameters_All_TabsSysAdmin.htm)* page,
corporate system user IDs are permitted to log in to the Platform. The
Platform uses the corporate ID and cross-references it with the local
Platform ID. After a user has successfully been authenticated by the
corporate system and logged in to a computer, the Platform can be
started without an additional login.

Integrated Authentication is typically used in a Windows Domain
environment. Integration with other authentication providers is also
possible.

**NOTE**: If the site uses Integrated Authentication, users can be added
to WebApp groups on initial log in. Refer to [Use Auto Register to Add
Users to WebApp Groups
Automatically](Use%20Auto%20Register%20to%20Add%20Users%20to%20WebApp%20Groups%20Automatically.htm)
for more information.

Authentication methods require configuration steps in IIS, in the file
system on the web server, and in the DSP®.

To enable Integrated Authentication at a high level:

1.  Disable IIS Enable Anonymous Access.
2.  Enable IIS Integrated Windows Authentication.
3.  Include the user’s corporate ID in the user’s account settings in
    the DSP®.

To enable Integrated Authentication in IIS and Windows:

1.  Open IIS Manager (under Administrative Tools).

2.  Expand the tree on the left and select the DSP virtual directory.

3.  Double-click the **Authentication** icon.

4.  Right-click **Anonymous Authentication** and select **Disable** from
    the list menu.

5.  Right-click **Windows Authentication** and select **Enable** from
    the list menu.
    
    **NOTE**: At this point the platform may not be accessible to all
    users.

<!-- end list -->

1.  Close IIS Manager.

2.  Locate the DSP Installation Directory in Windows Explorer.

3.  Right-click the DSP directory and select **Properties** from the
    list menu.

4.  Click the **Security** tab.

5.  Click **Edit**.

6.  Enter Authenticated Users in the **Enter the object names to
    select** field.
    
    **NOTE**: To browse for the Authenticated Users group, click the
    **Advanced** and **Find Now** buttons.

7.  Click **Check Names** button and verify that the name is recognized.

8.  Click **OK**.

9.  Select **Modify** from the **Permissions for Authenticated Users**
    option box.

10. Click **OK** to close the Permissions for DSP window.

11. Click **OK** to close the DSP Properties window.

12. Repeat steps \#9 – 16 to grant Modify permissions to the
    Authenticated Users group on all folders that are used by the DSP®
    and the WebApps. This will depend on which WebApps are installed and
    what file locations were chosen during the installation process.
    
    **NOTE**: The specific folders where permissions must be modified
    will be different at different sites. All folder locations accessed
    by the DSP® **must** have the appropriate permissions set, or errors
    will be reported.

To enable Integrated Authentication in the DSP®:

1.  Select **Admin \> Configuration \> Parameters** in the *Navigation*
    pane.

2.  Click the **Security Settings** tab.

3.  Click the **Support Integrated Authentication** check box.

4.  Click **Admin \> Security \> Users** in the *Navigation* pane.

5.  Click **Vertical View** for a user who will be accessing the DSP®
    using Integrated Authentication.

6.  Click **Edit**.
    
    *[View the field descriptions for the Users page’s Vertical
    View.](../Page_Desc/Users_H.htm#Users_V)*

7.  Enter the **Windows User Name**.
    
    **NOTE**: Use the format domain\\username. Do not provide a
    password.
    
    **NOTE**: A validation warning "User will not be able to login with
    basic authentication if password is NULL or empty" may appear. If
    users will only be logging in using Windows Integrated
    Authentication then accept the validation warning by clicking the
    Yes button; otherwise set a password.

8.  Confirm that Integrated Authentication has been configured correctly
    by accessing the site from a client computer (not the web server).
    Verify that the site can be accessed without the user having to
    provide credentials.
    
    **NOTE**: Perform the steps below if Integrated Authentication is
    the only supported authentication method and Basic is not required.

9.  Select **Admin \> Configuration \> Parameters** in the *Navigation*
    pane.

10. Click the **Security Settings** tab.

11. Click **Support Basic Authentication** check box to uncheck it.
