+++
title = 'Import Legacy BDCPlus Templates into Integrate'
solution = 'Platform'
+++

# Import Legacy BDCPlus Templates into Integrate

Importing a BDCPlus template creates a template in Integrate based on
the template in BDCPlus.  

To import legacy BDCPlus templates into Integrate:

1.  Populate the stBDCPlus\* table in the Integrate SQL database for
    BDCPlus data.
    
    **NOTE:** If the BDCPlus database has been backed up, the
    stBDCPlus\* table can be populated from the backup using the Extract
    process. Place a copy of the BDCPlus database on the same server as
    the Integrate database. The stBDCPlus\* tables will be populated
    during the Extract process in Integrate. If the BDCPlus database has
    not been backed up, manually populate the stBDCPlus\* tables.

2.  Select **Integrate \> Advanced \> BDCPlus** from *Navigation pane*.
    
    **NOTE:** If the stBDCPlus\* tables were populated manually, all
    BDCPlus templates display on the *[BDCPlus:
    Templates](../Page_Desc/BDCPlus_Templates.htm)* page. Otherwise, the
    page displays no records.

3.  If using a BDCPlus backup database, click **BDC Plus Extract** on
    the Page toolbar to populate the stBDCPlus\* tables. All BDCPlus
    Templates display on the *BDCPlus: Templates* page.
    
    **NOTE:** If there is no BDCPlus backup database, the stBDCPlus\*
    tables are manually and the records display on the page; the BDC
    Plus Extract icon is not visible. Continue with the following steps.

4.  Click **Edit** for a template.
    
    [View the field descriptions for the BDCPlus: Templates
    page](../Page_Desc/BDCPlus_Templates.htm)

5.  Update the CATEGORY field to change the default name of the
    Integrate category, if needed.
    
    **NOTE**:If the category name does not exist in Integrate, a new
    category is automatically created. If the field is blank, the
    category is named “BDCPlus Import.” If the category already exists,
    the template is added to that category.

6.  Click **Save**.

7.  Click the **IMPORT** check box to enable it, marking the BDCPlus
    templates for import.

8.  Click **Import to Integrate** on the Page toolbar to create
    Integrate templates from the templates where the IMPORT check box is
    enabled.

9.  Click **Ok**.
