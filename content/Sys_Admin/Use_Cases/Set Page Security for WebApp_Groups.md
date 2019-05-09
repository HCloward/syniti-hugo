+++
title = 'Set Page Security for WebApp Groups'
solution = 'Platform'
+++

# Set Page Security for WebApp Groups

Rights to view, add, edit or delete data on a page in a WebApp are
defined by WebApp groups. Page rights are configured by granting WebApp
groups access to any of the following rights:

  - **Allow Select** – Members of the WebApp group can view the page and
    data on the page. Users may download the data, if download is
    supported in the page properties and WebApp Group.
  - **Allow Insert** – Members of the WebApp group can add data to the
    page, if insert is supported in the page properties and WebApp
    Group.
  - **Allow Update** – Members of the WebApp group can edit data on the
    page, if update is supported in the page properties and WebApp
    Group.
  - **Allow Delete** – Members of the WebApp group can delete the page
    or rows from the page, if delete is supported in the page properties
    and WebApp Group.

WebApp groups define authorization or access on a page by page basis. As
a new page is added to a WebApp, security to the page with full page
access is granted to the Power User and Power Designer WebApp groups.

Page rights override WebApp group rights. For example, if the WebApp
group permits deletion on a page, but the page security restricts it,
users assigned to the WebApp group are unable to delete records from the
page.

An Administrator can access two DSP® pages to set page security to a
WebApp Group.

  - On the *[Group Pages](../Page_Desc/Group_Pages.htm)* page, all pages
    that the WebApp Group can access display.
  - On the *[Page Groups]()* page, all WebApp Groups that have access to
    a specific page display.

The following general rules apply to WebApp groups:

  - Users cannot view the page or exercise any other page rights unless
    the ALLOW SELECT check box is enabled for the page.
  - If a user is assigned to several WebApp groups, the user is given
    the sum of page rights. For example, if Group 1 can select and
    insert data on a page, and Group 2 can select and delete data from
    the page, a user who is a member of both WebApp groups can select,
    insert and delete data on the page.

To assign pages to a WebApp group on the *[Group
Pages](../Page_Desc/Group_Pages.htm)* page:

1.  Click **WebApps** on *Navigation* pane.

2.  Click **Groups** for a WEB APP NAME.

3.  Click **Pages** for a GROUP NAME.

4.  Click **Add**.
    
    [View the field descriptions for the Group Pages
    page](../Page_Desc/Group_Pages.htm)

5.  Select page from **PAGE ID** list box.

6.  Click any check boxes to remove rights for the selected group on
    this page.
    
    **NOTE:** By default, the page is automatically given full access
    rights. Click a check box to disable specific rights.

7.  Click **Save**.

To assign pages to a WebApp group on the *[Page Groups]()* page:

1.  Click **WebApps** on *Navigation* pane.

2.  Click the **Pages** icon for a WEB APP NAME.

3.  Click **Page Groups** for a page.

4.  Click **Add**.:
    
    [View the field descriptions for the Page Groups
    page](../Page_Desc/Page%20Groups.htm)

5.  Select the group from the **GROUP ID** list box.
    
    **NOTE**: If all of a WebApp’s WebApp Groups have been granted
    security to the page, no options display in this list box.

6.  Click check boxes to set rights for the selected group on this page.
    
    **NOTE**: By default, the page is automatically given full access
    rights. Click a check box to disable specific rights.

7.  Click **Save**.
