+++
title = 'Table (Rule) H'
solution = 'Platform'
+++

# Table (Rule) H

[Table (Rule) V](#Table_Rule_V)

<div class="use">

Use this page to [Register Rules to
Tables](../Use_Cases/Add_Rules_and_Indices_to_Tables#Register_Rules_to_Tables).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Collect \> Targets</span> in
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Sources</span> for target.
3.  Click <span style="font-weight: bold;">Tables</span> for source.
4.  Click <span style="font-weight: bold;">Rules</span> for table.

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
<td><p>PRIORITY</p></td>
<td><p>Displays order that rules are run.</p></td>
</tr>
<tr class="odd">
<td><p>RULE</p></td>
<td><p>Displays name of rule that builds the download package.</p></td>
</tr>
<tr class="even">
<td><p>RULE TYPE</p></td>
<td><p>Displays type of rule.</p>
<p>Values are:</p>
<ul>
<li><strong>Rule</strong> – Performed after the data has been downloaded by the package.</li>
<li><strong>Action</strong> – Generic and performed at the field level, where rules are customized and can be performed against an entire table or single column.</li>
</ul>
<p>Default value is <strong>Action</strong></p></td>
</tr>
<tr class="odd">
<td><p>PRECEDENCE</p></td>
<td><p>Displays execution order to determine whether the rule runs before or after download process.</p>
<p>Values are: After, Before</p>
<p>Default value is <strong>After</strong></p></td>
</tr>
<tr class="even">
<td><p>FIELDNAME</p></td>
<td><p>Displays field name impacted by action (does not apply to rules).</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If enabled, rule or action is available for processing. Default value is Active.</p></td>
</tr>
<tr class="even">
<td><p>ADD TARGET DB PARAM</p></td>
<td><p>If enabled, the database parameter is added to the stored procedure when the rule or action is run. This field is helpful when rules are stored in Collect database and run in another database; users are able to clearly see the originating database.  Default is Disabled.</p></td>
</tr>
<tr class="odd">
<td><p>WHERE CLAUSE</p></td>
<td><p>Displays a Where Clause that limits the rule to run only part of the data.</p></td>
</tr>
</tbody>
</table>

### <span id="Table_Rule_V"></span>Table (Rule) V

[Table (Rule) H](Table_Rule_H)

<div class="use">

Use this page to [Register Rules to
Tables](../Use_Cases/Add_Rules_and_Indices_to_Tables#Register_Rules_to_Tables).

</div>

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
<td><p>Priority</p></td>
<td><p>Displays order that rules are run.</p></td>
</tr>
<tr class="odd">
<td><p>Rule</p></td>
<td><p>Displays name of rule that builds the download package.</p></td>
</tr>
<tr class="even">
<td><p>Rule Type</p></td>
<td><p>Displays type of rule.</p>
<p>Values are:</p>
<ul>
<li><strong>Rule</strong> – Performed after the data has been downloaded by the package.</li>
<li><span style="font-size: 11pt;font-family: Arial, sans-serif;"><strong>Action</strong> – Generic and performed at the field level, where rules are customized and can be performed against an entire table or single column.</span></li>
</ul>
<p>Default value is <strong>Action</strong>.</p></td>
</tr>
<tr class="odd">
<td><p>Precedence</p></td>
<td><p>Displays execution order to determine whether the rule runs before or after download process.</p>
<p>Values are: After, Before</p>
<p>Default value is <strong>After</strong>.</p></td>
</tr>
<tr class="even">
<td><p>FieldName</p></td>
<td><p>Displays field name impacted by action (does not apply to rules).</p></td>
</tr>
<tr class="odd">
<td><p>Active</p></td>
<td><p>If enabled, rule or action is available for processing. Default value is Active.</p></td>
</tr>
<tr class="even">
<td><p>Add Target DB Param</p></td>
<td><p>If enabled, the database parameter is added to stored procedure when rule or action is run. This field is helpful when rules are stored in Collect database and run in another database; users are able to clearly see the originating database.  Default is Disabled.</p></td>
</tr>
<tr class="odd">
<td><p>Where Clause</p></td>
<td><p>Displays a Where Clause that limits the rule or action to run only part of the data.</p></td>
</tr>
<tr class="even">
<td><p>Comment</p></td>
<td><p>Displays notes about rule or action, e.g., description of what the rule does.</p></td>
</tr>
<tr class="odd">
<td><p>Spec ID</p></td>
<td><p>Displays client’s specification for a custom rule or action.</p></td>
</tr>
<tr class="even">
<td><p>Publish Group</p></td>
<td><p>Displays name of group that the table is published with.</p></td>
</tr>
<tr class="odd">
<td><p>Duration</p></td>
<td><p>Displays amount of time (in seconds) the rule took to run.</p></td>
</tr>
<tr class="even">
<td><p>Record Count</p></td>
<td><p>Displays the number of records affected by the rule or action (which may be limited if a Where clause is applied).</p></td>
</tr>
<tr class="odd">
<td><p>Job ID</p></td>
<td><p>Displays unique identifier associated with the job that ran the rule or action.</p></td>
</tr>
<tr class="even">
<td><p>Rule Preview</p></td>
<td><p>Displays the SQL for the rule after the user clicks Generate Rule Preview.</p></td>
</tr>
<tr class="odd">
<td><p>Generate Rule Preview</p></td>
<td><p>Click to generate a preview of the SQL for the rule.</p></td>
</tr>
</tbody>
</table>
