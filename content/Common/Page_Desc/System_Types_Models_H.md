+++
title = 'System Types Models H'
solution = 'Platform'
+++

# System Types Models H

[System Types Models V](#System_Type_Models_V)

<div class="use">

Use this page to:

  - [Add a System Type
    Model](../Use_Cases/Add_a_New_System_Type_Model)
  - [Add a System Type Model
    Table](../Use_Cases/Add_a_New_System_Type_Model_Table).
  - [View Fields Required for System Type
    Tables](../Use_Cases/View%20Fields%20Required%20for%20System%20Type%20Tables)
  - [Add a System Type Model
    Group](../Use_Cases/Add%20a%20System%20Type%20Model%20Group)

</div>

To access this page, select **Configuration \> System Type Models** in
the *Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Model Tables</p></td>
<td><p>Click to open the <em><a href="System_Types_Model_Tables">System Types Model Tables</a></em> page to add tables to a System Type model table.</p>
<p><strong>NOTE:</strong> These tables must exist in the target System Type data source to allow importing from a model.</p></td>
</tr>
<tr class="odd">
<td><p>Model Groups</p></td>
<td><p>Click to open the <em><a href="System_Types_Model_Groups">System Types Model Groups</a></em> page to add tables to a System Type model group.</p></td>
</tr>
<tr class="even">
<td><p>SYSTEM TYPE MODEL</p></td>
<td><p>Displays the name of the database where the data is located. JDE and SAP System Type models are pre-delivered with the product.</p></td>
</tr>
<tr class="odd">
<td><p>DATA SOURCE ID</p></td>
<td><p>Displays the data source of the configured model views.</p></td>
</tr>
<tr class="even">
<td><p>CONNECTION TYPE</p></td>
<td><p>Displays the source connection type for the System Type Model.</p>
<p><strong>NOTE</strong>: The available source connection types are configured in Collect and provide a mapping from the data type supplied in the Table Field Model View to a valid SQL Server data type.</p>
<p><strong>NOTE</strong>: If a mapping does not exist in the connection type, DSP will directly pass the data type from the Table Field Model View into the System Type on import.</p></td>
</tr>
<tr class="odd">
<td><p>MODEL VIEW: TABLE</p></td>
<td><p>Displays a view containing the list of tables with descriptions of the selected System Type.</p></td>
</tr>
<tr class="even">
<td><p>MODEL VIEW: TABLE FIELD</p></td>
<td><p>Displays a view containing the table fields with descriptions and column properties of the selected System Type.</p></td>
</tr>
<tr class="odd">
<td><p>MODEL VIEW: TABLE LOOKUP FIELD</p></td>
<td><p>Displays a view containing the list lookup tables assigned to table fields of the selected System Type.</p></td>
</tr>
<tr class="even">
<td><p>MODEL VIEW: TABLE FIELD STATIC VALUE LIST</p></td>
<td><p>Displays a view containing the list of values assigned to table fields of the selected System Type.</p>
<p><strong>NOTE:</strong> In SAP, these would be the domain values assigned at the data dictionary level.</p></td>
</tr>
<tr class="odd">
<td><p>Model Required For Tables</p></td>
<td><p>Click to open the <em><a href="System_Types_Model_Required_Fields">System Types Model Required Fields</a></em> page to view fields required for the table model view.</p></td>
</tr>
<tr class="even">
<td><p>Model Required For Tables Fields</p></td>
<td><p>Click to open the <em><a href="System_Types_Model_Required_Fields">System Types Model Required Fields</a></em> page to view fields required for the table fields model view.</p></td>
</tr>
<tr class="odd">
<td><p>Model Required For Table Lookup Fields</p></td>
<td><p>Click to open the <em><a href="System_Types_Model_Required_Fields">System Types Model Required Fields</a></em> page to view fields required for the lookup table model view.</p></td>
</tr>
<tr class="even">
<td><p>Model Required For Table Field Domains</p></td>
<td><p>Click to open the the <em><a href="System_Types_Model_Required_Fields">System Types Model Required Fields</a></em> page to view fields required for the lookup table value description model view.</p></td>
</tr>
<tr class="odd">
<td><p>MODEL VIEW: TABLE JOIN</p></td>
<td><p>Displays a view containing the list of table joins by field of the selected System Type.</p></td>
</tr>
<tr class="even">
<td><p>MODEL VIEW: TABLE JOIN FIELD</p></td>
<td><p>Displays a view containing the list of table and field joins by field of the selected System Type.</p></td>
</tr>
<tr class="odd">
<td><p>MODEL VIEW: LOOKUP TABLE VALUE DESCRIPTION</p></td>
<td><p>Displays a list of tables which contain descriptions of the associated lookup table’s values of the selected System Type.</p></td>
</tr>
<tr class="even">
<td><p>Model Required For Table Joins</p></td>
<td><p>Click to open the <em><a href="System_Types_Model_Required_Fields">System Types Model Required Fields</a></em> page to view fields required for the table joins model view.</p></td>
</tr>
<tr class="odd">
<td><p>Model Required For Table Join Fields</p></td>
<td><p>Click to open the <em><a href="System_Types_Model_Required_Fields">System Types Model Required Fields</a></em> page to view fields required for the table field joins model view.</p></td>
</tr>
<tr class="even">
<td><p>Model Required For Descr Table</p></td>
<td><p>Click to open thethe <em><a href="System_Types_Model_Required_Fields">System Types Model Required Fields</a></em> page to view fields required for the description table model view.</p></td>
</tr>
</tbody>
</table>

## <span id="System_Type_Models_V"></span>System Types Models V

[System Types Models H](#System_Type_Models_H)

<div class="use">

Use this page to [Add a System Type Model
Table](../Use_Cases/Add_a_New_System_Type_Model_Table).

</div>

Field

Description

Model Tables

Click to open the *[System Types Model
Tables](System_Types_Model_Tables)* page to add tables to a System
Type model.

Model Groups

Click to open the *[System Types Model
Groups](System_Types_Model_Groups)* page to add tables to a System
Type model group.

Build Views

Click to open the *[System Types Model Build
Views](System_Types_Model_Build_Views)* page to build the views
based on the System Type model.

System Type Model

Displays the name of the database where the data is located for the
selected System Type model.

Data Source ID

Displays the data source ID.

Connection Type

Displays the source connection type for the System Type Model.

**NOTE**: The available source connection types are configured in
Collect and provide a mapping from the data type supplied in the Table
Field Model View to a valid SQL Server data type.

**NOTE**: If a mapping does not exist in the connection type, DSP will
directly pass the data type from the Table Field Model View into the
System Type on import.

Catalog Options

Include Z Column

If enabled, during the catalog export (on the Catalog Phrases page), an
additional phrase entry with a “z”? appended is added to the
catalog. This is so source reports will translate correctly. For
example, zMATNR has a phrase out of Material Number.

If disabled, an additional “z”? phrase is not added to the catalog.

Include Legacy Column

If enabled, during the catalog export (on the Catalog Phrases page), an
additional phrase entry with a “zLegacy”? appended to it is added to the
catalog. This is so source and target reports translate correctly. For
example, zLegacyMATNR has a phrase out of Legacy Material Number.

If disabled, an additional ”zLegacy”? phrase is not added to the
catalog.

Model View: Table

Displays a view containing the list of tables with descriptions of the
selected System Type.

Model View: Table Field

Displays a view containing the table fields with descriptions and column
properties of the selected System Type.

Model View: Table Lookup Field

Displays a view containing the list lookup tables assigned to table
fields of the selected System Type.

Model View: Lookup Table Value Description

Displays a list of tables which contain descriptions of the associated
lookup table’s values of the selected System Type.

Model View: Table Join

Displays a view containing the list of table joins by field of the
selected System Type.

Model View: Table Join Field

Displays a view containing the list of table and field joins by field of
the selected System Type.

Model View: Table Field Static Value List

Displays a view containing the list of values assigned to table fields
of the selected System Type.

**NOTE:** In SAP, these would be the domain values assigned at the data
dictionary level.
