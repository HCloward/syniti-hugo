+++
title = 'Variant Import Staging'
solution = 'Data Quality'
+++

# Variant Import Staging

<div class="use">

Use this page to [Import a Variant View for a
Category](../Use_Cases/Import_Views.htm#Import_a_Variant_View_for_a_Category).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspConduct
    \></span>**Configuration \> Category Import View Configuration** in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the **Variant Import Required Columns** icon.

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
<td><p>Import</p></td>
<td><p>Click to import the variant view.</p>
<p><strong>NOTE:</strong> Import only adds or removes variants. Existing variants in the WebApp are not deleted.</p></td>
</tr>
<tr class="odd">
<td><p>Activate</p></td>
<td><p>Click to enable the ACTIVE check box for selected variants.</p>
<p><strong>NOTE:</strong> Enabling the ACTIVE check box for a variant enables all of the associated column settings for the variant.</p></td>
</tr>
<tr class="even">
<td><p>Deactivate</p></td>
<td><p>Click to disable the ACTIVE check box for selected variants.</p>
<p><strong>NOTE:</strong> Disabling the ACTIVE check box for a variant disables all of the associated column settings for the variant.</p></td>
</tr>
<tr class="odd">
<td><p>ACTION</p></td>
<td><p>Displays the action that takes place when the variant is imported.</p>
<p><strong>NOTE:</strong> The variant records in the view are compared to the variants in the WebApp. If the Action field is Change the variant exists in the WebApp for the scenario&gt;role&gt;task combination and it is updated with the values in the view when imported. If the Action field is New Task the variant is not in the WebApp.</p></td>
</tr>
<tr class="even">
<td><p>CATEGORY ID</p></td>
<td><p>Displays the category into which the variant view is being imported.</p></td>
</tr>
<tr class="odd">
<td><p>SCENARIO ROLE TASK ID</p></td>
<td><p>Displays the scenario &gt; role &gt; task combination to which the variant view is applied.</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the variant name in the view.</p></td>
</tr>
<tr class="odd">
<td><p>CONDITIONAL COLUMN</p></td>
<td><p>Displays the column in which the variant logic looks for the value of the variant.</p></td>
</tr>
<tr class="even">
<td><p>OPERATOR</p></td>
<td><p>Displays the logical operator for the variant condition. Default is “=”.</p></td>
</tr>
<tr class="odd">
<td><p>VALUE</p></td>
<td><p>Displays the value for which the variant logic looks.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the variant is imported. If disabled, the variant is not imported.</p></td>
</tr>
<tr class="odd">
<td><p>Columns</p></td>
<td><p>Click to open the <em><a href="Variant_Column_Import_Staging.htm">Variant Column Import Staging</a></em> page to view the column settings for the variant.</p></td>
</tr>
</tbody>
</table>
