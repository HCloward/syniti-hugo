+++
title = 'Add a System Type Model Table'
solution = 'Platform'
+++

# Add a System Type Model Table

An Administrator performs this task to document which tables are
required to be populated when building the System Type.

The System Type model must be [added](Add_a_New_System_Type_Model)
before this task can be performed.

For the System Type import to work, all tables on the [System Types
Model Tables](../Page_Desc/System_Types_Model_Tables) page must
exist and contain data.

The following System Type models and associated tables are delivered
with the product:

System Type Model

Table Names

JDE

F0004

F9200

F9202

F9210

F9860

F98711

SAP

DD02L

DD02T

DD03L

DD04T

DD05S

DD07T

DD08L

**NOTE:** For the JDE and SAP System Type models, the data from the
customer’s JDE and SAP environment must exist in the tables.

To add a System Type model table in Common:

1.  Select **Configuration \> System Type Models** in the *Navigation*
    pane.

2.  Select the **SYSTEM TYPE MODEL** on the *[System Types
    Models](../Page_Desc/System_Types_Models_H)* page.

3.  Click **Add**.
    
    *[View the field descriptions for the System Types Model Tables
    page](../Page_Desc/System_Types_Model_Tables)*

4.  Enter text in the **TABLE NAME** text box.
    
    **NOTE:** Each table name listed needs to exist and be populated
    with data in order for the System Types to import the correct
    descriptions and check tables. Otherwise, the import fails.

5.  Click **Save**.
