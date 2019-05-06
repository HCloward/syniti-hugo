# Include Data Type and Help Text in the Excel Template

The Excel template that is downloaded from a page for use with Excel
Integration can have up to four column header rows. All templates have
the column’s technical name in the first row, and the translated name in
the second row. A Page Designer can include the data type and length
details for each column in a row, and the help text for a column in a
row. These columns are not included by default.

When downloading an Excel template through Excel Integration on a page
it is possible to include the Data Type in the header.

  - varchar, nvarchar, char, nchar will show the data type and length;
    for example, nvarchar (50), when the field has maximum length, it
    will show (-1) as the length; for example, nvarchar (-1), ntext will
    show always (-1)
  - decimal, numeric, money and smallmoney will show the data type and
    the number of whole digits and decimals; for example, decimal (10,4)
  - bit, int, smallint, bigint, double, float, real, datetime,
    datetime2, time and uniqueidentifier will show only the data type

**NOTE:** Help text must exist for the column. Refer to [Add Column Help
Text](../../WebApp_Dev/Add_Column_Help_Text.htm) for more information.
The help text displays as text only, without HTML markup.

**NOTE:** Before header rows can be configured for the template for a
page, Excel Integration must be enabled for that page. Refer to [Enable
Excel Integration](Enable_Excel_Integration.htm) for more information.

The Excel template uses the current user’s language, set on the [My
Profile](../../../My%20Profile.htm) page, to translate the translated
column name and the help text in the template. Translated phrases must
exist for the column headers and help text for them to display in the
spreadsheet.

To include the data type or help header rows:

1.  Navigate to the page where the Excel template columns should be
    configured.

2.  Click the **Change Settings** icon in the Site toolbar.

3.  Select **Design**.
    
    **NOTE:** A new tab opens in the browser. The original page remains
    open in a tab as well.

4.  Click **Vertical View**.

5.  Click the **Excel** tab.

6.  Click **Edit**.
    
    [View the field descriptions for the Pages
    page](../Page_Desc/Pages_H.htm#DynamicExceltab)

7.  Check the **Excel Data Type Header** check box.
    
    **NOTE:** The data type and length details for each column displays
    in the third row of the downloaded file.

8.  Check the **Excel Help Text Header** check box.
    
    **NOTE:** The text-only representation of the column's help text
    (without HTML markup) displays in the fourth row of the downloaded
    file.

9.  Click **Save**.
