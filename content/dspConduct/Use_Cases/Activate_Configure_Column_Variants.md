+++
title = 'Activate and Configure Column Variants'
solution = 'Master Data Management'
+++

# Activate and Configure Column Variants

For a scenario \> role \> task combination, a Designer can define
variations in the Control Status and Required settings for a column when
a column value in a record meets a certain condition.

Before performing this task, the design process must be complete and a
task must be defined in the Content WebApp. Refer to [dspConduct™ Design
Process Overview](dspConduct_Design_Process_Overview.htm) for more
information.

In SAP, for each material type on the Material table, only a subset of
the fields are enabled, disabled, hidden, and required or not required.
For example, using a variant with the condition of material type column
= raw materials (MTART = ‘ROH') a Designer can change the default
Control Status for the Sales Price column to Hide because raw materials
are not sold.

Variants are first set up on the *[Task
Variant](../Page_Desc/Task_Variant.htm)* page. Refer to [Add a Variant
to a Task](Add_a_Variant_to_a_Task.htm) for more information about
setting up variants for a task. The variants are then activated on the
*[Scenario Role Task
Variant](../Page_Desc/Scenario_Role_Task_Variant.htm)* page. Once
active, the column settings for Control Status and Required can be
configured for the particular scenario \> role \> task combination.

To activate and configure variants for scenario role task columns in
dspConduct™:

1.  Select **dspConduct \> Design** in the *Navigation* pane.

2.  Click the **Scenarios** icon for a category on the
    *[Category](../Page_Desc/Category_H.htm)* page.

3.  Click the **Roles** icon.

4.  Click the **Tasks** icon on the Scenario (Roles) page.

5.  Click the **Variants** icon; the list of variants available for the
    task display on the Scenario Role Task Column page.
    
    [View the field descriptions for the Scenario Role Task Variants
    page.](../Page_Desc/Scenario_Role_Task_Variant.htm)

6.  Select one or more variants, and then click the Activate icon to
    enable the **ACTIVE** check box.
    
    **NOTE:** A variant is only applied to the parent page columns, not
    child level page columns associated with the parent page.

7.  On the [Scenario Role Task](../Page_Desc/Scenario_Role_Task_H.htm)
    page (parent pane), click the **Columns** icon.
    
    [View the field descriptions for the Scenario Role Task Column
    page.](../Page_Desc/Scenario_Role_Task_Column_H.htm)

To update the default column status value for one or more columns,
select the columns, and then click the **Enable Selected Columns**,
**Disable Selected Columns**, or **Hide Selected Columns** icon as
needed.

To update the required setting for one or more columns, select the
columns, and then click the **Require Selected Columns** or **Not
Require Selected Columns** icon as needed.
