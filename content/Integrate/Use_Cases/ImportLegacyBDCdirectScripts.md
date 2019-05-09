+++
title = 'Import Legacy BDCdirect<span>®</span> Scripts into Integrate'
solution = 'Platform'
+++

# Import Legacy BDCdirect<span>®</span> Scripts into Integrate

Importing a BDCdirect® script creates a template in Integrate based on
the script in BDCdirect®.

To import legacy BDCdirect® scripts into Integrate:

1.  Populate the stUSYS\* tables in the Integrate SQL Database with
    BDCdirect® data.
    
    **NOTE:** Populating this table is a manual process.

2.  Select **Integrate \> Advanced \> BDCdirect** from *Navigation
    pane*; all BDCdirect® scripts display.

3.  Click **Edit** for a script.
    
    [View the field descriptions for the BDCdirect: Script
    page](../Page_Desc/BDCDirect_Script)

4.  Update the **CATEGORY** field to change the default name of the
    Integrate category if needed.
    
    **NOTE**: If the category name does not exist in Integrate, a new
    category is automatically created. If the field is blank, the
    category is named “BDCdirect Import.” If the category already
    exists, the template is added to that category.

5.  Click **Save**.

6.  Click the **IMPORT** check box to enable it, marking the BDCdirect®
    script for import.

7.  Click **Import to Integrate** on thePage toolbar to create Integrate
    templates from the scripts where the IMPORT check box is enabled.

8.  Click **Ok**.
