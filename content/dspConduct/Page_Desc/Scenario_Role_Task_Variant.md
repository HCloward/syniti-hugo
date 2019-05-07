+++
title = 'Scenario Role Task Variant'
solution = 'Master Data Management'
+++

# Scenario Role Task Variant

<div class="use">

Use this page to [Activate and Configure Column
Variants](../Use_Cases/Activate_Configure_Column_Variants.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspConduct
    \></span>**Design** in the *Navigation* pane.
2.  Click the **Scenarios** icon for a category on the *Category* page.
3.  Click the **Roles** icon.
4.  Click the **Tasks** icon on the *Scenario (Roles)* page.
5.  Click the **Variants** icon;

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
<td><p>Click to activate the column variant. When activated the variant can be configured on the <em><a href="Scenario_Role_Task_Column_H.htm">Scenario Role Task Column</a></em> page.</p></td>
</tr>
<tr class="odd">
<td><p>Deactivate</p></td>
<td><p>Click to deactivate the column variant. When deactivated, the variant is not displayed on the <em><a href="Scenario_Role_Task_Column_H.htm">Scenario Role Task Column</a></em> page.</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the name of the variant.</p></td>
</tr>
<tr class="odd">
<td><p>COLUMN</p></td>
<td><p>Displays the column in which the variant logic looks for the value of the variant.</p></td>
</tr>
<tr class="even">
<td><p>OPERATOR</p></td>
<td><p>Displays the logical operator for the variant condition.</p></td>
</tr>
<tr class="odd">
<td><p>CONSTANT</p></td>
<td><p>Displays the value for which the variant logic looks. When this value is encountered in a record in the column indicated in the COLUMN field, the Control Status and Required settings are applied to other columns as indicated on the <em><a href="Scenario_Role_Task_Column_H.htm">Scenario Role Task Column</a> page.</em></p>
<p>For example, for raw materials records in a Material table a Designer can change the default Control Status for the Sales Price column to Hide (because raw materials are not sold) by establishing a variant that looks for the condition material type column = value raw materials (MTART = ‘ROH').</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled the variant is active and applied to the columns as indicated on the <em><a href="Scenario_Role_Task_Column_H.htm">Scenario Role Task Column</a></em> page. If disabled the variant is not applied.</p></td>
</tr>
</tbody>
</table>
