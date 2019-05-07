+++
title = 'Automation SQL Target Source (Update Row)'
solution = 'Migration'
+++

# Automation SQL Target Source (Update Row)

<div class="use">

Use this page to:

  - [Build an Update Row Source Table Using SQL
    AutoGen](../Use_Cases/Build_an_Update_Row_Source_Table.htm)
  - [Create Rules for an Update Row Source Using SQL
    AutoGen](../Use_Cases/Create_Rules_for_an_Update_Row_Source.htm)

</div>

To access this page:

1.  Click the **Automation** tab in the Quick Panel.
2.  Click the **Sources** icon for a Target.
3.  Click the <span style="font-weight: bold;">Update Row Sources</span>
    icon for a Source in the Parent pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Create Source Table</p></td>
<td><p>Click to create the Update Row source table and Insert and Delete stored procedures used to load data into the target table.</p>
<p><strong>NOTE:</strong> This icon is disabled if the source is assigned to a Target that has a Design Status of Inactive or Complete in Target Design.</p>
<p><strong>NOTE:</strong> A source table cannot be built for a source of {Target Rules}. If the selected source is {Target Rules}, the Create Source Table icon is disabled.</p>
<p><strong>NOTE:</strong> A System Type must be defined for a source before the table can be built. If the user did not import a System Type in Target Design (for example, an Excel file import, database table import, or manual entry was used for the target design) an error message displays when the user clicks the Create Source Table icon. The user must set a System Type before the table can be created. Add a System Type to a source in Target Design (Design &gt; Targets &gt; Sources &gt; System Type ID).</p>
<p>Refer to <a href="../Use_Cases/Build_an_Update_Row_Source_Table.htm">Build an Update Row Source Table Using SQL AutoGen</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Create All Rules</p></td>
<td><p>Click to create all rules for field mappings for the Update Row source that have a MAPPING STATUS of Complete on the <em><a href="../../Map/Page_Desc/Field_Mappings_H.htm">Field Mappings</a></em> page in Map. </p>
<p><strong>NOTE:</strong> This icon is disabled if the source is assigned to a Target that has a Design Status of Inactive or Complete in Target Design.</p>
<p>Refer to <a href="../Use_Cases/Create_Rules_for_an_Update_Row_Source.htm">Create Rules for an Update Row Source Using SQL AutoGen</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>UPDATE SOURCE VIEW</p></td>
<td><p>Displays the name of the source as defined in Target Design.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE BUILT ON</p></td>
<td><p>Displays the date and time the source table was built (for example, the date a user clicked the Create Source icon in the Page toolbar).</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If checked, the source is active for the target.</p>
<p><strong>NOTE:</strong> If unchecked, the source is not active, and rules cannot be created for the source.</p></td>
</tr>
<tr class="odd">
<td><p>Mappings</p></td>
<td><p>Click to open the <em><a href="Automation_SQL_Field_Mappings_H.htm">Automation SQL Field Mappings</a></em> page to view the mappings that can be used in AutoGen, to create a rule, or to reset a mapping for the Update Row source.</p></td>
</tr>
<tr class="even">
<td><p>Log</p></td>
<td><p>Click to open the <em><a href="AutoGen_SQL_Log.htm">AutoGen SQL Log</a></em> page and view successful or failed AutoGen tasks.</p>
<p><strong>NOTE:</strong> If the icon is disabled, no source tables, target tables or rules have been generated for the selected object.</p></td>
</tr>
</tbody>
</table>
