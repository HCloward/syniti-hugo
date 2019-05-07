+++
title = 'Automation SQL Target Source'
solution = 'Migration'
+++

# Automation SQL Target Source

<div class="use">

Use this page to [Build a Source
Table](../Use_Cases/Build_Source_Tables.htm).

</div>

To access this page:

1.  Click the **Automation** tab on the Quick Panel.
2.  Click the **Sources** icon for an Object.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Create Source Table</p></td>
<td><p>Click to create the source table and Insert and Delete stored procedures used to load data into the target table.</p>
<p><strong>NOTE:</strong> This icon is disabled if the source is assigned to a Target that has a Design Status of Inactive or Complete in Target Design.</p>
<p><strong>NOTE:</strong> A source table cannot be built for a source of {Target Rules}. If the selected source is {Target Rules}, the Create Source Table icon is disabled.</p>
<p><strong>NOTE:</strong> A System Type must be defined for a source before the table can be built. If the user did not import a System Type in Target Design (for example, an Excel file import, database table import, or manual entry was used for the target design) an error message displays when the user clicks the Create Source Table icon. The user must set a System Type before the table can be created. Add a System Type to a source in Target Design (Design &gt; Targets &gt; Sources &gt; System Type ID).</p></td>
</tr>
<tr class="odd">
<td><p>Create All Rules</p></td>
<td><p>Click to create all rules for field mappings that have a MAPPING STATUS of Complete on the <span style="font-style: italic;"><a href="../../Map/Page_Desc/Field_Mappings_H.htm">Field Mappings</a></span> page in Map. If the Auto Gen Level on the <span style="font-size: 11.0pt;font-family: Arial, sans-serif;font-style: italic;"><a href="Automation_page.htm#Automation_V">Automation</a></span> page’s <span style="font-size: 11.0pt;font-family: Arial, sans-serif;font-style: italic;">Vertical</span> View is set to Off for the target, the rules are not created.</p>
<p><strong>NOTE:</strong> This icon is disabled if the source is assigned to a Target that has a Design Status of Inactive or Complete in Target Design.</p></td>
</tr>
<tr class="even">
<td><p>Map Source</p></td>
<td><p>Click to open the <a href="../../Map/Page_Desc/Target_Sources_H_Map.htm"><span style="font-style: italic;">Target Sources</span></a> page in Map to view information about the source such as a status summary of all mappings, the source schema, and the field mapping details.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE</p></td>
<td><p>Displays the name of the source as defined in Target Design, {Target Rules} if the source is the target rules, or DSPConstruct if the source is built using Construct.</p></td>
</tr>
<tr class="even">
<td><p>ST TABLE NAME</p></td>
<td><p>Displays the name of the source table or view, or indicates if the source is an Update Row source.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE BUILT ON</p></td>
<td><p>Displays the date and time the source table was built (for example, the date a user clicked the Create Source icon in the Page toolbar).</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the source is active for the target. If is not active, rules cannot be created for the source.</p></td>
</tr>
<tr class="odd">
<td><p>Update Row Sources</p></td>
<td><p>Click to open the <a href="Automation_SQL_Target_Source_Update_Row.htm">Automation SQL Target Source (Update Row)</a> page to create Update Row source tables and all rules for an Update Row source.</p></td>
</tr>
<tr class="even">
<td><p>Mappings</p></td>
<td><p>Click to open the <em><a href="Automation_SQL_Field_Mappings_H.htm">Automation SQL Field Mappings</a></em> page to view the mappings that can be used in AutoGen, to create a rule or to reset a mapping.</p></td>
</tr>
<tr class="odd">
<td><p>Log</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="AutoGen_SQL_Log.htm">AutoGen SQL Log</a></span> page and view successful or failed AutoGen tasks.</p>
<p><strong>NOTE:</strong> If the icon is disabled, no source tables, target tables or rules have been generated for the selected object.</p></td>
</tr>
</tbody>
</table>
