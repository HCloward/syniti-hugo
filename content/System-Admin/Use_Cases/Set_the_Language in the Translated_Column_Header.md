+++
title = 'Set the Language for the Translated Column Name Header in the Excel Template'
solution = 'Platform'
+++

# Set the Language for the Translated Column Name Header in the Excel Template

The translated column name heading row and the help text row in the
Excel template are translated to the user’s language. A user’s language
is set on the *[My Profile](../../../My%20Profile.htm)* page in the
Language field.

Translations must exist for the language in the DSP, and the the
language must be active. Refer to [Set a Language as
Active](Set_a_Language_as_Active.htm) for more information.

If the translated column name heading row or the help text heading row
contain a phrase that has a translation, then the translation displays
in the header row of the Excel template.

These translations can exist at three levels:

1.  The system level which is the highest level
2.  The WebApp catalog level
3.  The page level which only exists for that page

The search begins at the page level, then the catalog level and finally
the system level until a translation is found. If no translation exists,
the translated column name heading row displays the technical column
name If a translation does not exist for the help text, the untranslated
help text displays.

To set the language to translate column headers in the Excel template
for a page for the current user:

1.  Navigate to the page where the Excel template columns should be
    configured.
2.  Click the gear.
3.  Select **Settings**.
4.  Select the desired language from the **Language** list box.
5.  Click **Save**.
6.  Refresh the browser. The column names on the page are translated to
    phrases containing the name of the chosen language.

**NOTE:** To see the translated column headers, download the template.
Refer to [Download an Excel
Template](../../Excel_Int/Download_an_Excel_Spreadsheet.htm) for more
information.
