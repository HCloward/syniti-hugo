+++
title = 'Create Validation Views for Content WebApp Task Pages'
solution = 'Master Data Management'
+++

# Create Validation Views for Content WebApp Task Pages

A Designer can create a validation view for task pages with an active
variant that checks to confirm that required columns for a scenario \>
role \> task combination contain data. The validation checks every
column with the Required check box enabled on the
<span style="font-style: italic;">[Scenario Role Task
Column](../Page_Desc/Scenario_Role_Task_Column_H.htm)</span> page for
all pages in a task.

Refer to [Configure the Required Setting for a Scenario Role Task
Column](Configure_Required_Setting_Scenario_Role_Task_Column.htm) for
more information.

dspConduct™ creates a validation view for each required column. If a
column is required, the validation fails if there is no data in the
column on the page for this scenario \> role \> task combination. Other
scenario \> role \> task combination may use different column settings.

A validation view is also created for the default (\*) variant which
acts as a catch all for values in the variant column that could
potentially end up within the request content table and are not setup as
a variant on the task.

**NOTE**: The Request ID must be a key on the validation view when
building pages in the Content WebApp.

One validation is always created with the name web\[Page View’s Root
Name\] \_\[column name\]\_StarVariant\_isRequiredVal. This view is used
for validating against the Required checkmark on records under Scenario
Role Task Column with a ‘\*’ value for the variant name. An additional
validation view is created when a task has active variants named
web\[Page View’s Root Name\] \_\[column name\]isRequiredVal. Both views
should be used as a basis for page validations.

Refer to [Activate and Configure Column
Variants](Activate_Configure_Column_Variants.htm) for more information.

**NOTE**: Refer to [Create Tables and Views for Content WebApp Pages
Overview](Create_Tables_and_Views_for_Content_WebApp_Pages_Overview.htm)
 for general information.

**NOTE**: Once created, a Designer must register the view to the page in
the Content WebApp.

A Designer can also create required column validation views a specific
page in a task. Refer to [Create Validation Views for a Content WebApp
Task Page](Create_ValidationViews_Content_Page.htm) for more
information.

To create a validation view for task pages:

1.  Click **Design** in the *Navigation* pane.
2.  Click the **Scenarios** icon for a category.
3.  Click the **Roles** icon for a scenario.
4.  Click the **Tasks** icon for a role.
5.  Click the **Columns** icon for a scenario \> role \> task
    combination.
6.  Click the **Create Required Column Validations For All Column**
    icon.
