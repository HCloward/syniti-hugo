+++
title = 'Set up ZSources'
solution = 'Migration'
+++

# Set up ZSources

ZSources are Source systems to which user security is granted. Users
with security to a ZSource are permitted to create data for the Source
system. When Source data (legacy) is moved from Source tables to Target
tables, the following occurs:

  - A ZSource field is added to the Target table.
  - The field is populated with a value indicating which Source system
    the row came from, for example, data from JDEdwards may contain
    “JDE.”
  - Data in the Target table indicates its origin.

For a user to view a ZSource:

  - The ZSource must be added to Construct

  - The user must be added to the specific ZSource

To register a ZSource in Construct:

1.  Click **ZSource** in the *Navigation* pane.

2.  Click **Add**.
    
    [View the field descriptions for the ZSource
    page](../Page_Desc/Z_Source)

3.  Enter a Source name in the **Z SOURCE** field.

4.  Click **Save**.

5.  Click the **Users** icon for the ZSource.

6.  Click **Add**.
    
    [View the field descriptions for the ZSourceUser
    page](../Page_Desc/ZSourceUser)

7.  Select a name from the **USER NAME** list box.

8.  Click **Save**.
