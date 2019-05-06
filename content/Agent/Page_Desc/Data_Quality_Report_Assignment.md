# Data Quality Report Assignment

<div class="use">

Use this page to [Configure the IGC Migration
dashboard](../Use_Cases/Configure_the_Migration_Dashboard.htm).

</div>

To access this page:

1.  Select **Agent Interface \> Dashboards \> Migration Dashboard** in
    the *Navigation* pane.
2.  Click the **Data Quality Report Assignment** icon for a wave.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>WAVE PROCESS AREA ID</p></td>
<td><p>Displays the name of the wave-process area combination for which the error and opportunity reports are selected.</p></td>
</tr>
<tr class="odd">
<td><p>WAVE PROCESS AREA OBJECT ID</p></td>
<td><p>Displays the name of the wave-process area-object combination for which the error and opportunity reports are selected.</p></td>
</tr>
<tr class="even">
<td><p>WAVE PROCESS AREA OBJECT TARGET ID</p></td>
<td><p>Displays the name of the wave-process area-object-target combination for which the error and opportunity reports are selected.</p></td>
</tr>
<tr class="odd">
<td><p>TYPE</p></td>
<td><p>Displays how data in the Target table moves through the migration process.</p>
<ul>
<li><strong>Natural</strong> — The Target follows the standard migration process. The Target fields and Source must be entered or imported into Target Design and synced to Map. Map must have Source tables selected and fields mapped. SQL AutoGen creates the Target table, Source table, and rules Objects.</li>
<li><strong>Utility</strong> — The Target is not mapped in Map and SQL AutoGen does not create any Objects. A user must still enter the Target into Target Design and the Target’s fields and Sources. The Target tables, Source Tables and rule Objects must be created manually.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>DATA QUALITY OPPORTUNITY REPORT</p></td>
<td><p>Displays the name of the opportunity report used in the Quality metrics calculation.</p>
<p><strong>NOTE:</strong> The Quality metric indicates the data quality of the wave. This percentage is calculated using the totals on the error reports registered to the wave and targets (post load reports) divided by the total number of records on the opportunity reports registered to the waves and targets (preload reports).</p>
<p><strong>NOTE:</strong> For reports to display in this list box, they must follow the proper naming conventions.</p>
<ul>
<li>tv[InformalTableName]_[FieldName]_[Description]Sel or</li>
<li>tv[InformalTableName]_[FieldName]Sel or</li>
<li>tv[InformalTableName]_[Description]Sel</li>
</ul>
<p>Refer to <a href="../../../Migration/Transform/Use_Cases/Naming_Conventions.htm">Naming Conventions</a> and <a href="../../WebApp_Dev/Naming_Conventions_and_the_Enforce_Strict_Naming_Feature.htm">Naming Conventions and the Enforce Strict Naming Feature</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>DATA QUALITY ERROR REPORT</p></td>
<td><p>Displays the name of the error report used in the Quality metrics calculation.</p>
<p><strong>NOTE:</strong> For reports to display in this list box, they must follow the proper naming conventions.</p>
<ul>
<li>tv[InformalTableName]_[FieldName]_[Description]Sel or</li>
<li>tv[InformalTableName]_[FieldName]Sel or</li>
<li>tv[InformalTableName]_[Description]Sel</li>
</ul>
<p>Refer to <a href="../../../Migration/Transform/Use_Cases/Naming_Conventions.htm">Naming Conventions</a> and <a href="../../WebApp_Dev/Naming_Conventions_and_the_Enforce_Strict_Naming_Feature.htm">Naming Conventions and the Enforce Strict Naming Feature</a> for more information.</p></td>
</tr>
</tbody>
</table>
