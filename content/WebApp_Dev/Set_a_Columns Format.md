+++
title = "Set a Column's Format"
solution = 'Platform'
+++

# Set a Column's Format

Some control types allow a user to set the column’s format.

<table>
<tbody>
<tr class="odd">
<td><p>Control</p></td>
<td><p>Formats</p></td>
</tr>
<tr class="even">
<td><p>Text Box</p></td>
<td><ul>
<li>Email</li>
<li>Password</li>
<li>Text</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Text Area</p></td>
<td><p>SQL</p></td>
</tr>
<tr class="even">
<td><p>Numeric</p></td>
<td><ul>
<li>Currency</li>
<li>Numeric</li>
<li>Numeric Positive</li>
<li>Percent</li>
<li>Zero Padded Integer</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>DateTime</p></td>
<td><ul>
<li>Date</li>
<li>Date and Time</li>
<li>Formatted Date</li>
<li>Formatted Time</li>
<li>Time</li>
<li>Time (24 hour)</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Check Box</p></td>
<td><ul>
<li>SAP BDC</li>
<li>SAP Checkbox - Deprecated</li>
<li>Y or N</li>
</ul></td>
</tr>
</tbody>
</table>

To apply formatting to a column, select an option from the Format list
box on the *Page Columns* page's *Vertical* View. For a check box,
select an option from the Checkbox Format ID list box. Numeric fields
allow for additional formatting options.

To apply additional formats to a numeric column:

1.  <span id="Column Properties Navigation" class="popUpLink">Access the
    *Page Columns*</span> *Vertical* View for a Numeric column.

2.  Click **Edit**.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H)*

3.  Select an option from the**Format** list box.
    
    **NOTE:** Depending on the Format selected and the purpose of the
    field, set these additional options.

4.  Enter a value in the **Numeric Scale** text box.
    
    **NOTE:** The Numeric Scale field determines the number of decimal
    places to display after the decimal separator.

5.  Click **Display Thousands Separator** check box.
    
    **NOTE:** The Display Thousands Separator will force a number to use
    the current user’s locale to display a number such as 4213.22 as
    4,213.22 given that English – United States is selected in the
    Currency Locale ID list box.

6.  Click **Total** check box.
    
    **NOTE:** A totals column recalculates when records are added,
    deleted, or modified.

7.  Click **Save**.
