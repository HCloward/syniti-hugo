# Generate Control Views for Content WebApp Pages

A Designer can create views, including Page Control Views (PCV) and Data
Control Views (DCV), for a scenario \> role \> task combination. These
objects are created and stored in the Content WebApp’s database.

Before performing this task, [Generate a Control Table for Content
WebApp Pages](Generate_a_Control_Table_for_Content_WebApp_Pages.htm).

Views are based on a control table that has been generated when a user
clicked the Create Control Table icon on the
<span style="font-style: italic;">[Scenario Role Task
Page](../Page_Desc/Scenario_Role_Task_Page.htm)</span>page.  dspConduct™
reads in the control value for each column (Hide, Enable, Disable)
stored in the control table when building the view.

If a task has active variants assigned, dspConduct™ builds a DCV. Refer
to [Add a Variant to a Task](Add_a_Variant_to_a_Task.htm) for more
information.

When a DCV is built, three views are created:

  - A view for default columns with the naming convention web\[Page
    View’s Root Name\]\_StarDcv that is linked to the Control Table
  - A view for the column variant, named web\[Page View’s Root
    Name\]\_\[variant column name\]\_Dcv that is linked to the Control
    Table
  - A final DCV view named web\[Page View’s Root Name\]\_Dcv, as a union
    combining the other two views

If a task does not have active variants, dspConduct™ builds a PCV with
the naming convention web\[Page View’s Root Name\]\_Pcv.

**NOTE:** When generating views for content WebApp pages, dspConduct
checks to see if that Page is used in any task that has an active
variant.

<span style="font-weight: bold;">NOTE:</span> PVCs and DCVs are only
created for pages with a page type of Dynamic.

<span style="font-weight: bold;">NOTE:</span> At creation, these views
may not be fully functional based on the design of your Task Page These
can be used as a starting point. A Designer must complete and test the
created views before registering the views to a page(s) in the Content
WebApp. The Control Table contains ScenarioID and RoleID values that may
need to be added to the view, or used as join criteria to other tables,
or registered as Binding Fields in the Link to Page Column criteria. If
a change to the views is to be made, it is best practice to rename the
view so that if it was created or altered via the Create Control Views
event on the <span style="font-style: italic;">Scenario Role Task</span>
page, the changes made are not overwritten. Control views typically need
to factor in RequestID and RoleID as these methods are designed with the
intent to minimize dual maintenance of pages. In dspConduct™ you should
only have to ever build a single page to represent a table in your
enterprise data model. Use control views to display fields and events
differently based on variables such as BusinessProcessID, ScenarioID,
RoleID, and boaUserID.

To create a control view:

1.   Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Scenarios</span> icon for
    a category.
3.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    scenario.
4.  Click the <span style="font-weight: bold;">Tasks</span> icon for a
    role.
5.  Click the <span style="font-weight: bold;">Pages</span> icon for a
    scenario \> role \> task combination.
6.  Select one or more page records, and then click the
    <span style="font-weight: bold;">Create Control View</span> icon in
    the Page toolbar.
