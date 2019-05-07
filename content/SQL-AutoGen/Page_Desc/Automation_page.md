+++
title = 'Automation H'
solution = 'Migration'
+++

# Automation H

[Automation V](#Automation_V)

<div class="use">

Use this page to:

  - [Build Target Tables](../Use_Cases/Build_Target_Tables.htm)
  - [Create Rules](../Use_Cases/Create_Rules.htm)
  - [Build Reports](../Use_Cases/Build_Reports.htm)
  - [Build and Refresh Data Services
    Jobs](../../Data_Services_AutoGen/Use_Cases/Build_and_Refresh_DS_Jobs.htm)

</div>

To access this page, click the **Automation** tab in the Quick Panel.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Create Target Table</p></td>
<td><p>Click to create a target table for the selected object based on the settings in Target Design. The tables are written to the data source defined for the object in Console.</p>
<p><strong>NOTE:</strong> A System Type must be defined for a target before the table can be built. If the user did not import a System Type in Target Design (for example, an Excel file import, database table import, or manual entry was used for the target design), an error message displays when the user clicks the Create Target Table icon. The user must set a System Type before the table can be created. Add a System Type to a target in Target Design (Design &gt; Targets &gt; Vertical View for a target &gt; System Type ID).</p>
<p><strong>NOTE:</strong> If a table exists in the database, this icon is disabled until the target is synced with Map.</p></td>
</tr>
<tr class="odd">
<td><p>Create All Rules</p></td>
<td><p>Click to create all rules for the target and source for the selected object based on mappings submitted in Map. The rules are written to the data source defined for the object in Console.</p></td>
</tr>
<tr class="even">
<td><p>Build Reports</p></td>
<td><p>Click to build target and source reports (added as a view in the database) for the selected object. The reports are written to the data source defined for the object in Console.</p></td>
</tr>
<tr class="odd">
<td><p>Build Reports with Remediation</p></td>
<td><p>Click to build target remediation reports (added as a view in the database) for the selected object. These error reports become the basis of remediation rules.</p></td>
</tr>
<tr class="even">
<td><p>Build and Refresh Data Services</p></td>
<td><p>Click to open the <a href="../../Data_Services_AutoGen/Page_Desc/AutoGen_Data_Services.htm"><span style="font-style: italic;">AutoGen Data Services</span></a> page to auto-generate Data Services Jobs for the selected target.</p></td>
</tr>
<tr class="odd">
<td><p>Create and Approve Rules</p></td>
<td><p>Click to create and approve all rules for the object that have a Mapping Status of Complete.</p>
<p>Rules are not generated for mappings in any other Mapping Status.</p>
<p>Rules are written to the data source defined for the object in Console.</p></td>
</tr>
<tr class="even">
<td><p>Create All Objects</p></td>
<td><p>Click to create all objects using SQL AutoGen. The target table, source table, Update Row source table (if used) and rules are automatically created.</p></td>
</tr>
<tr class="odd">
<td><p>OBJECT</p></td>
<td><p>Displays the name of the object as created in Console.</p></td>
</tr>
<tr class="even">
<td><p>TARGET</p></td>
<td><p>Displays the name of the target as created in Target Design.</p></td>
</tr>
<tr class="odd">
<td><p>Sources</p></td>
<td><p>Click to open the <em><a href="Automation_SQL_Target_Source.htm">Automation SQL Target Source</a></em> page to create a source table and rules for a source.</p>
<p>The count on this icon represents the number of sources assigned to the target in Target Design.</p></td>
</tr>
<tr class="even">
<td><p>Target Rules</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Automation_SQL_Field_Mappings_H.htm">Automation SQL Field Mappings</a></span> page to Create, Reset or Reject a Target Rule Only mapping and to view the mappings that can be used in SQL AutoGen to create a rule.</p>
<p>The count on this icon represents the total number of Target Rule mappings. A mapping is complete when the Mapping Status is set to Complete and Submitted on the <span style="font-style: italic;"><a href="../../Map/Page_Desc/Field_Mappings_H.htm">Field Mappings</a></span> page in Map. If a target field has a basic or complex rule added, this rule bypasses Map and is considered complete by AutoGen.</p></td>
</tr>
<tr class="odd">
<td><p>Mappings</p></td>
<td><p>Click to open the <em><a href="Automation_SQL_Field_Mappings_H.htm">Automation SQL Field Mappings</a></em> page to reset a mapping and to view the mappings that can be used in SQL AutoGen to create a rule.</p>
<p>The count on this icon represents the number of mappings that are completed and can have rules auto-generated. A mapping is complete when the Mapping Status is set to Complete on the <span style="font-style: italic;"><a href="../../Map/Page_Desc/Field_Mappings_H.htm">Field Mappings</a></span> page in Map. If a target field has a basic or complex rule added, this rule bypasses Map and is considered complete by AutoGen.</p></td>
</tr>
<tr class="even">
<td><p>Log</p></td>
<td><p>Click to open the <em><a href="AutoGen_SQL_Log.htm">AutoGen SQL Log</a></em> page and view successful or failed AutoGen tasks.</p>
<p><strong>NOTE:</strong> If the icon is disabled, no source tables, target tables or rules have been generated for the selected object.</p></td>
</tr>
</tbody>
</table>

## <span id="Automation_V"></span>Automation V

Automation H

<div class="use">

Use this page to [Set the Auto Gen Level for a
Target](../Use_Cases/Set_the_Auto_Gen_Level_for_a_Target.htm).

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Object</p></td>
<td><p>Displays the name of the object as created in Console.</p></td>
</tr>
<tr class="odd">
<td><p>Description</p></td>
<td><p>Displays a description of the object.</p></td>
</tr>
<tr class="even">
<td><p>Auto Gen Level</p></td>
<td><p>Displays an option indicating if and how tables, views and stored procedures are autogenerated.</p>
<p>Values are:</p>
<ul>
<li><strong>New Rules – Alter Table and Build New Views and Stored Procedures Only –</strong> When autogenerating, a table is updated and only new views and stored procedures are created. Existing views and stored procedures are not updated.</li>
<li><p><strong>Off – No Generating Any SQL Objects –</strong> AutoGen is not used.</p>
<p><strong>NOTE:</strong> Rules for mappings with the Copy, Default, Rule, XRef, and Xref actions are not built. For mappings with the Construction action (for example, mappings that use Enhanced Construction), the table and field are not created in the target database and a page is not created in Construct. Full Construction objects are built via the Sync in Target Design. The rules must be generated on the <span style="font-style: italic;"><a href="Automation_SQL_Field_Mappings_H.htm">Automation SQL Field Mappings</a></span> page. Refer to <a href="../Use_Cases/Create_Rules.htm">Create Rules using SQL AutoGen</a> for more information.</p></li>
<li><strong>On – Drop &amp; Rebuild Table, Views and Stored Procedures –</strong> Any SQL objects previously created for the target are dropped and a new table, SQL views and stored procedures with the same name are added.</li>
<li><strong>Rebuild – Alter Table and Drop &amp; Rebuild Views And Stored Procedures –</strong> The table is updated. Views and stored procedures previously created for the target are dropped and new SQL views and stored procedures with the same name are added.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Report Auto Gen Level</p></td>
<td><p>Displays an option indicating if and how business user reports are generated for the target with SQL AutoGen.</p>
<p>Options are:</p>
<ul>
<li><strong>On - Drop &amp; Rebuild Report Views and Registrations –</strong> Any SQL views previously created for the business user reports in the target are dropped and new SQL views with the same name are added.</li>
<li><strong>Off - No Report Generation –</strong> AutoGen is not used.</li>
<li><strong>New - Add new reports without modifying existing report views or registrations –</strong> When autogenerating, only new views are created. Existing views are not updated.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Built On</p></td>
<td><p>Displays the date the SQL objects were created.</p>
<p><strong>NOTE:</strong> If the objects have not yet been built, or the Auto Gen Level is Off, this field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>Built By</p></td>
<td><p>Displays the name of the user who built the objects.</p>
<p><strong>NOTE:</strong> If the objects have not yet been built, or the Auto Gen Level is Off, this field is blank.</p></td>
</tr>
</tbody>
</table>
