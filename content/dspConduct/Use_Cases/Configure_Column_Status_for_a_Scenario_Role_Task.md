+++
title = 'Configure Column Status for a Scenario Role Task'
solution = 'Master Data Management'
+++

# Configure Column Status for a Scenario Role Task

For a scenario \> role \> task combination a Designer can specify
columns to disable, enable, or hide on a particular task page to manage
exceptions for a scenario \> role \> task combination that might
otherwise require adding a new role.

Before performing this task, the design process must be complete and a
task must be defined in the Content WebApp. Refer to [dspConduct™ Design
Process Overview](dspConduct_Design_Process_Overview) for more
information.

The default settings for a column are based on the framework settings.
If no setting is defined in the framework, the database defaults are
used. Columns are defaulted to Enabled in the database. If a column is
nullable in the database, it defaults to not required.

Changing the column status on this page does not overwrite the default
settings established in the framework. Column variants can be set up to
configure the control status default for records with columns that meet
certain conditions. Refer to [Activate and Configure Column
Variants](Activate_Configure_Column_Variants) for more information.

**NOTE:** If, in the Content WebApp, a page can be updated through links
on other pages, it is possible that the page is in multiple tasks for
the same scenario \> role combination. So, if a column setting is
changed for one task, that column is updated in all tasks in which it is
used in a scenario \> role combination for all column variants. Refer to
[Add a Task](Add_a_Task) for more information about tasks and
[Activate and Configure Column
Variants](Activate_Configure_Column_Variants) for more information
about column variants.

To configure columns for a task in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span> **Design** in the *Navigation* pane.

2.  Click the **Scenarios** icon for a category on the *Category* page.

3.  Click the **Roles** icon.

4.  Click the **Tasks** icon on the *Scenario (Roles)* page.

5.  Click the **Columns** icon.
    
    *[View the field descriptions for the Scenario Role Task Column
    page.](../Page_Desc/Scenario_Role_Task_Column_H)*

6.  To update the default value for one or more columns, select the
    columns, and then click the <span style="font-weight: bold;">Enable
    Selected Columns</span>, <span style="font-weight: bold;">Disable
    Selected Columns</span>, or <span style="font-weight: bold;">Hide
    Selected Columns</span> icon as needed to update the **CONTROL
    STATUS** list box.
    
    Values are:
    
    **Disabled** – Column displays but is not editable.
    
    **Enabled** – Column displays and is editable.
    
    **Hide** – Column does not display.
