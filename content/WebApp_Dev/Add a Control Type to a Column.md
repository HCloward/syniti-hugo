+++
title = 'Add a Control Type to a Column'
solution = 'Platform'
+++

# Add a Control Type to a Column

Column properties are specified to control the behavior of the Control
Types, what is displayed: and how values are stored in a table. Before
adding column properties, the control type for the column must be set.

Controls are:

<table>
<tbody>
<tr class="odd">
<td><p>Control</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Button</p></td>
<td><p>Displays a button that can be clicked to perform an action or navigate to another page.</p>
<p>Refer to <a href="Link_to_a_Page_Using_Buttons_and_Images">Link to a Page using Buttons and Images</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Check Box</p></td>
<td><p>Displays a check box that indicates whether a setting is enabled or disabled.</p>
<p>Refer to <a href="Add%20a%20Check%20Box">Add a Check Box</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Combo Box</p></td>
<td><p>Displays a field as a List Box or text box with options from a selected Table or View.</p>
<p>Refer to <a href="Add_List_Boxes_and_Combo_Boxes">Add List Boxes and Combo Boxes</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>DateTime</p></td>
<td><p>Displays a date-formatted field that may or may not accept input.</p></td>
</tr>
<tr class="even">
<td><p>File</p></td>
<td><p>Used to stage any type of file including graphics, text, Word or Excel files. Files are stored in a specific location on the web server and are enabled for download.</p>
<p>Refer to <a href="Enable_File_Upload_Download">Enable File Upload and Download</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>HTML Area</p></td>
<td><p>Provides a tool to format text within the field using bold, italics, colors or additional fonts.</p>
<p>Refer to <a href="Add_an_HTML_Area_to_a_Column">Add an HTML Area to a Column</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Image</p></td>
<td><p>Displays an image that can be clicked to perform an action or navigate to another page. An image can also be used as a column header.</p>
<p>Refer to <a href="Link_to_a_Page_Using_Buttons_and_Images">Link to a Page using Buttons and Images</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Label</p></td>
<td><p>Displays a label to distinguish between Vertical View sections.</p>
<p>Refer to <a href="Add_a_Label">Add a Label</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>List Box</p></td>
<td><p>Displays a field as a List Box or text box with options from a selected Table or View. Refer to <a href="Add_List_Boxes_and_Combo_Boxes">Add List Boxes and Combo Boxes</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Numeric</p></td>
<td><p>Displays a numeric field that can be formatted as currency, percent or other options.</p>
<p>Refer to <a href="Set_a_Columns%20Format">Set a Column's Format</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>tab</p></td>
<td><p>Displays data on different tabs accessible at the top of a Vertical View.</p>
<p>Refer to <a href="Add_a_Tab">Add a tab</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Text Area</p></td>
<td><p>Displays a field to enter more data than can be stored in a text box.</p></td>
</tr>
<tr class="even">
<td><p>Text Box</p></td>
<td><p>Displays a field that allows a user to enter free-form text.</p>
<p><strong>NOTE</strong>: The character limit for a text box is determined by the character limit on the corresponding column in the SQL table.</p></td>
</tr>
<tr class="odd">
<td><p>Toolbar</p></td>
<td><p>Displays a page toolbar with buttons that can be used for page navigation or to perform some action, such as run a rule.</p>
<p>Refer to <a href="../Sys_Admin/Use_Cases/Add%20a%20Toolbar%20Button">Add a Toolbar Button</a> for more information.</p></td>
</tr>
</tbody>
</table>

The steps for adding a control type on the *Horizontal* View of the
*[Page Columns](../Sys_Admin/Page_Desc/Page_Columns_H)* page are
identical, regardless of the control type to be added. After the record
is saved on the *Horizontal* View, the fields that display on the
*Vertical* View depend on the control type added to that column.

The controls available to a column depend on the column’s page’s page
type. Refer to [View the Controls Available For A Pag e
Type](View%20the%20Controls%20Available%20For%20A%20Page%20Type) for
more information.

There are three ways to access the *[Page
Columns](../Sys_Admin/Page_Desc/Page_Columns_H)* page:

  - Select **Admin \> WebApps** in the *Navigation* pane, and click the
    **Pages** icon for a WebApp. Locate the page and click the **Column
    Properties** icon.
  - Navigate to the page in the WebApp where the column property is to
    be applied. Click **Change Settings** on the Site Toolbar, then
    select **Design \>Column Properties**.
  - Navigate to the page in the WebApp where the column property is to
    be applied, right-click the column heading, and click **Add** or
    **Edit** **(Control Name)** if the column property already exists.

To add a control to a column:

1.  <span id="Column Properties Navigation" class="popUpLink">Navigate
    to the *Page Columns* page.</span>

2.  Click **Add**.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H)*.

3.  Select the column in the **COLUMN** list box.
    
    **NOTE:** This list displays the columns from the page’s underlying
    view or table.

4.  Select the view that the column property applies to in the
    <span class="popUpLink">VIEW TYPE</span> list box.
    
    **NOTE:** Refer to [Use View Types with Column
    Properties](Use%20View%20Types%20with%20Column%20Properties) for
    more information.

5.  Select the control from the **CONTROL** list box.

6.  Click **Save**.

Continue with assigning column properties on the *Vertical* View.
