+++
title = ''
solution = 'Platform'
+++

## Add a Mass Change Custom Link to a Custom Page

In dspCompose<span style="font-weight: bold;">™</span>, if Mass Changes
should be allowed to the request data, the MassChange Custom Link must
be defined for the Data Entry page so that a user can access the
*Request Mass Change* page from the Data Entry page. An Administrator
must use the Custom Link WebApp Customization feature in System
Administration to add the link.

Refer to [Add Custom Links to a Page](Add_a_Custom_Link.htm) for more
information.

To add the custom link to the Data Entry page:

1.  Select **Admin \> Customization \> WebApp Customization** from the
    *Navigation* page.

2.  Click **Custom Links** for the custom WebApp name.
    
    **NOTE:** If no records exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    *[View the field descriptions for the Link Customization
    page](../Page_Desc/LinkCustomization.htm)*

3.  Select the page in the custom WebApp that will be the data entry
    page in the **PAGE ID** list box.

4.  Enter a unique column name in the **COLUMN NAME** field.
    
    **NOTE:** The suggested column name is
    <span style="font-weight: bold;">MassChange</span>.

5.  Select **All Views** in the **VIEW TYPE** list box.

6.  Select **Toolbar** in the **CONTROL** list box.

7.  Select **dspCompose: Request Mass Change** in the **LINK TO PAGE
    ID** list box.

8.  Click **Save**; *Vertical* View displays.

9.  Select **Legacy.Action.ProcessEdit** from the **Image ID** list box.

10. Select **Selected Row** from the **Bind From** list box.

11. Click **Save**.

12. Click the link under **the LINK TO PAGE ID** column on the
    *Horizontal* View of the *Link Customization* page.

13. Click **Edit**.
    
    *[View the field descriptions for the Custom Page Column Links
    page](../Page_Desc/Custom_Page_Column_Links.htm)*

14. Enter
    <span style="font-weight: bold;">RequestID=RequestID,boaUserID=boaUserid</span>
    in the <span style="font-weight: bold;">Binding Field Names</span>
    field.

15. Click **Save**.

**NOTE:** If the PAGE ID selected on the *Link Customization* page had a
previously defined Toolbar view, remove that definition or ensure that
the Toolbar view does not contain the same COLUMN NAME as the COLUMN
NAME defined for the MassChange Custom Link.
