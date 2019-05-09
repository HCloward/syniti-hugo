+++
title = 'Create a Dashboard Page'
solution = 'Platform'
+++

# Create a Dashboard Page

A Dashboard page can be created to display one or more charts.
Dashboards are associated with a layout to determine how the charts
display. A layout controls how and which charts display. DSP® comes
delivered with Layout Templates that can be copied but not modified.
Custom layouts can be created.

Layouts can also be added to the
*[Layouts](../Sys_Admin/Page_Desc/Layouts)* page. Refer to [Add
Layouts](Add%20Layouts) for more information.

**NOTE:** A layout that is currently assigned to a page cannot be
modified. This is because if it were modified, the changes would cascade
to all dashboards with potential undesired results. If a custom Layout
needs to be modified, it must be unassigned from the page.

The *[Layouts](../Sys_Admin/Page_Desc/Layouts)* page can be accessed
through the *Navigation* pane, but it is more often accessed as part of
creating a dashboard. The user clicks the + icon in the Layout ID field
on the *Vertical* View of the
*[Pages](../Sys_Admin/Page_Desc/Pages_H)* page to access the
*Layouts* page to add the layout as part of dashboard creation.

To create a Dashboard page:

1.  Select **Admin \> WebApps \> Pages** in the *Navigation* pane.

2.  Click **Add.**
    
    [View the field descriptions for the Pages
    page](../Sys_Admin/Page_Desc/Pages_H)

3.  Enter a description of the dashboard in **DESCRIPTION** field.

4.  Select **Dashboard** from **PAGE TYPE** list box.
    
    **NOTE**: Do not select a Table.

5.  Click **Save**.

6.  Either:
    
    Select the layout in the **Layout ID** list box and skip to step 18.
    
    OR
    
    Add a layout by clicking the **+** icon, the *Layouts* page
    displays.

7.  Enter a description of the dashboard in the **DESCRIPTION** field.

8.  Click **Filter** to select a **Layout Template ID,** the *Layout
    Template ID* page displays.

9.  Click **Save** next to the desired layout.

10. Click **Save** on the *Layouts* page.

11. Click the **Layout Frames** icon for the newly added layout, the
    *Layout Frames* page displays in a new tab.

12. Click **Edit** for a Frame.

13. Select a chart name from the **DEFAULT PAGE ID** list box.

14. Click **Save**.
    
    **NOTE**: Repeat the previous three steps and select the chart name
    to display in each frame of the dashboard.

15. Close the **Layout Frames** tab, and return to the *Pages* page.

16. Click **Edit**.

17. Select the dashboard from the **Layout ID** list box.

18. Click **Save**.

19. Close the *Vertical* View.
    
    **NOTE**: The Dashboard must be registered to the *Navigation* pane
    in the WebApp.

20. Locate **Dashboard** on *Pages* page.

21. Click **Vertical View**.

22. Click the **WebApp Name:  Switchboard** link for **Horizontal Menu
    ID**.

23. Click **Add**.

24. Enter **a number** in the **PRIORITY** field.
    
    **NOTE**: The Priority sets the order that page displays on the
    *Navigation* pane.

25. Select the created **Dashboard** page from **Link to Page ID** list
    box.

26. Click **Save**.
