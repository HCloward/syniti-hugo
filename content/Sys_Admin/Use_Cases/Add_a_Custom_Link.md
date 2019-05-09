+++
title = 'Add Custom Links to a Page'
solution = 'Platform'
+++

# Add Custom Links to a Page

Users can add Toolbar buttons with custom links to a DSP® page, without
the need for database changes, via registrations within the DSP®
exclusively. Custom page links added using the Custom Link feature are
retained during the upgrade process.

To add a custom link:

1.  Select **Admin \> Customization \> WebApp Customization** from the
    *Navigation* pane.

2.  Click the **Custom Links** icon for a WEB APP NAME.
    
    <span style="font-weight: bold;">NOTE:</span> If no records exist,
    the page automatically opens in Add mode. Otherwise, click **Add**
    
    [View the field descriptions for the Link Customization
    page](../Page_Desc/LinkCustomization).

3.  Select an option from the **PAGE ID** list box.
    
    **NOTE:** The custom link will be added to the selected page.

4.  Enter the name of the column that will be displayed as the custom
    link in the **COLUMN NAME** field.

5.  Select an option from the **VIEW TYPE** list box to indicate the
    view where the custom link displays.
    
    **NOTE:** Options are:
    
      - **All Views —** The link displays on all views for the page.
      - **Excel —** The link displays on the Excel template downloaded
        for Excel Integration. Refer to [Use Excel
        Integration](../../Excel_Int/Use_Excel_Integration) for more
        information.
      - **Horizontal —** The link displays on the *Horizontal* View
        only.
      - **Vertical —** The link displays on the *Vertical* View only.

6.  Select an option from the **VIEW TYPE** list box to indicate the
    view where the custom link displays.
    
    **NOTE:** The VIEW TYPE defines the view type, Horizontal, Vertical,
    or All, of the page where the custom link will appear.
    
    **NOTE:** The **CONTROL** list box has one option, Toolbar. The DSP®
    only allows adding custom links to the Toolbar.

7.  Select an option from the **LINK TO PAGE ID** list box.
    
    **NOTE:** When a user clicks the custom link, the selected page
    displays.

8.  Click **Save**; the *Vertical* View displays.
    
    [View the field descriptions for the Link Customization page's
    Vertical View.](../Page_Desc/LinkCustomization)

9.  Select an option from the **Bind From** list box.
    
    **NOTE:** This option sets the scope of which criteria will carry
    over during the link’s navigation. If the user chooses Selected Row,
    the selected row’s keys are included when binding against the target
    page.

10. Click **Save**. After the record is saved, the page name in the
    **LINK TO PAGE ID** field displays a hyperlink. Click the link to
    set advanced options. Refer to the [Custom Page Column
    Links](../Page_Desc/Custom_Page_Column_Links) field descriptions
    for details on each advanced option.
