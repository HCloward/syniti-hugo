+++
title = 'Guidelines for the Navigation Pane'
solution = 'Platform'
+++

# Guidelines for the Navigation Pane

The *Navigation* pane on the left displays page links to the WebApp.

The following are the suggested menu links on the *Navigation* pane for
each WebApp (in this order, from top to bottom):

  - **WebApp Name** – Displays the name of the current WebApp with the
    proper trademark. This menu item links to the WebApp home page or
    message board.
  - **Configuration** – A submenu often created to link to the multiple
    pages available under Configuration. Each page under Configuration
    should display the *Navigation* pane at the left, with links to all
    configuration tables specific to the WebApp. It is suggested that
    every WebApp contain a link to the *Parameters* page that contains,
    at a minimum, the following fields: **Application Name**,
    **Version** and **Release Date**.

**NOTE:** The *Configuration* submenu often provides links to other
pages that can be used for list boxes on other pages within the WebApp.

The following are general menu guidelines:

  - Use a standard Navigation pane on all pages. The menu items on the
    Navigation pane vary depending on the WebApp.
  - Do not modify the Navigation pane labels that are automatically
    added by DSP® when a WebApp is created. If copying an existing
    WebApp to create a new WebApp, the Navigation pane links must be
    modified to link to the appropriate pages within the new WebApp.
    Refer to [Copy Page](Copy_a_Page_in_a_WebApp.htm) for more
    information.
  - Do not use labels for menus unless the name of the page needs to be
    different only when displayed on the menu.

**NOTE:** When a user navigates from one WebApp to another, the menu
displayed in the navigation pane is chosen from the target page the user
is loading. Most WebApps are accessed via the *Navigation* pane with a
link to the WebApp’s home page. The Horizontal Menu of that target page
is chosen, unless it is null where it will fall back to the Vertical
Menu. This menu will be the menu used for the entirety of the time the
user remains in this WebApp. The most common usage is to define the main
pages on the *Switchboard* menu and use that on most pages as the
Horizontal View. Submenus can be created and then registered on the
*Switchboard* menu to provide access to other top-level pages.
