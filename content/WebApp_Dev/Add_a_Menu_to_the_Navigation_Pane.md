+++
title = 'Add a Menu to the Navigation Pane'
solution = 'Platform'
+++

# Add a Menu to the Navigation Pane

By default, a new WebApp has one menu created called *Switchboard*.
Menus can be registered within menus to allow sub menus to drill through
to other options inside the *Navigation* pane.

To create a menu:

1.  Click **Admin** \> **WebApps** on the *Navigation* pane.

2.  Click **Menus** for a WebApp.
    
    [View the field descriptions for the Menus
    page](../Sys_Admin/Page_Desc/Menus)

3.  Click **Add**.

4.  Enter a name in **MENU NAME** field.

5.  Click **Save**.

6.  Click **Menu Links**.
    
    [View the field descriptions for the Menu Links
    page](../Sys_Admin/Page_Desc/Menu%20Links)

7.  Click **Add**.

8.  Enter a number in the **PRIORITY** field.
    
    **NOTE:** The priority determines the order of the page links from
    top to bottom. Priority automatically sorts in an ascending order.
    The higher the priority, the lower an item displays in the
    *Navigation* pane.

9.  Select an image name in the IMAGE ID list box (optional).
    
    **NOTE:** This image displays to the left of the menu item in the
    *Navigation* pane.

10. Select the page that the menu option links to from the **Link to
    Page ID** list box (optional).
    
    **NOTE:**If there is page identified in the Link to Page ID field,
    the URL entered is ignored. Only one of these options can be used.
    
    **NOTE:** When a GUID displays in the **Link to Page ID** column, it
    indicates the page is an external WebApp. Do **not** alter or remove
    this menu link; it could render the WebApp not editable.

11. Enter the name that displays on the *Navigation* pane in **Label**
    field, if necessary.
    
    **NOTE:** If the Label field is left blank, the name of the target
    page displays in the Link to Page ID field, and this is translated
    automatically if enabled.

12. Select an option from **SUBMENUID** list box.
    
    **NOTE:** The **Submenu ID** determines the options on the main
    menu. For example, all menu links defined in Configuration display
    as a submenu under *Configuration* on the *Navigation* pane.

13. Enter a URL to which the menu options links (optional ).
    
    **NOTE:** If there is page identified in the Link to Page ID field,
    the URL entered is ignored. Only one of these options can be used.

14. Click **Save**.
