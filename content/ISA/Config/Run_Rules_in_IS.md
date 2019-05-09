# Run Rules in IS

Run the rule to see the failed data.

To run a new rule in IS:

1.  Click the **Workspace Home** icon in the tree toolbar on the left
    side of the page.

2.  Click **Rule Results**.
    
    **NOTE:** In the pane on the left, expand the source connection and
    click the check box next to the table name that has the rule.

3.  Click **Calculate Score**.
    
    **NOTE:** This runs the rule.

4.  Enter the name in the **Name** field.

5.  Select the name of the database connection that was created to store
    the failed data in the **Save all field data to** list box.
    
    **NOTE:** This is where the data that fails the rule is stored. It
    **must** be the connection to the IsFailedData database.

6.  Click **Save and Run Now**.
    
    **NOTE:** Once the rule is run, view the results on the Workspace
    Home page.
    
    **NOTE:** After a rule is run, it may require editing.

To edit a rule:

1.  Click the **Tasks** icon in the tree toolbar on the left side of the
    page.
2.  Select the rule name.
3.  Click **Edit**.
4.  Ensure that the option in the **Save all failed data to:** list box
    is the name of the database connection to the **IsFailedData**
    database.
5.  This connection name must be selected for ISA to work. Refer to
    [Create a Database Connection to Store IS Failed
    Data](Create_a_Database_Connection_to_Store_IS_Failed_Data) for
    more information.
6.  Make changes to the rule as needed.
7.  Click **Save and Run Now** to test the changes.
