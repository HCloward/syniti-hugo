+++
title = 'Merge or Copy BDC Screens to Another BDC Script Template'
solution = 'Platform'
+++

# Merge or Copy BDC Screens to Another BDC Script Template

<span id="Post Data using a BDC Script Steps" class="popUpLink">\>Review
the steps in the process. </span>

Once a BDC script has been recorded or imported into the BDC Script
template, the BDC screens captured in the recording can be copied to
another BDC Script template or can be merged into another BDC Script
template.

**NOTE**: To merge or copy a BDC screen to another BDC Script template,
the destination template must be inactive.

The merge process copies all BDC screens captured in the recording to
another BDC Script template. The destination template can be associated
with any category. When merging, the priority assigned to the original
BDC screens is copied over to the new template.  For example, the
original template has three screens with a priority of 10, 20, and 30.
When merged with the destination template, the original screens retain
the priority of 10, 20, and 30. The destination template’s first screen
continues with an updated priority of 40, the second is 50, and so on.

The copy process copies a selected screen to another BDC Script
template. The destination template can be associated with any category.

**NOTE**: When copying or merging BDC Screens, Integrate does not
overwrite duplicate screens. If a copy or merge has already been
performed from the original template to the destination template,
another copy or merge will create duplicate screens in the destination
template.

To merge all BDC screens with another BDC Script template:

1.  Select **Categories** on *Navigation pane*.

2.  Click the **Templates** icon for a category.

3.  Click **Vertical View** for the BDC Script template that should be
    merged.

4.  Click **Copy** tab.

5.  Click **Merge BDC Screens**.
    
    **NOTE**: The Copy Type displays **Merge**.

6.  Click **Edit**.
    
    *[View the field descriptions for the Copy
    page.](../Page_Desc/Copy)*

7.  Select a category name in the **Copy to Category** list box.
    
    **NOTE**: All categories added to Integrate display.

8.  Select a template in the **Copy to Existing Template** list box.
    
    **NOTE**: This must be a template based on a BDC Script.

9.  Click **Save**.

10. Click **Execute**; a confirmation message displays.

11. Click **Ok**.

The BDC screens from the original template are merged with the screens
in the destination template.

To copy a BDC screen to another BDC Script template:

1.  Click the **Templates** icon for a category.

2.  Click **Vertical View** for the BDC Script template that should be
    copied.

3.  Click **Configuration** tab.

4.  Click **BDC Screen**.

5.  Click **Vertical View** for the screen to be copied.

6.  Click **Copy** tab.

7.  Click **Copy BDC Screen**.
    
    **NOTE**: The Copy Type displays **BDCScreen**.

8.  Click **Edit**.
    
    *[View the field descriptions for the Copy
    page.](../Page_Desc/Copy)*

9.  Select a category name in the **Copy to Category** list box.
    
    **NOTE**: All categories added to Integrate display.
    
    <span style="font-weight: bold;">NOTE</span>: This field is required
    to perform the copy.

10. Select a template in the **Copy to Existing Template** list box.
    
    **NOTE**: This must be a template based on a BDC script.
    
    <span style="font-weight: bold;">NOTE</span>: This field is required
    to perform the copy.

11. Click **Save**.

12. Click **Execute**; a confirmation message displays
    
    <span style="font-weight: bold;">NOTE</span>: This button is
    disabled until required fields are completed.

13. Click **Ok**.

The BDC screen from the original template is copied to the destination
template.
