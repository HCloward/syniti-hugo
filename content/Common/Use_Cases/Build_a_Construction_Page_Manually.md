+++
title = 'Build a Construction Page Manually'
solution = 'Platform'
+++

# Build a Construction Page Manually

When the construction page should not be generated automatically, build
the page manually.

To build the page in Target Design:

1.  Select **Design** in the Context bar.

2.  Click the **Targets**icon on the
    *[Design](../../../Migration/Design/Page_Desc/Design)* page.

3.  Select the **Sources** icon for a Target.

4.  Click **Add**.
    
    *[View the field descriptions for the Target Sources
    page](../../../Migration/Design/Page_Desc/Target_Sources_H_Design)*
    
    **NOTE**: The Add button is only available if the selected Target
    has a Design Status of In Design.

5.  Select **{Full Construction}** from the **SOURCE DATA SOURCE** list
    box.

6.  Click **Save**.

7.  Click the **Vertical View** icon for the newly added Source.

8.  Click **Edit**.

9.  Enter the page name in the **Construction Page ID** field.

10. Click **Save**.

After the page is built in Target Design:

1.  Create the underlying table for the page.
2.  Add the fields to be used on the page to the table.
3.  Build a CranPort package for the process to move the data entered in
    the Construct  page to the sdbDSPConstruct data source.
4.  Register the process in Collect as Target sdbDSPConstruct and Source
    of Construct with the table name of the table created for the
    manually constructed page.
5.  Add the Wave-Process Area ID to the page’s table to set security.
