+++
title = 'Link Customization'
solution = 'Platform'
+++

# Link Customization

[Link Customization V](#Link_Customization_V)

<div class="use">

Use this page to [Add Custom Links to a
Page.](../Use_Cases/Add_a_Custom_Link)

</div>

To access this page:

1.  Select **Admin \> Customization \> WebApp Customization** from the
    *Navigation* pane.
2.  Click the **Custom Links** icon for a WEB APP NAME.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PAGE ID</p></td>
<td><p>Displays the name of the page that will contain the custom link.</p></td>
</tr>
<tr class="odd">
<td><p>COLUMN NAME</p></td>
<td><p>Displays the column name that appears as the custom link.</p></td>
</tr>
<tr class="even">
<td><p>VIEW TYPE</p></td>
<td><p>Displays the view type where the custom link will display.</p>
<p>Options are:</p>
<ul>
<li><strong>All Views —</strong> The link displays on views for the page.</li>
<li><strong>Excel —</strong> The link displays on the Excel template downloaded for Excel Integration. Refer to <a href="../../Excel_Int/Use_Excel_Integration">Use Excel Integration</a> for more information.</li>
<li><strong>Horizontal —</strong> The link displays on the <em>Horizontal</em> View only.</li>
<li><strong>Vertical —</strong> The link displays on the <em>Vertical</em> View only.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>CONTROL</p></td>
<td><p>Displays Toolbar. Currently, custom links can only be added to Toolbars.</p></td>
</tr>
<tr class="even">
<td><p>LINK TO PAGE ID</p></td>
<td><p>Displays the name of the page that displays when a user clicks the custom link.</p></td>
</tr>
</tbody>
</table>

## <span id="Link_Customization_V"></span>Link Customization V

[Link Customization H](#Link_Customization)

Use this page to [Add Custom Links to a
Page.](../Use_Cases/Add_a_Custom_Link)

Field

Description

Basic Properties

Image ID

Displays the image that will be added to the toolbar for the custom
link. These images are defined in System Administration \> Configuration
\> Images. To use a custom image, add it to the
<span style="font-style: italic;">Images</span> page to make it
available in this list box.

Link To Page ID

Displays the name of the page that displays when a user clicks the
custom link.

Bind From

Displays the scope of which criteria to include during a link’s
navigation. If the user chooses Selected Row, the selected row’s keys
are included when binding against the target page.

Advanced Properties

Allow Multi Row Action

If enabled, the custom link will be active when multiple rows are
selected in the data grid. If disabled, users cannot navigate using the
custom link if more than one row is selected in the data grid.
