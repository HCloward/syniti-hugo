+++
title = 'Relationship Joins H'
solution = 'Migration'
+++

# Relationship Joins H

[Relationship Joins V](#RelationshipV)

<div class="use">

Use this page to [Add Relationship Joins to
Sources.](../Use_Cases/Add_Relationship_Joins_to_Source.htm)

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Map</span> in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area Launch](Process_Area_Launch_map.htm)* page.
4.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target in the Parent pane.
5.  Click the **Update Row Sources** icon for a Target Source in the
    Child pane.
6.  Click the **Secondary Source** icon for a Target Source (Add Row) in
    the Parent pane.
7.  Click the <span style="font-weight: bold;">Relationships</span> icon
    for the Target Source (Update Row) in the Child pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the name of the relationship, for example Join MARA to MARC (Material to Plants).</p></td>
</tr>
<tr class="odd">
<td><p>RIGHT TABLE</p></td>
<td><p>Displays the rule source table name where the SQL for the join is stored.</p>
<p><strong>NOTE:</strong> This is the Update Row source defined for the Add Row source.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE DATABASE OBJECT ID</p></td>
<td><p>Displays the source object within the database, which may be different from the Source Rule table. This value is inherited from the Source Database Object field on the <em><a href="Target_Sources_H_Map.htm">Target Sources</a></em> page in Map.</p></td>
</tr>
<tr class="odd">
<td><p>JOIN SQL</p></td>
<td><p>Displays the SQL join code to be appended to the rules.</p></td>
</tr>
<tr class="even">
<td><p>Fields</p></td>
<td><p>Click to open the <em><a href="Relationship_Fields.htm">Relationship Fields</a></em> page to edit fields used in the relationship.</p></td>
</tr>
</tbody>
</table>

## <span id="RelationshipV"></span>Relationship Joins V

[Relationship Joins H](#)

<div class="use">

Use this page to [Add Relationship Joins to
Sources.](../Use_Cases/Add_Relationship_Joins_to_Source.htm)

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Name</p></td>
<td><p>Displays the name of the relationship, for example Join MARA to MARC (Material to Plants).</p></td>
</tr>
<tr class="odd">
<td><p>Lock</p></td>
<td><p>If checked, the join cannot be deleted.</p>
<p><strong>NOTE:</strong> The check box is enabled by default if the join was auto-built from Target Design.</p>
<p>This check box only displays for joins between target tables.</p></td>
</tr>
<tr class="even">
<td><p>Comment</p></td>
<td><p>Displays a user-entered comment about the relationship join.</p></td>
</tr>
<tr class="odd">
<td><p>Join SQL</p></td>
<td><p>Displays the SQL join code to be appended to the rules.</p></td>
</tr>
<tr class="even">
<td><p>Where Clause</p></td>
<td><p>Displays the Where Clause used for the relationship to apply the JOIN correctly during auto-generation.</p></td>
</tr>
</tbody>
</table>
