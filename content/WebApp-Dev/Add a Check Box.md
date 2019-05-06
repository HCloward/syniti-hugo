# Add a Check Box

A check box allows a user to enable or disable a setting. Refer to [Add
a Control Type to a
Column](Add%20a%20Control%20Type%20to%20a%20Column.htm) for general
information about adding a check box.

By default, a check box data type is bit in the underlying table using 1
for enabled and 0 for disabled. Additionally, if the data type of the
table column in SQL is set to bit, the DSP® assumes the field is a check
box and appropriately populate the data with a 1 or 0.

A check box can use other formats.

**NOTE**: If a format other than the default is set for the check box,
the data type of the table column in SQL must be set to a character of
length 1. If a check box format listed below is used on a page and the
data type of the check box is bit or another non-character format, an
error displays when the user attempts to add data to the page.

Check box formats are:

  - SAP BDC

**NOTE**: A check box using this format uses the values ‘X’ for checked
and ‘\!’ for unchecked in the table column. The ‘\!’ is a special
character used in an SAP BDC that tells the program there is no data in
the field (i.e., the field should be ignored.) This is useful when doing
an update to existing data in SAP and you do not want to inadvertently
overwrite existing field values. For example, a material exists in SAP
and the user wants to update 2 fields with a BDC. The BDC the user
chooses has 10 fields available for input, but only 2 fields need to be
updated. It the 2 fields are populated in the DSP® and the remaining 8
fields are left blank, the BDC produces a load file to update the 2
fields properly, but also sets the remaining 8 fields that exist in the
BDC to blank. When the data is posted in this case, the remaining 8
fields are set to blank in SAP. To prevent this, pass ‘\!’ in the
remaining fields, rather than leaving them blank. When posting data, SAP
does not update the data for fields with ‘\!’.

  - SAP Checkbox

**NOTE**: A check box using this format uses the values ‘X’ for checked
and ‘ ‘ for unchecked in the table column.

  - Y or N

**NOTE**: A check box using this format uses the values ‘Y’ for checked
and ‘N’ for unchecked in the table column.

To set a check box format:

1.  Navigate to the *[Page
    Columns](../Sys_Admin/Page_Desc/Page_Columns_H.htm)* page’s
    *Vertical* View for the column with the check box control and click
    **Edit**.
2.  Select an option in the **Checkbox Format ID** list box.
3.  Click **Save**.
