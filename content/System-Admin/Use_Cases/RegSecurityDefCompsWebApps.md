+++
title = 'Register Security Definitions to Components (WebApps)'
solution = 'Platform'
+++

# Register Security Definitions to Components (WebApps)

**NOTE:** This section only applies to custom components and the three
delivered custom components: Construct, MC and dspCompose\_Data.

Once the security definition is fully defined, it is registered to the
DSP® component (i.e., the WebApp).  This registration limits the records
returned on the page for a particular user by the data elements assigned
to the user for the security definition. Binding is established between
a security definition and the column(s) on the page. The binding is the
linking of column(s) on the page to columns defined in the security
definition view that are used for comparison. When displaying records to
the user, the DSP® uses this binding to limit the displayed records to
only those values to which the user has access.

To register security definition to the DSP® component or a custom
WebApp:

Select **WebApps** in *Navigation* pane.

Click **Pages** icon for WEBAPP NAME.

Click **Security Definitions** for the page DESCRIPTION.

Click **Add**. 

[View the field descriptions for the Security Definition Pages
page](../Page_Desc/Security_Definition_Pages.htm)

Select name of security definition from **SECURITY DEFINITION ID** list
box.

Click **UPDATE USER DEFINITION ON SAVE** check box to enable it,
allowing records added by the user to be automatically added to the
user’s security key. This allows users to automatically have security
to the new data without the added step of manually granting security.

Click **Save**.

Click **Bindings** button to view the linking of column(s) on the page
to columns defined in the security view.

Click **Edit** icon for a COLUMN NAME.

[View the field descriptions for the Security Definition Column Bindings
page](../Page_Desc/SecurityDefPgColbindings.htm)

Select a column defined in the security definition view from **COLUMN
BINDING** list box.
