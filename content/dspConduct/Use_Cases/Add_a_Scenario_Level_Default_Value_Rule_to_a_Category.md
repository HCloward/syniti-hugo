+++
title = 'Add a Scenario Level Default Value Rule to a Category'
solution = 'Master Data Management'
+++

# Add a Scenario Level Default Value Rule to a Category

A Designer can add a default value rule that indicates a default value
for a column and whether the value in the column is mandatory. Before
performing this task, a category and scenario must be added. Refer to
[dspConduct™ Design Process
Overview](dspConduct_Design_Process_Overview.htm) for more information
on creating elements in dspConduct™.

After a scenario level default value rule has been added to a category,
it can be assigned to a scenario in that category. Refer to [Assign a
Default Value Rule to a
Scenario](Assign_a_Default_Value_Rule_to_a_Scenario.htm) for more
information.

To add a scenario level default value rule to a category in dspConduct™:

1.  Select **dspConduct \> Design** in the *Navigation* pane.

2.  Click **Vertical View** for the category.

3.  Click **Edit**.
    
    [View the field descriptions for the Category page's Vertical
    View.](../Page_Desc/Category_H.htm#Category_V)

4.  Select the data source for the condition table in the **Condition
    Table Datasource Id** list box.

5.  Click **Save**.

6.  Click the **Rules and Actions tab**.

7.  Click the **Default Value Rules** icon.
    
    [View the field descriptions for the Default Value Rules
    page.](../Page_Desc/Default_Value_Rules.htm)

8.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.

9.  Enter a name for the rule in the **NAME** field.

10. Select the table from the **TABLE NAME** list box.

11. Select the column to which the rule applies in the **COLUMN NAME**
    list box.

12. Enter a value for the rule in the **CONSTANT** field.

13. Click the **IS MANDATORY** check box to enable it (optional).
    
    **NOTE**: If enabled, the default value is considered required and
    cannot be changed when the scenario is being executed within a
    request.
    
    **NOTE**: This configuration MUST be enforced by the Content WebApp.
    dspConduct™ does not enforce this setting.

14. Click **Save**.
