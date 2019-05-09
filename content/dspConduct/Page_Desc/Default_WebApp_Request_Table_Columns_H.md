+++
title = 'Default WebApp Request Table Columns H'
solution = 'Master Data Management'
+++

# Default WebApp Request Table Columns H

[Default WebApp Request Table Columns V](#Default)

<div class="use">

Use this page to [Auto-generate Request-related
Objects](../Use_Cases/Auto_Generate_Request_related_Objects).

</div>

To access this page:

1.  Click **dspConduct \> Design** in the *Navigation* pane.

2.  Click **Vertical View** for a category.

3.  Click the **Create Default Web App Request Table and Views** icon.
    
    **NOTE**: This page allows the user to create the request-related
    objects in the WebApp and the database, and this icon is active if
    those objects have not been built. After the objects have been built
    successfully, the Create Default Web App Request Table and Views
    icon is disabled. In other words, this page is not accessible once
    the request-related objects have been built.

4.  Click **Table Columns**.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>COLUMN NAME</p></td>
<td><p>Displays the name of the table column or page column.</p></td>
</tr>
<tr class="odd">
<td><p>COLUMN ORDER</p></td>
<td><p>Displays the order the column name appears in the table definition. If the value is 0, the column is a page column only and is not included in the ttRequest table when it is auto-generated.</p></td>
</tr>
<tr class="even">
<td><p>DATA TYPE</p></td>
<td><p>Displays the data type of the column name in the table definition.</p>
<p>If a column is a page column only, this field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>VIEW TYPE</p></td>
<td><p>Displays whether the column will appear on the <em>Horizontal</em>, <em>Vertical</em> or All views.</p></td>
</tr>
<tr class="even">
<td><p>HOR VIEW ORDER</p></td>
<td><p>Displays the order the column name will appear in the <em>Horizontal</em> View when the table is auto-generated. If the value is 0, the column does not display in the <em>Horizontal</em> View.</p></td>
</tr>
<tr class="odd">
<td><p>VER VIEW ORDER</p></td>
<td><p>Displays the order the column name will appear in the <em>Vertical</em> View when the table is auto-generated. If the value is 0, the column does not display in the <em>Vertical</em> View.</p></td>
</tr>
<tr class="even">
<td><p>TABLE KEY</p></td>
<td><p>If enabled, the column name will be included in the Primary Key for the table definition.</p></td>
</tr>
<tr class="odd">
<td><p>PAGE KEY</p></td>
<td><p>If enabled, the column name will be included in the Primary Key for the page column definition.</p></td>
</tr>
<tr class="even">
<td><p>CONTROL</p></td>
<td><p>Displays the control type used by the column, such as button, text box or list box.</p></td>
</tr>
<tr class="odd">
<td><p>CONTROL STATUS</p></td>
<td><p>Displays whether the column should be enabled (displayed), disabled (display only), or hidden in the associated View Type.</p></td>
</tr>
</tbody>
</table>

 

## <span id="Default"></span>Default WebApp Request Table Columns V

[Default WebApp Request Table Columns H](#top)

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Column Name</p></td>
<td><p>Displays the name of the table or page column.</p></td>
</tr>
<tr class="odd">
<td><p>Column Order</p></td>
<td><p>Displays the order the column name appears in the table definition. If the value is 0, the column is a page column only and is not included in the ttRequest table when it is auto-generated.</p></td>
</tr>
<tr class="even">
<td><p>Data Type</p></td>
<td><p>Displays the data type of the column name in the table definition.</p>
<p>If a column is a page column only, this field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>Length</p></td>
<td><p>Displays the maximum character length allowed in the column.</p></td>
</tr>
<tr class="even">
<td><p>Decimal places</p></td>
<td><p>Displays the number of decimal places allowed in the column. This value is only valid for columns with a control of Numeric.</p></td>
</tr>
<tr class="odd">
<td><p>Table Key</p></td>
<td><p>If enabled, the column name will be included in the Primary Key for the table definition.</p></td>
</tr>
<tr class="even">
<td><p>Page Key</p></td>
<td><p>If enabled, the column name will be included in the Primary Key for the page column definition.</p></td>
</tr>
<tr class="odd">
<td><p>Table Default </p></td>
<td><p>Displays the value that is used to create the column's default value in SQL.</p></td>
</tr>
<tr class="even">
<td><p>Page Default</p></td>
<td><p>Displays the value that will be added as the default value in the column. For example, a COUNTRY list box can have the default value US.</p></td>
</tr>
<tr class="odd">
<td><p>Control</p></td>
<td><p>Displays the control type used by the column, such as button, text box or list box.</p></td>
</tr>
<tr class="even">
<td><p>Control Status</p></td>
<td><p>Displays whether the column should be enabled (displayed), disabled (display only), or hidden in the associated View Type.</p></td>
</tr>
<tr class="odd">
<td><p>Consider Valid</p></td>
<td><p>If enabled, the boaStatus column is used to determine whether the control is enabled or disabled.</p></td>
</tr>
<tr class="even">
<td><p>List Source</p></td>
<td><p>Displays the source of the data for the column when the control is Combo Box or List Box. The value can either be a SQL object (Table or View) or a List Data Provider plugin.</p></td>
</tr>
<tr class="odd">
<td><p>List Display Field</p></td>
<td><p>Displays the option visible in the List Box or Combo Box.</p></td>
</tr>
<tr class="even">
<td><p>List Value Field</p></td>
<td><p>Displays the name of the field that stores the value.</p>
<p>In most cases, List Value Field is the primary key stored in the table</p></td>
</tr>
<tr class="odd">
<td><p>List Where Clause</p></td>
<td><p>Displays the Where Clause used to restrict the values that display in a List Box or Combo Box.</p></td>
</tr>
<tr class="even">
<td><p>Hor. View Order</p></td>
<td><p>Displays the order the column name will appear in the <em>Horizontal</em> View when the table is auto-generated. If the value is 0, the column does not display in the <em>Horizontal</em> View.</p></td>
</tr>
<tr class="odd">
<td><p>Ver. View Order</p></td>
<td><p>Displays the order the column name will appear in the <em>Vertical</em> View when the table is auto-generated. If the value is 0, the column does not display in the <em>Vertical</em> View.</p></td>
</tr>
<tr class="even">
<td><p>Required</p></td>
<td><p>Displays the requirement level on a column by adding a page validation view. The requirement levels are:</p>
<ul>
<li><strong>Required (Hard)</strong> - This setting specifies this field must contain valid data before a save can be completed.</li>
<li><strong>Required (Soft)</strong> - This setting generates an error but allows records to be saved.</li>
<li><strong>No</strong> - The field is not required.</li>
</ul>
<p>If the field value contains NOT NULL in the table (such as a key), the column automatically defaults to Required (Hard).</p></td>
</tr>
</tbody>
</table>
