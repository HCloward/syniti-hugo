+++
title = 'Configure a Conditional for a BDC Screen'
solution = 'Platform'
+++

# Configure a Conditional for a BDC Screen

<span id="Post Data using a BDC Script Steps" class="popUpLink">\>Review
the steps in the process. </span>

This optional step allows a user to add conditionals at the BDC screen
level. A conditional is a data condition that, if true, will result in
the inclusion of the data from the process template field mappings
associated with the screen in the resulting posting script.  If the data
condition is false, the screen will be left out of the posting script. 

Each conditional is data record specific.  For example, if 10 records
are posted, Integrate evaluates the conditional for each data record and
applies it to the data in that record only. 

If there is no conditional applied to a screen, then the screen will be
included in the posting script.

Only one conditional can be configured per BDC screen.

**NOTE**: Conditionals cannot be modified if the template is active.

**NOTE**<span>:</span> Conditionals can be applied to custom fields.
Refer to [Add Custom Fields to a BDC Script
Template](Add_Custom_Fields_to_a_BDC_Script_Template) for more
information.

To configure a conditional for a BDC screen on the *BDC Screen* page:

1.  Select **Categories** from *Navigation pane*.

2.  Click **Template**.

3.  Locate the Template with a Type of BDC Script.

4.  Click **Vertical View**.

5.  Click **Configuration** tab.

6.  Click **BDC Screen** button.

7.  Click **Vertical View** for a screen.

8.  Click **Conditionals** button.
    
    *[View the field descriptions for the BDC Screen Conditionals
    page](../Page_Desc/BDC_Screen_Conditionals)*

9.  Select a field from **CONDITIONAL FIELD NAME** list box.

10. Select a conditional from **CONDITIONAL TYPE** list box.

11. Enter a value in **CONDITIONAL VALUE**.

12. Click **Save**.

After this template is added to a process, the data set that will be
posted will meet the conditions configured.
