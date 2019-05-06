# Configure a Data Services Repository

On the *Data Services Repositories* page, set up the Data Services
Repository to accept the Data Services Jobs.

When configuring a Data Services Repository, configure the Web Services
connection, then configure the connection to the repository database.

To configure a Data Services Repository in AutoGen:

1.  Click the **Automation** tab in the Quick Panel.

2.  Select the Object for which the Data Services Repository is being
    set up.

3.  Click the **Build and Refresh Data Services** icon in the Page
    toolbar; the *AutoGen Data Services* page's *Vertical* View
    displays.

4.  Select **Configuration\>Data Services Repositories** in the AutoGen
    *Navigation* pane.

5.  Click <span style="font-weight: bold;">Add</span>; the *Data
    Services Repositories* page's *Vertical* View displays.
    
    **NOTE:** If no records exist, the page displays in add mode.
    
    [View the field descriptions for the Data Services Repositories
    page.](../Page_Desc/Data_Services_Repositories_H.htm)

6.  Enter the name of the repository in the **Name** field.

7.  Enter the URL for the Data Services web service in the **Web Service
    Url** field.

8.  Enter the IP address for the CMS system in the **CMS System** field.

9.  Enter the login for the Data Services Repository in the **Login**
    field.

10. Enter the password in the **Password** field.

11. Select the authentication method from the **Authentication Method**
    list box.

12. Enter the operation timeout seconds in the **Operation Timeout
    Seconds** field.
    
    **NOTE:** The recommended setting for the Operation Timeout Seconds
    field is 600.

13. Click **Save**.

14. Click the **Test Wave Services Connection** icon.
    
    **NOTE:** If the connection fails, confirm the connection
    information to the Web services before testing the connection again.

15. Enter the IP address for the repository SQL server in the **Repo Sql
    Server Name** field.

16. Enter the repository SQL server database name in the **Repo Sql DB
    Name** field.

17. Enter the SQL server login ID in the **Repo Sql Login** field.

18. Enter the SQL server password in the **Repo Sql Password** field.

19. Click **Save**.

20. Click the **Test Repo Database Connection** icon to test the
    connection to the repository database.
    
    **NOTE:** If the information entered is confirmed correct and the
    connection fails, refer to SAP documentation for details about Data
    Services connections.

21. Click **Save**.
