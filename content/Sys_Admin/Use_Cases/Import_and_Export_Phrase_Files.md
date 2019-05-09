+++
title = 'Import and Export Phrase Files'
solution = 'Platform'
+++

# Import and Export Phrase Files

Phrase files can be imported or exported at the WebApp catalog level.
Use this feature to:

  - Make multiple phrase changes
  - Add phrase translations
  - Generate a report of all phrases to analyze or view

**NOTE:** If a catalog is read-only, a phrase file cannot be imported or
exported. Most delivered catalogs are read only. To make a custom
catalog read only, check the **Read Only** check box on the
*[Catalogs](../Page_Desc/Catalogs_H.htm#Catalogs_V)* page's *Vertical*
View.

**NOTE:** Importing a phrase file replaces all phrases, translations and
dynamic help for the catalog with the contents of the XML file.

A user can also [Add Phrases to Catalogs](Add_Phrases_to_Catalogs.htm)
manually.

To export a phrase file:

1.  Select **Admin \> Translations \> Catalogs** in the *Navigation*
    pane.
2.  Click **Vertical View** for a catalog.
3.  Click **Export**.
4.  Click **Download a file** to download the phrase file.

**NOTE:** The file downloads in xml format, and can be edited with any
program as long as the schema of the document remains the same. On
import, the DSP expects the schema that was exported.

To import phrases:

1.  Select **Admin \> Translations \> Catalogs** in the *Navigation*
    pane.
2.  Click **Vertical View** for a Catalog.
3.  Click the **Upload a File** icon next to **File Location** and
    select the XML file.
4.  Click **Import**.
5.  A confirmation message displays to replace ALL phrases, translations
    and dynamic help with the contents of the XML file.
6.  Click **Ok**.

To clear all phrases, translations and dynamic help from a catalog:

1.  Select **Admin \> Translations \> Catalogs** in the *Navigation*
    pane.
2.  Click **Vertical View** for a Catalog.
3.  Click **Clear**.
4.  A confirmation message displays to clear ALL phrases, translations
    and help from the Catalog.
5.  Click **Ok**.
