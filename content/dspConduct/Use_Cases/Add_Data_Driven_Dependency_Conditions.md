+++
title = 'Add Data-Driven Dependency Conditions'
solution = 'Data Quality'
+++

# Add Data-Driven Dependency Conditions

A data-driven dependency condition identifies a condition within a field
when processing a scenario that determines whether a subsequent
dependent scenario or role is processed or if a workflow notification is
sent. Refer to [Add a Dependent Scenario](Add_a_Dependent_Scenario.htm)
for more information.

Before performing this task, [Design a Governance
Hierarchy](dspConduct_Design_Process_Overview.htm).

Once conditions are added to the category, the Designer assigns
conditions to a scenario dependency relationship.

Conditions can also be assigned to roles. Refer to [Assign a Condition
to a Role Dependency
Relationship](Role_Dependencies.htm#Assign_a_Condition_to_a_Role_Dependency_Relationship)
and [Add Dependencies to
Roles](Role_Dependencies.htm#Add_Dependencies_to_Roles) for more
information.

This topic contains the following sections:

  - [Data-driven Dependency Condition
    Example](#Data_driven_Dependency_Condition_Example)
  - [Add the Data-Driven Dependency
    Condition](#Add_the_Data-Driven_Dependency_Condition)
  - [View the Dependency Relationships for a Data-Driven Dependency
    Condition](#View_the_Dependency_Relationships_for_a_Data_Driven_Dependency_Condition)

## <span id="Data_driven_Dependency_Condition_Example"></span>Data-driven Dependency Condition Example

The following flowchart illustrates an example situation for using a
data-driven dependency condition:

![](../../../Resources/Images/DataDrivenDependencies.png)

The same logic applies to data-driven dependencies conditions for roles.
If a condition is met in a role, a subsequent role is processed.
Otherwise it is skipped.

Along with processing dependent scenarios or roles, conditions control
whether workflow messages are sent. If a scenario or role is not
processed, the workflow notifications are not sent.

If multiple conditions exist, if one of the conditions are not met,
processing stops and the role is automatically finished. If one data
record meets the condition, the workflow is sent and the role is not
automatically
finished.

## <span id="Add_the_Data-Driven_Dependency_Condition"></span>Add the Data-Driven Dependency Condition

To add data-driven dependency conditions to a category in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \> Design</span>
    in the *Navigation* pane.

2.  Click **Vertical View** for the category.

3.  Click **Edit**.
    
    [View the field descriptions for the Category page's Vertical
    View.](../Page_Desc/Category_H.htm#Category_V)

4.  Select the data source for the condition table in the **Condition
    Table Datasource Id** list box.

5.  Click **Save**.

6.  Click the **Conditions** icon.

<!-- end list -->

1.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.
    
    *[View the field descriptions for the Conditions
    page.](../Page_Desc/Conditions.htm)*

2.  Select the table name for the condition from the **TABLE NAME** list
    box.

3.  Select the column for the condition from the **COLUMN** list box.

4.  Select the operator for the condition from the **OPERATOR** list
    box.

5.  Enter a value for the condition in the
    <span style="font-weight: bold;">CONSTANT</span> field.

6.  Click
**Save**.

## <span id="View_the_Dependency_Relationships_for_a_Data_Driven_Dependency_Condition"></span>View the Dependency Relationships for a Data-Driven Dependency Condition

A Designer can view the scenarios or roles that use data-driven
dependency conditions at the category level.

Before performing this task, [Create a Category](Create_a_Category.htm),
[Add Data-Driven Dependency Conditions](#) and [Assign a Condition to a
Scenario Dependency
Relationship](Assign_a_Condition_to_a_Scenario_Dependency_Relationship.htm).

To view the dependency relationships for a data-driven dependency
condition in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Design** in the *Navigation* pane.
2.  Click **Vertical View** for the category.
3.  Click the **Conditions** icon.
4.  Click the **SCENARIO DEPENDENCIES** or **ROLE DEPENDENCIES** icon.

*[View the field descriptions for the Scenario Dependency Condition
page.](../Page_Desc/Scenario_Dependency_Condition.htm)*

*[View the field descriptions for the Role Dependency Condition
page.](../Page_Desc/Role_Dependency_Condition.htm)*
