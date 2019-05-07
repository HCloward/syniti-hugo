+++
title = 'Copy a Template'
solution = 'Platform'
+++

# Copy a Template

Integrate allows a user to copy an existing template to create a new
template in any category. A copy of a template includes all settings in
the original template, including:

  - Screens, fields, loops and conditionals in the case of BDC Scripts
    and GUI Scripts

  - Custom commands in the case of GUI Scripts

  - Structures and fields in the case of User Defined templates

  - Global Variables in BODS Execution templates

**NOTE**: Copy template functionality is not available for BAPI/RFC
template types.

A copy of a template does not copy the processes associated with the
original template.

**NOTE**: A template can be copied whether the template is active or
not.

To copy a template:

1.  Select **Categories** on *Navigation pane*.

2.  Click **Templates** for a category.

3.  Click **Vertical View** for the template that should be copied.

4.  Click **Copy** tab.

5.  Click <span style="font-weight: bold;">Copy Template</span>.
    
    **NOTE**: The **Copy Type** displays **Template**.

6.  Click **Edit**.
    
    [View the field descriptions for the Copy
    page.](../Page_Desc/Copy.htm)

7.  Select a category name in the **Copy to Category** list box.
    
    **NOTE**: All categories added to Integrate display.

8.  Enter a name in <span style="font-weight: bold;">Copy To Template
    Name</span>.
    
    **NOTE**: This name must be unique. The name can contain all letters
    (A-Z), all numbers (0-9), and underscores. It cannot contain special
    characters. Integrate will replace special characters with
    underscores when the template is saved.
    
    <span style="font-weight: bold;">NOTE</span>: This field is required
    to perform the copy.

9.  Enter a description in <span style="font-weight: bold;">Copy To
    Template Description</span>.

10. Click **Save**.

11. Click **Execute**; a confirmation message displays.
    
    <span style="font-weight: bold;">NOTE</span>: This button is
    disabled until required fields are completed.

12. Click **Ok**.

The template is added to the category. It must be activated, and then
can be assigned to a process.
