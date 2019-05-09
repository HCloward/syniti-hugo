+++
title = 'Manage BDC Screens and Fields'
solution = 'Platform'
+++

# Manage BDC Screens and Fields

<span id="Post Data using a BDC Script Steps" class="popUpLink">\>Review
the steps in the process. </span>

This optional step allows for BDC scripts to be manually modified to
remove or edit screens as well as remove or edit fields on screens.

BDC screen fields are individual fields that capture data during the BDC
script recording. If redundant steps were created during a recording or
if a step was left out, the screens can be manually added, deleted or
edited without having to re-record the script, regardless of the
recording mechanism used.

Fields can be edited or removed from each screen on the *BDC Screen
Fields* page.

**NOTE**: Screens and fields cannot be updated if the template is
active.

**NOTE**: If a user makes changes to screens or fields then records the
BDC script again for the template, Integrate overwrites these changes.

To manage BDC screen fields:

1.  Select **Categories** from *Navigation pane*.

2.  Click the **Templates** icon for a category.

3.  Locate the template with a type of BDC Script.

4.  Click **Vertical View**.

5.  Click **Configuration** tab.

6.  Click **BDC Screen** button.

7.  Click **Edit**; *Vertical* View displays.
    
    *[View the field descriptions for the BDC Screen page’s Vertical
    View.](../Page_Desc/BDC_Screen_H)*

8.  Enter a sort order value in **Priority**.

9.  Enter an SAP screen number name in **Screen Number**.

10. Enter an SAP program name in **Program**.

11. Click **Save**.

12. Click the **Fields** icon for a screen.
    
    **NOTE** The number displays the number of screen fields (those
    records that have the **Is Field** check box enabled). If **Is
    Field** is checked, the record represents a field in SAP and can be
    mapped to data in a process.

13. Click **Edit**.
    
    *[View the field descriptions for the BDC Screen Fields
    page.](../Page_Desc/BDC_Screen_Fields_H)*

14. Enter a sort order value in **PRIORITY**.

15. Enter an SAP field name in **FIELD NAME**.

16. Enter an SAP field value in **FIELD VALUE**.

17. Click **Save**.

18. Locate a field.

19. Click **Vertical View**.

20. Click **Advanced** tab to view additional screen field properties
    pulled from SAP.

**NOTE**: The field metadata is extracted from SAP for manually added
fields when the template is activated.
