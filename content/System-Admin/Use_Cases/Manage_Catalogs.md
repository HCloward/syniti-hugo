# Manage WebApp Catalogs

Catalogs provide a means to:

  - Populate and administer translations or alias values
  - Create dynamic help text that displays in the Information pane

Refer to [Add Dynamic Help to a
Page](../../WebApp_Dev/addDynamicHelpToAPage.htm) and [Add Column Help
Text](../../WebApp_Dev/Add_Column_Help_Text.htm) for more information.

Catalogs contain groups of WebApp phrases and WebApp phrase
translations. They can be tailored to contain a complete WebApp phrase
set, a subset of phrases, such as SAP field names, or a larger set of
phrases that can be applied to several WebApps. For each phrase it
encounters, the DSP searches for a translation in all catalogs assigned
to a WebApp in a prioritized order.

The DSP searches for translations starting with the highest level
catalog (the one assigned at the WebApp level with the lowest priority).
If a match is not found, the next level catalog is searched (either the
catalog at the WebApp level with the next lowest priority, or the
catalog at the page level). If no translations are found, the DSP
displays the original phrase.

It is recommended to translate phrases at the highest level appropriate.
The higher the level the phrase is translated, the more useful the
translation will be. A phrase translated at the WebApp level can be
reused by many applications and many pages. A phrase translated at the
page level is used only for that page.

There are cases where a phrase has a unique meaning on a page, different
from its usual meaning, and should be translated at the page level.
However, page-level translation should be the exception to the rule.

Catalogs are included for delivered WebApps and, in most cases, cannot
be edited. Custom catalogs can be added, and assigned to both delivered
and custom WebApps.

Managing catalogs includes the following topics:

  - [Create WebApp Catalogs](Create_WebApp_Catalogs.htm)
  - [Add Phrases to Catalogs](Add_Phrases_to_Catalogs.htm)
  - [Assign a Catalog to a Custom
    WebApp](Assign%20a%20Catalog%20to%20a%20Custom%20Webapp.htm)
  - [Add a Catalog to a Delivered
    WebApp](Add%20a%20Catalog%20to%20a%20Delivered%20WebApp.htm)
  - [Import and Export Phrase Files](Import_and_Export_Phrase_Files.htm)
  - [Display Translations for Column
    Data](Display_Translations_for_Column_Data.htm)
  - [Troubleshoot Translations](Troubleshoot%20Translations.htm)
