+++
title = 'Create a Delimited or Fixed Width User Defined Template'
solution = 'Platform'
+++

# Create a Delimited or Fixed Width User Defined Template

<span id="Post Data Using UDF or Fixed Width Steps" class="popUpLink">Review
the steps in the process. </span>

Delimited files contain data elements, each separated by a
character.  The delimiter can be any character, and is defined on the
**Configuration** tab of the *Vertical* View of the *Template* page.

Each data element in a Fixed Width file has a defined length.  On the
**Configuration** tab, define the pad location to pad the values to its
full length.

**NOTE**: Begin template creation on the *Template* page in *Horizontal*
View. Refer to [Create a Basic Template](Create_a_Basic_Template.htm)
for more information.

To create a Delimited or Fixed Width template on the *Vertical* View of
the *Template* page:

1.  Select <span style="font-weight: bold;">Delimited</span> or
    <span style="font-weight: bold;">FixedWidth</span> in the
    <span style="font-weight: bold;">User</span><span style="font-weight: bold;">Defined</span><span style="font-weight: bold;">Template</span><span style="font-weight: bold;">Type</span>
    list box.

2.  Click **Save**.

3.  Click **Edit**.
    
    *[View the field descriptions for the Template page’s Vertical
    View.](../Page_Desc/Template_H.htm#Template_V_All_Tabs)*

4.  Click <span style="font-weight: bold;">Configuration</span> tab.

5.  Select an option in the **Fixed Width Pad Location** list box for
    Fixed Width files.
    
    **NOTE**: For Fixed Width files, the selection sets whether
    Integrate will pad the value to its full length before or after the
    value.  A Pad Location of **After** will write the value to the file
    and then fill the remaining length with spaces.  A Pad Location of
    **Before** will write spaces before the value so that the length is
    filled by the combination of spaces and values.
    
    **NOTE**: Select **None** in the **Fixed Width Pad Location** list
    box if the template is Delimited.

6.  Enter the character to use when separating the values for Delimited
    files in **Delimiter**. 
    
    **NOTE**: This field does not display for Fixed Width templates.

7.  Click **Save**.
