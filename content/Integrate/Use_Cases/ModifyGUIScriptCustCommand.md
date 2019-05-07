+++
title = 'Modify a GUI Script with a Custom Command'
solution = 'Platform'
+++

# Modify a GUI Script with a Custom Command

<span id="Post Data using a GUI Script Steps" class="popUpLink">\>Review
the steps in the process. </span>

Integrate allows a user to manually overwrite the GUI script using a
custom command that performs advanced checks and functionality during
posting.

To view the current command and create a custom command for a field
captured in the GUI recording:  

1.  Select **Categories** from *Navigation pane*.

2.  Click the **Templates** icon for a category.

3.  Locate the Template with a Type of **GUI Script**.

4.  Click **Vertical View**.

5.  Click **Configuration** tab.

6.  Click **GUI Script Data** button.

7.  Click **Vertical View** for a field.
    
    *[View the field descriptions for the GUI Script Data page’s
    Vertical
    View.](../Page_Desc/GUI_Script_Data_H.htm#GUI_Script_Data_V_All)*
    
    **NOTE**: The script line related to this field displays in **VB
    Script Line**.

8.  Click **Recording** tab.

9.  Click **Commands** to view the commands and actions captured for
    this field during the GUI script recording.

10. Navigate back to the *GUI Script Data* page’s *Vertical* View.

11. Click **General** tab.

12. Click **Edit**.

13. Click **Custom Command** check box to enable it.

14. Modify the text in **VB Script Line** field to include the custom
    command.
    
    **NOTE**: The **VB Script Line** must contain valid VBScript syntax
    for the custom command to run.

Integrate will run the custom command when posting data.
