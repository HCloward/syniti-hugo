# View Results

After duplicates have been identified and resolved, review results to
verify the duplicate resolution is accurate.

To view results:

1.  Click **Analyze** in the *Navigation* pane.

2.  Click **Duplicates** for Data Source ID.

3.  Select an object.

4.  Click **Results** on Page toolbar.
    
    [View the field descriptions for the Results
    page](../../../Platform/Common/Page_Desc/Results.htm)

5.  Review the **RESULT STATUS** to determine if there are unresolved
    candidates that must be reviewed. Options are:
    
      - ** Green** – All duplicates have been resolved.
      - **Yellow** – Ten or fewer duplicates have been resolved.
      - **Red** – No duplicates have been resolved or if there are no
        records returned.
    
    **NOTE:** If there are unresolved candidates, click **Objects** icon
    on the Page toolbar and resolve the duplicate candidates.
    
    **NOTE:** To allow business users to see the results of the
    Duplicate Detection process:
    
    1.  Add the business user to the Common WebApp, then add the user to
        the Analyze WebApp Group. Refer to [Assign Users to WebApp
        Groups](../../../Platform/Sys_Admin/Use_Cases/Assign_Users_to_WebApp_Groups.htm)
        in System Administration for more information.
    2.  Assign a user-specific security definition to each business
        user. Add the Analyze data source(s) that are used in the
        Duplicate Detection process as a key to each user’s security
        definition. Refer to [Establish User-specific Security
        Definitions](../../../Platform/Sys_Admin/Use_Cases/Establish_UserSpecific_Security_Definitions.htm)
        in System Administration for more information.
