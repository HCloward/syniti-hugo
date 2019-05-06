# Create Validation Views for a Content WebApp Task Page

A Designer can create a validation view for a page in a task with an
active variant that checks to confirm that required columns for a
scenario \> role \> task combination contain data. The validation checks
every column with the Required check box enabled on the
<span style="font-style: italic;">[Scenario Role Task
Column](../Page_Desc/Scenario_Role_Task_Column_H.htm)</span> page for
the page selected.

Refer to [Configure the Required Setting for a Scenario Role Task
Column](Configure_Required_Setting_Scenario_Role_Task_Column.htm) for
more information.

dspConduct™ creates a validation view for each required column for the
page in the task. If a column is required, the validation fails if there
is no data in the column on the page for this scenario \> role \> task
combination. Other scenario \> role \> task combinations may use
different column settings.

A validation view is also created for the default (\*) variant which
acts as a catch all for values in the variant column that could
potentially end up within the request content table and are not set up
as a variant on the task.

<span style="font-weight: bold;">NOTE</span>: The Request ID must be a
key on the validation view when building pages in the Content WebApp.

One validation is always created with the name web\[Page View’s Root
Name\]\_\[column name\]\_StarVariant\_isRequiredVal. This view is used
for validating against the Required setting on records under Scenario
Role Task Column with a ‘\*’ value for the variant name. An additional
validation view is created when a task has active variants named
web\[Page View’s Root Name\]\_\[column name\]\_isRequiredVal. Both views
should be used as a basis for page validations.

Refer to [Activate and Configure Column
Variants](Activate_Configure_Column_Variants.htm) for more information.

<span style="font-weight: bold;">NOTE</span>: Refer to [Create Tables
and Views for Content WebApp Pages
Overview](Create_Tables_and_Views_for_Content_WebApp_Pages_Overview.htm)
for general information.

<span style="font-weight: bold;">NOTE</span>: Once created, a Designer
must register the views to a page(s) in the Content WebApp.

A Designer can also create required column validation views for all
pages in a task. Refer to [Create Validation Views for Content WebApp
Task Pages](Generate_Control_Views_for_Content_WebApp_Pages.htm) for
more information.

To create validation views for a page:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the Navigation pane.
2.  Click the <span style="font-weight: bold;">Scenarios</span> icon for
    a category.
3.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    scenario.
4.  Click the <span style="font-weight: bold;">Tasks</span> icon for a
    role.
5.  Click the <span style="font-weight: bold;">Pages</span> icon for a
    scenario \> role \> task combination.
6.  Select one or more page records, and then click the
    <span style="font-weight: bold;">Create Validation Views</span> icon
    for a page.
