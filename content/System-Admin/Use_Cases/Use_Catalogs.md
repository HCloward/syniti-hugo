# Use Catalogs During Application Development

DSP® catalogs provide a means to populate and administer translations,
help text and alias values at the WebApp and page levels.

Catalogs exist in the system at these levels:

  - **Page-specific Catalogs** – Catalogs that exist for a given page.
    Translations, help text and alias values in these types of catalog
    are only applicable for the one page to which the catalog is linked.
  - **WebApp Catalogs** – Catalogs that are created generally in System
    Administration and are applied to one or many WebApps. Translations,
    help text and alias values found in these catalogs apply to all
    pages in a WebApp to which it is assigned.

When phrases on a page are translated, DSP® searches through all
catalogs assigned to the page. A translation is attempted to be made at
the highest level catalog. If a match is not found, the next level
catalog is searched until a phrase translation match is found.

It is recommended to translate phrases at the most generic level
appropriate. The higher the level the phrase is translated, the more
useful the translation will be. A phrase translated at the Catalog
(WebApp) level can be reused by many applications and many pages. A
phrase translated at the page level is only good for that single page.

There are cases where a Phrase has a unique meaning on a page, different
from its *usual* meaning, and should be translated at the page level.
However, page level translation should be the exception to the rule.

Refer to [Manage Catalogs](Manage_Catalogs.htm) for more information.

This section contains these topics:

  - [Add Phrase Out Values to Alias a Column on a
    Page](Add_Phrase_Out_Values_to_Alias_a_Column_on_a_Page.htm)
  - [Add Column Help Text](../../WebApp_Dev/Add_Column_Help_Text.htm)
