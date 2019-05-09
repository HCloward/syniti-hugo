+++
title = 'Variant Column Import Staging'
solution = 'Master Data Management'
+++

# Variant Column Import Staging

<div class="use">

Use this page to [Import a Variant View for a
Category](../Use_Cases/Import_Views#Import_a_Variant_View_for_a_Category).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspConduct
    \></span>**Configuration \> Category Import View Configuration** in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Select a category.
3.  Click the <span style="font-weight: bold;">Import Variants</span>
    icon.
4.  Click the **Columns** icon.

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
<td><p>Activate</p></td>
<td><p>Click to enable the ACTIVE check box for selected variants.</p></td>
</tr>
<tr class="odd">
<td><p>Deactivate</p></td>
<td><p>Click to disable the ACTIVE check box for selected variants.</p></td>
</tr>
<tr class="even">
<td><p>ACTION</p></td>
<td><p>Displays the action that takes place when the column setting is imported.</p>
<p><strong>NOTE:</strong> The column settings in the view are compared to the column settings in the WebApp. If the Action field is Change, the column settings exist in the WebApp and it is updated with the values in the view when imported. If the Action field is New Task, the column settings are not in the WebApp and are added when the view is imported.</p></td>
</tr>
<tr class="odd">
<td><p>COLUMN PAGE ID</p></td>
<td><p>Displays the ID of the page on which the column displays.</p></td>
</tr>
<tr class="even">
<td><p>PAGE COLUMN</p></td>
<td><p>Displays the column name.</p></td>
</tr>
<tr class="odd">
<td><p>CONTROL STATUS</p></td>
<td><p>Displays the status setting of the column on the page for the scenario &gt; role &gt;task combination.</p>
<p>Values are:</p>
<ul>
<li><strong>Disabled</strong> – Column displays but is not editable.</li>
<li><strong>Enabled</strong> – Column displays and is editable.</li>
<li><strong>Hide</strong> – Column does not display.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>REQUIRED</p></td>
<td><p>If enabled, indicates that this is defined as a required column within the scenario &gt; role &gt; task combination. If disabled, indicates that this is not defined as a required column within the scenario &gt; role &gt;task combination.</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the column settings are imported. If disabled, the column settings are not imported.</p></td>
</tr>
</tbody>
</table>
