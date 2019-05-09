+++
title = 'Extract Data using IG Universal Connect in Collect'
solution = 'Platform'
+++

# Extract Data using IG Universal Connect in Collect

IG Universal Connect allows the DSP® to extract data from systems, which
are defined by the connector associated with a Boomi Process. The Boomi
Process also has an associated atom, the default execution environment
(for example, Dev, QA and Prod). The Boomi Process is associated with
the IG Universal Connect data source when it’s [registered in
Common](../Common/Use_Cases/Register_a_Data_Source_in_Common).

Collect does not automatically build tables or refresh
packages/Processes when a Connection Type of IG Universal Connect is
used. Essentially, the Target Source is a placeholder for a Boomi
Process that is built manually and registered via Collect. Collect then
takes care of the scheduled execution of that Boomi Process. When a
Connection Type of “IG Universal Connect” is selected at the Target
Source level, the package type of IG Universal Connect is set by default
for each Target Source Table and is not editable. When the Target Source
Tables are refreshed, the Boomi Process registered to the Target Source
Table executes and pulls data into a Target table in the DSP®.

**NOTE**: The table must exist in the Target database. Collect does not
build the table for Target Source Tables that are registered using an IG
Universal Connect package type.

Before performing these steps, the IG Universal Connect data source must
be [registered in
Common.](../Common/Use_Cases/Register_a_Data_Source_in_Common)

To create a Target Source to execute a Boomi Process:

1.  Select **Collect \> Targets** in the *Navigation* pane.

2.  Click the **Source** icon for the Target.

3.  Click **Add**.
    
    [View the field descriptions for the Target Source
    page](../Collect/Page_Desc/Target_Sources_H_Collect)

4.  Select the IG Universal Connect data source that was registered in
    Common in the **SOURCE** list box.

5.  Select **IG Universal Connect** in the **CONNECTION** **TYPE** list
    box.

6.  Click **Save**; *Vertical* View displays.

7.  Enter a description of the source in the **Description** field.

8.  Click the **Advanced Settings** tab to change the atom, if needed.

9.  Select the atom in the **Boomi Atom Override** field, if needed.
    
    **NOTE**: This field allows the user to run the Target Source
    refresh against a registered atom other than the one assigned to the
    default data source. Use this feature for testing purposes if there
    are multiple atoms set up on different DSP® server environments and
    the tests should be run against the different environments
    registered under the single tenant.

10. Click **Save** and close *Vertical* View.

11. Click the **Tables** icon.

12. Click **Add**.
    
    [View the field descriptions for the Tables
    page](../Collect/Page_Desc/Tables_H)

13. Enter the table name where the IG Universal Connect Process will
    write the data in the **TABLE** field.
    
    **NOTE**: This table must exist in the database registered as the
    Target in Collect.

14. Click **Save**.

15. Click **Cancel**.

16. Click **Vertical View**.

17. Click **Edit**.

18. Click the **Advanced Settings** tab.

19. Select the Boomi process to run during the table refresh.
    
    **NOTE**: A process ID must be selected for each table.

20. Click **Save**.

21. Click the **Refresh** icon on the Page toolbar.

The Boomi Process associated with each table executes to pull data into
the Target table. By default, a refresh deletes data from a table, as
well as adding and updating records. If the existing data must not be
deleted when the table is refreshed, check the Do Not Delete Data check
box on the Advanced Settings tab of the
*[Tables](../Collect/Page_Desc/Tables_H)* page’s *Vertical* View.

**NOTE**: The refresh can also be run on a schedule. Refer to [Schedule
Updates to Tables](../Collect/Use_Cases/Schedule_Updates_to_Tables)
for more information.
