+++
title = 'Create Tables and Views for Content WebApp Pages Overview'
solution = 'Master Data Management'
+++

# Create Tables and Views for Content WebApp Pages Overview

A Designer can create control tables and views, including Page Control
Views (PCV), Data Control Views (DCV) and validation views, for a
scenario \> role \> task combination. These objects are created and
stored in the Content WebApp’s database.

Tables and control views are based on the Content WebApp page’s column
settings for control status (Hide, Enable, Disable) set in dspConduct™.
Refer to [Configure Column Status for a Task for a Scenario Role
Combination](Configure_Column_Status_for_a_Scenario_Role_Task.htm) for
more information.

If a task has active variants assigned under any scenario \> role
combination in the category, dspConduct™ builds a DCV. In other words, a
specific scenario \> role \> task combination may not have an active
variant. However, if the task has an active variant in a different
scenario \> role \> task combination, dspConduct™ builds the DCV.

If a task does not have active variants in any scenario \> role \> task
combinations in the category, dspConduct™ builds a PCV.

Refer to [Activate and Configure Column
Variants](Activate_Configure_Column_Variants.htm) for more information.

<span style="font-weight: bold;">NOTE</span>: A Designer must register
views to a page(s) in the Content WebApp.

<span style="font-weight: bold;">NOTE</span>: The prefix of the table
name can be updated if needed. Refer to [Set the Control Table
Prefix](Set_the_Control_Table_Prefix.htm) for more information.

To generate page validations and page control views:

1.  Create a control table that contains a list of relevant columns from
    the page table registered to the corresponding Column PageID on the
    <span style="font-style: italic;">[Scenario Role Task
    Column](../Page_Desc/Scenario_Role_Task_Column_H.htm)</span> page.
    This table stores the data to be used as the basis for DCVs and
    PCVs. Refer to [Generate a Control Table for Content WebApp
    Pages](Generate_a_Control_Table_for_Content_WebApp_Pages.htm) for
    more information.
    
    **NOTE:** Relevant columns are columns used for data entry, not
    internal reserved columns.
    
    **NOTE:** If the control tables and control views have already been
    created, a Designer can click the Create Control Table icon on the
    [Scenario Role Task Page](../Page_Desc/Scenario_Role_Task_Page.htm)
    page to drop and rebuild the table and repopulate the control data.
    When the Create Control Views button is clicked, dspConduct™ changes
    any existing control views back to their initial creation state
    (losing any modifications).

2.  Create the control view or change the control view if it already
    exists and a new column has been added to the page. Refer to
    [Generate Control Views for Content WebApp
    Pages](Generate_Control_Views_for_Content_WebApp_Pages.htm) for more
    information.
    
    **NOTE:** A DCV  is created for a page with active variants and a
    PCV is created for a page without active variants.

3.  Create a validation view for each required column based on the
    Required setting on the <span style="font-style: italic;">[Scenario
    Role Task
    Column](../Page_Desc/Scenario_Role_Task_Column_H.htm)</span> page.
    Refer to  [Create Validation Views for a Content WebApp Task
    Page](Create_ValidationViews_Content_Page.htm) and [Create
    Validation Views for Content WebApp Task
    Pages](Create_Valid_Views_Task_Pages.htm) for more information.
    
    <span style="font-weight: bold;">NOTE:</span> If column
    configuration is updated on the
    <span style="font-style: italic;">[Scenario Role Task
    Column](../Page_Desc/Scenario_Role_Task_Column_H.htm)</span> page,
    the data in the control table can be updated with the Update Control
    Data button. In this case, the tables do not need to be rebuilt and
    views do not need to be updated to capture these sort of changes. If
    columns are added to or removed from the content page use the Update
    Column List icon on the <span style="font-style: italic;">Scenario
    Role Task Column</span> page to capture the column additions or
    subtractions, then rebuild the control table. Refer to [Update
    Control Table Data](Update_Control_Table_Data.htm) for more
    information.
