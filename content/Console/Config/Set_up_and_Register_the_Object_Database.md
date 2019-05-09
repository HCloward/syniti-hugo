+++
title = 'Set up and Register the Object Database (dsw\*)'
solution = 'Migration'
+++

# Set up and Register the Object Database (dsw\*)

**NOTE**: Databases should not be added before consulting the on-site
DBA or technical lead on the project. Database and server settings and
parameters play into the creation of every database and if not set up
correctly can lead to severe performance issues.

To create and register the object database:

1.  Launch and log in to Microsoft SQL Server Management Studio.

2.  Click the **+** icon on the root SQL Server Group.

3.  Click the **+** icon on Database.

4.  Select **New Database**.

5.  Enter the name of the database in the **Database name** field.
    
    **NOTE**: Prefix the object database with “dsw.”

6.  Click the **Ok** button.

To add users to the newly added database:

1.  Click the **+** icon for the database.

2.  Click the **+** icon for Security.

3.  Click the **+** icon for Users.

4.  Right-click **Users** and select **New User**.

5.  Enter the User Name **CranSoft**, the Login name **CranSoft** and
    the Default Schema **dbo** and click the**OK** button.
    
    **NOTE**: If a different CranSoft login was set up during
    installation, assign that login here. For the purposes of this
    document, “CranSoft” is used as the server login setup name (as
    suggested in the BOA Solutions Installation and Upgrade Manual).

6.  Right-click the CranSoft user.

7.  Select **Properties**.

8.  On the Owned Schemas tab, check the **db\_owner** check box.

9.  On the Membership tab, check the **db\_owner** check box.

10. Click the **OK** button.

11. [An Administrator must then register the data source in System
    Administration.](../../../Platform/Sys_Admin/Use_Cases/Register_the_Object_Database_\(dsw_\)_in_System_Administration)

After the data source has been registered:

1.  Select **dspMigrate \> Waves \> Process Areas \> Vertical View** of
    an Object.

2.  Click **Edit**.
    
    [View the field descriptions for the Process Area: Object
    page](../Page_Desc/Process_Area_ObjectH)

3.  Select the Object database in the **Data Source ID** list box.

4.  Click **Save**.
