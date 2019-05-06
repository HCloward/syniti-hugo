# Assign a Custom Page to a Template Role

To optimize flexibility in request processing, dspCompose™ allows a
Template Administrator to assign any page in any component in the
platform to a Data role. A user assigned to the role navigates to this
custom page by clicking the **Data Entry** button on the *Request
(Roles)* page. A Review role accesses the custom page while reviewing
the request.

<span style="font-weight: bold;">NOTE</span>: If the custom page should
allow a user to perform a mass change, refer to [Add a Mass Change
Custom Link to a Custom
Page](Add_a_Mass_Change_Custom_Link_to_a_Custom_Page.htm) for more
information.

**NOTE**: To add a custom page to a role at the template level, the
template must not be active or must be in Developer Mode. Refer to
[Modify an Active Template in Developer
Mode](Modify_an_Active_Template_in_Developer_Mode.htm) for more
information.

**NOTE**: dspCompose™ does not apply a Review filter set for a Review
role to a custom page.

To assign a custom page to a template role:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Vertical View** for the role.

5.  Click the **Page Settings** tab.

6.  Click the **Custom Page** check box to enable it.

7.  Click **Edit**.
    
    *[View the field descriptions for the Template (Role) page’s
    Vertical
    View.](../Page_Desc/Template_Role_H.htm#Template_Role_V_All_Tabs)*

8.  Select a component in the **WebApp ID** list box that contains the
    custom page.

9.  Select the custom page from the **Page ID** list box.
    
    **NOTE**: The page that corresponds to the Page ID opens when the
    user(s) assigned to the Data Entry or Review roles for the template
    click the **Data Entry** button on the *Request (Roles)* page.
    
    <span style="font-weight: bold;">NOTE</span>: Once a WebApp ID and
    Page ID have been saved for the custom template, the columns on the
    custom page can be viewed on the
    <span style="font-style: italic;">Template (Role Column)</span> page
    (Team \> Templates \> Roles \> Columns).

10. Click **Save**.
    
    <span style="font-weight: bold;">NOTE</span>: if assigning a custom
    page from a custom WebApp to a role, enter all the custom page
    information following these steps before generating the custom
    template (by clicking Generate Custom on the
    <span style="font-style: italic;">Templates</span> page).
