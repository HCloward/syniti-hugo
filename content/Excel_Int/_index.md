+++
title = "Excel Integration Overview"
weight = 3
layout = "single"
tips = "Excel"
+++

# Use Excel Integration Overview

Page Designers create pages for use by business users, SMEs, and other
data contributors. Often, data contributors enter data in Excel and want
to upload that data into the DSP. Designed for users without technical
knowledge, Excel Integration facilitates this workflow in a user
friendly way that guides the user through the process of importing from
Excel. It allows users to download a formatted template, enter data, and
then import that data from the template into DSP® pages.

The Page Designer can enable this feature on Construct pages and pages
in custom WebApps. The feature is [enabled on some pages delivered with
the
DSP](../Sys_Admin/Use_Cases/DSP_Pages_Delivered_with_Excel_Integration_Enabled).

Excel Integration honors the binding and drill criteria on a page. When
Excel Integration is used on a child page, the columns coming from the
parent page are automatically set when the data is imported from Excel
to the child page.

For example, a user accesses a parent page called Categories and selects
a Category ID of Entertainment. The child page, Products, displays a
list of products included in the Entertainment category.

The user downloads an Excel template from the Products page. The
template includes the Category ID column.

When the user imports the Excel spreadsheet into the Products page, a
warning displays stating that any values entered in the spreadsheet for
the Category ID field will be replaced with the value Entertainment,
(the binding criteria passed from the parent page, Categories).

To use Excel Integration:

  - [Download an Excel Template](Download_an_Excel_Spreadsheet)
  - [Import Data](Import_Data)
  - [Lock Records](Lock_Records)
  - [Unlock Records](Unlock_Records)
