# Register the Database for a Custom WebApp

The database must be registered as a data source in DSP® to create a
WebApp. In most cases, the System Administrator registers the database.

The database contains the tables and views needed to design the WebApp.
Additional views are automatically added from the DSP® after the data
source is added and the WebApp is created and validated. These views
pull in BOA views from the platform database. This is beneficial for
development when a user may not have security to the DSP® database or if
the WebApp is on a different server than the DSP® database.

To register the database:

1.  Log in to the DSP®.

2.  Click **Admin \> Data Sources** in the *Navigation* pane.

3.  Click **Add**.

4.  Enter a unique name in the **DATA SOURCE NAME** field.
    
    **NOTE:**   The Data Source Name is a logical name and may contain
    any alpha/numeric character, including spaces.

5.  Click **Save**, the *Vertical* View displays.

6.  Enter the server address where the data source is stored in the
    **Server Address** combo box.

7.  Enter the database name in the **Database** field.
    
    **NOTE:** The database name must match the actual name of the
    database located on the SQL Server.

8.  Enter the user account to access the database in the **User ID**
    field.

9.  Enter the password to access the database in **Password** field.
    
    **NOTE:** The Security or System Administrator may have to establish
    the **User ID** and **Password** to the database.

10. Click **Advanced Properties** tab.

11. Click **System Views** check box to enable it.
    
    **NOTE:  ** Having **SystemViews** checked will automatically
    install all BOA views into the data source. They are useful for
    applications that need to select data from the DSP® database.

12. Click **Test Connection** on the Page toolbar; a confirmation
    message displays.
    
    **NOTE:  ** If the connection is not made, verify the database name
    and login information are correct and try again.

13. Click **AppendColumns** on the Page toolbar, a confirmation message
    displays.
    
    **NOTE:** Refer to [*<span style="color: #0000ff;">Append BOA
    Reserved Columns to
    Tables</span>*](Append_BOA_Reserved_Columns_to_Tables.htm) for more
    information.

14. Click **OK**.
    
    **NOTE**: Use the **Recompile Objects** icon on the Page toolbar to
    recompile every object in a database to ensure they are still valid,
    if needed. A list of object names is returned if they fail to
    compile. The failed objects need to be manually fixed.
    
    **NOTE:** When recompiling a data source, SQL inline Table-Valued
    functions are not supported.
