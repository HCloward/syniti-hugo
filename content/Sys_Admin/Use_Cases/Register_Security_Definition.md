+++
title = 'Register Security Definition'
solution = 'Platform'
+++

# Register Security Definition

**NOTE:** This section only applies to custom components and the three
delivered custom components: Construct, MC and dspCompose\_Data. After
creating the view, the Security Definition is created on the *Security
Definitions* page.  On this page, the view created in [Create a
View](Create_a_View.htm) is registered along with the necessary
description information about the Security Definition. 

To register the security definition in System Administration:

1.  Select **Security \> Security Definitions \> Security Definitions**
    in *Navigation* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Security Definitions
    page](../Page_Desc/Security_Definitions.htm)

3.  Enter a unique name of the definition in **SECURITY DEFINITION
    NAME** field. Use the following naming convention to help with
    versioning: **WebAppName.SecViewTables.Columns**.

4.  Select a data source where the security definition is registered
    from **DATA SOURCE ID** list box.

5.  Select the view created in the [Create a View](Create_a_View.htm)
    section from **DATA VIEW** list box.
    
    **NOTE:** Only views that reside in the DATA SOURCE ID are available
    in the DATA VIEW list box.

6.  Enter a brief description or explanation of the security definition
    in **DESCRIPTION** field.

7.  Click **Save**.

8.  Click **Keys** button to define key columns within the DATA VIEW
    that contain values by which security can be administered.

9.  Click **Add**.
    
    [View the field descriptions for the Security Definitions Keys
    page](../Page_Desc/Security_Definition_Keys.htm)

10. Select a column within the view from **COLUMN NAME** list box that
    contains values by which security can be administered.

11. Click **Save**.
