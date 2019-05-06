# Filter Controls

The controls on the Filter View allow the user to define filter
criteria. Filter criteria operates on individual columns. Only one set
of criteria can be applied to a column at a time. However, different
filter criteria can be specified for each column.

An Administrator can set the control type for the filter. The controls
used are a variation of the standard controls. The relationship between
controls defined at the column property level and those used on the
Filter View are outlined in the following table:

<table>
<tbody>
<tr class="odd">
<td><p>Column Property Control</p></td>
<td><p>Filter View Control</p></td>
<td><p>Notes</p></td>
</tr>
<tr class="even">
<td><p>Text Box</p></td>
<td><p>Text Box Range</p></td>
<td><p>The Text Box Range control allows users to define a high and/or low range and to use a wildcard when searching in a range.</p></td>
</tr>
<tr class="odd">
<td><p>Text Area</p></td>
<td><p>Text Area Wildcard</p></td>
<td><p>The Text Area Wildcard control provides wildcard pattern matching. If a string without a wildcard character is entered into the Text Area Wildcard control, the wildcard character is automatically appended to the string.</p></td>
</tr>
<tr class="even">
<td><p>HTML Area</p></td>
<td><p>Not Supported</p></td>
<td><p>Columns with an HTML Area Control Type are not supported on the Filter View. The developer must manually hide columns HTML Area Control Types on the Filter View because the DSP® does not automatically hide them. Developers can change the control type for the column to a Text Area or Text Box in the Filter View. However, filter criteria is applied against the HTML source, not the rendered display. For example, a string that includes the ampersand (&amp;) character produces erroneous results because the ampersand is a special character in HTML used for escape sequences.</p></td>
</tr>
<tr class="odd">
<td><p>Check Box</p></td>
<td><p>Options</p></td>
<td><p>A check box is converted into a list of options::</p>
<ul>
<li><strong>Both</strong> – Does not limit the result set. This is the default option.</li>
<li><strong>Checked</strong> – Limits the result set to only those records for which the check box is checked.</li>
<li><strong>Unchecked</strong> – Limits the result set to only those records for which the check box is unchecked.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>List Box</p></td>
<td><p>Selection</p></td>
<td><p>The Selection control allows users to limit results to only those records containing an exact match and follows all the rules of the List control. None is added to all Selection controls. This option does not restrict the result set; it is the default option.</p></td>
</tr>
<tr class="odd">
<td><p>Label</p></td>
<td><p>Ignored</p></td>
<td><p>Columns with a Label Control Type are excluded from the filter view. The Label control is not valid for the Horizontal View, and inherently, labels do not represent data.</p></td>
</tr>
<tr class="even">
<td><p>Button</p></td>
<td><p>Text Box Rang</p></td>
<td><p>Columns with the Button control type use the Text Box Range control. When filtering based on the data in these columns, the filter criteria are applied to the underlying cell value. In the case of buttons, the underlying cell value is rendered as the button label. When filtering on a column with a Button Control Type, the filter criteria applies to the button label. If the cell value is NULL or a zero length string, the column name is used for the button label. In these cases, the same filter rules for NULL and zero length strings apply.</p></td>
</tr>
<tr class="odd">
<td><p>Image</p></td>
<td><p>Text Box Range</p></td>
<td><p>Columns with the Image control types use the Text Box Range control. When filtering based on the data in these columns, the filter criteria are applied to the underlying cell value. Columns specified with an Image Control Type can implement either static or dynamic images.</p>
<p>Static images are defined at the column level and the cell value can be any arbitrary value. For example, a column totals the number of orders per customer. Instead of displaying the number, an image is displayed. To see the number, the user must hover over the image. Since the value is in the result set, it can be used as part of the filter criteria.</p>
<p>With dynamic images, the underlying cell value contains the relative or absolute path to the image. The filter criteria are applied against the image path string.</p></td>
</tr>
<tr class="even">
<td><p>File</p></td>
<td><p>Text Box Range</p></td>
<td><p>Columns with the File control type use the Text Box Range control. When filtering based on the data in these columns, the filter criteria are applied to the underlying cell value. Since the underlying value of a File control is the file path, physical or virtual, filtering a File control produces a filter on the file path string.</p>
<p>In the case of virtual file paths, the filter is only applied to the relative portion of the path because that is the only portion stored in the table.</p></td>
</tr>
<tr class="odd">
<td><p>Combo Box</p></td>
<td><p>Selection</p></td>
<td><p>The Selection control allows users to limit results to only those records containing an exact match and follows all the rules of the List control. None is added to all Selection controls.</p>
<p>This option does not restrict the result set; it is the default option.</p></td>
</tr>
<tr class="even">
<td><p>DateTime</p></td>
<td><p>Text Box Range</p></td>
<td><p>Columns with the DateTime control types use the Text Box Range control. When filtering based on the data in these columns, the filter criteria are applied to the underlying cell value.</p></td>
</tr>
<tr class="odd">
<td><p>Numeric</p></td>
<td><p>Text Box Range</p></td>
<td><p>Columns with the Numeric control types use the Text Box Range control. When filtering based on the data in these columns, the filter criteria are applied to the underlying cell value.</p></td>
</tr>
</tbody>
</table>
