# Configure Excel Integration Overview

Excel Integration allows users to import records from a worksheet in an
Excel Workbook file by one of the following methods:

  - **Page-level Import** — A user can manually import the Excel file
    via the Page Gear menu \> Excel Integration (if the feature is
    enabled on the page).
  - **Public WebApp Event** — The Public WebApp event, added to the page
    as a business rule, can import the Excel file without user
    involvement. This is useful if an Excel file should be imported
    every day at a certain time from a service page.

**NOTE:** Refer to the Knowledge Base article on the BackOffice
Associates Support site [DSP® Microsoft® Excel® Integration Developer
Guide](https://support.boaweb.com/hc/en-us/articles/115013359708-DSP-Microsoft-Excel-Integration-Developer-Guide)
for information about running Excel Integration via a Public WebApp
event.

To perform Excel Integration on a Construct page or a page for a custom
WebApp, the Page Designer must enable the feature on the page. Refer to
[Enable Excel Integration](Enable_Excel_Integration.htm) for more
information.

Refer to [DSP Pages Delivered with Excel Integration
Enabled](DSP_Pages_Delivered_with_Excel_Integration_Enabled.htm) for
information about pages in delivered WebApps that allow the use of Excel
Integration.

The Excel template uses the current user’s language, set on the *[My
Profile](../../../My%20Profile.htm)* page, to translate the translated
column name and the help text in the template. Translated phrases must
exist for the column headers and help text for them to display in the
spreadsheet. Refer to [Set the Language for the Translated Column Name
Header in the Excel
Template](Set_the_Language%20in%20the%20Translated_Column_Header.htm)
for more information.

Excel Integration cannot be performed on a page if it is read only.

**NOTE:** The security definitions associated with a user’s role may
prevent that user from viewing records added via Excel Integration. If a
user’s role prevents that user from viewing records on a page through a
security definition, and the UPDATE USER DEFINITION ON SAVE check box on
the *[Security Definitions
Pages](../Page_Desc/Security_Definition_Pages.htm)* page is unchecked,
the user can add records to the page using Excel Integration. However,
the user cannot view these records.

Refer to [Use Excel
Integration](../../Excel_Int/Use_Excel_Integration.htm), the Knowledge
Base article [Use Excel Integration to Create or Update Multiple User
Accounts](https://support.boaweb.com/hc/en-us/articles/115015883247--DSP-Administration-Use-Excel-Integration-to-Create-or-Update-Multiple-User-Accounts)
and the Data Insiders article [Excel
Integration](https://support.boaweb.com/hc/en-us/community/posts/115008946068-Excel-Integration)
for more information.

Configure Excel Integration includes the following topics:

  - [DSP® Pages Delivered with Excel Integration
    Enabled](DSP_Pages_Delivered_with_Excel_Integration_Enabled.htm)
  - [Enable Excel Integration](Enable_Excel_Integration.htm)
  - [Add Reserved Columns to Tables to Track Excel
    Integration](Add%20Reserved%20Columns%20to%20Tables%20to%20track.htm)
  - [Include Data Type and Help Text in the Excel
    Template](Include%20Data%20Type%20and%20Help%20Text.htm)
  - [Configure Column Header and Text Color in the Excel
    Template](Configure_Column_Header_Color_in_the_Excel_Template.htm)
  - [Exclude Columns from Excel
    Integration](Exclude%20Columns%20Excel%20Integration.htm)
  - [Set the Language for the Translated Column Header in the Excel
    Template](Set_the_Language%20in%20the%20Translated_Column_Header.htm)
  - [Enable/Disable Sheet with
    Instructions](Enable_Disable_Sheet_with_Instructions_for_a_Page.htm)
