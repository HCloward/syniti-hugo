+++
title = 'Set a Baseline CTS Configuration for a Custom WebApp'
solution = 'Platform'
+++

# Set a Baseline CTS Configuration for a Custom WebApp

The CTS Configuration pages contain the settings used by the CTS process
to build packages.

If CTS’ing a custom WebApp, you much set the baseline configuration on
the CTS Configure pages before the CTS process can begin.

**NOTE:** Do not modify the CTS configurations for delivered DSP®
WebApps on these pages. This could break the CTS process for those
WebApps.

For general information about the CTS process, refer to [CTS
Overview](CTS_Overview.htm).

The baseline configuration can automatically generate:

  - All SQL objects that are contained in the data source for that CTS
    configuration
  - SQL object dependencies (including objects in multiple data sources)
    that define which objects are dependent on the object

**NOTE:** Dependencies can be detected automatically within the current
data source and others.

  - SQL Object relationships that define foreign and primary keys and
    binding field names for child objects

The user then adds:

  - The shippable items
  - The required keys for the shippable items
  - SQL Object Registrations, which define all additional objects that
    must be registered for a SQL object for the object to be moved via
    CTS. For example, an image object requires a registration for the
    image’s location, while a page object requires multiple
    registrations, for views and a table registration.

To create a baseline configuration for custom WebApps:

1.  Click **Admin \> CTS \> Configuration** in the *Navigation* pane.

2.  Click **Add**.
    
    *[View the field descriptions for the CTS Configure
    page](../Page_Desc/CTS%20Configure%20H.htm)*

3.  Select the data source for the custom WebApp in the **DATA SOURCE
    ID** list box.

4.  Click **Save**.

5.  Click the **Vertical View** icon.
    
    **NOTE:** On the *Vertical* View, the Trusted Cache check box is
    unchecked by default. This setting must remain unchecked for custom
    WebApps, or the CTS process will not work.

6.  Click the **Generate Config** button.

7.  Close **Vertical View**.

**NOTE:** The DSP crawls the data source and adds records on the CTS
Configuration pages.

Once this process is complete, access the following pages to confirm the
automatically generated configuration:

  - *[CTS Configure (SQL
    Objects)](../Page_Desc/CTS%20Configure%20SQL%20Objects.htm)* —
    Displays all objects in the data source for the CTS Configuration.
  - *[CTS Configure (SQL Object
    Dependencies)](../Page_Desc/CTS%20Configure%20SQL%20Object%20Dependencies.htm)*
    — Displays dependent object names in the current data source and in
    other data sources.
  - *[CTS Configure (SQL Object
    Relationships)](../Page_Desc/CTS%20Configure%20SQL%20Object%20Relationships.htm)*
    — Displays the child object and binding field names for related
    objects.

To add the shippable items and registrations to the CTS Configuration
for a custom WebApp:

1.  Select **Admin \> CTS \> Configuration** in the *Navigation* pane.

2.  Click the **Shippable Items** icon.

3.  Click **Add**.
    
    [View the field descriptions for the CTS Configure (Shippable Items)
    page](../Page_Desc/CTS%20Configure%20Shippable%20Items.htm)

4.  Enter the item name in the **Name** field.

5.  Enter a brief description in the **Description** field.

6.  Select the table name that stores the shippable item in the **Table
    Name** list box.

7.  Click **Save**.

8.  Click the **Keys** icon on the *CTS Configure* page.

9.  Click **Add**.
    
    [View the field descriptions for the CTS Configure (Shippable Item
    Keys)
    page](../Page_Desc/CTS%20Configure%20Shippable%20Item%20Keys.htm)

10. Enter a value in the **PRIORITY** field.

11. Select the name of the key in the **NAME** list box.
    
    **NOTE:** If the item is stored in a list box, complete the LIST
    TABLE, LIST VALUE FIELD, and LIST DISPLAY FIELD fields.

12. Click **Save**.

13. Click the **Registrations** icon on the *CTS Configure* page.

14. Click **Add**.
    
    [View the field descriptions for the CTS Configure (SQL Object
    Registrations)
    page](../Page_Desc/CTS%20Configure%20SQL%20Object%20Registrations.htm)

15. Select the name of the object to register to the CTS Config item in
    the **OBJECT NAME** list box.

16. Select the item in the **CTS CONFIG ITEM ID** list box.

17. Select the view name for the registration in the **VIEW NAME** list
    box.

18. Select the column from the **REQUIRED COLUMN** list box.

19. Click **Save**.

After the baseline configuration is complete, follow the steps in
[Create a CTS Package and Build Archive in Source
Instance](CreatePckgeBuildArcSrceInstance.htm).
