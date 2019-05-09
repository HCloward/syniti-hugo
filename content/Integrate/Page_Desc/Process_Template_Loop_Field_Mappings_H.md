+++
title = 'Process Template Loop Field Mappings H'
solution = 'Platform'
+++

# Process Template Loop Field Mappings H

[Process Template Loop Field Mappings V](#Process_Template_Loop1)

<div class="use">

Use this page to:

  - [Configure Field Mappings for a Process Based on a BDC Script
    Template](../Use_Cases/ConfigureFieldMappingsBDC_Script_Template)
  - [Configure Field Mappings for a Process Based on a GUI Script
    Template](../Use_Cases/ConfigureFieldMappingsGUI_Script_Template)
  - [Configure Field Mappings for a Process Based on an
    RFC](../Use_Cases/VwConfigureFldMappingsProcRFC)
  - [Configure Field Mappings for a Process Based on a
    BAPI](../Use_Cases/ViewandConfigureFieldMappingsBAPI)

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Integrate \>
    </span><span style="font-family: Arial, sans-serif;">**Categories** from *Navigation
    pane*.</span>
2.  Click the **Processes** icon for the category.
3.  Click the **Templates** icon for a process.
4.  Click the **Loops** icon for the template.
5.  Click the **Fields Mappings** icon for a loop level.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>TEMPLATE FIELD UNIQUE NAME</p></td>
<td><p>Displays the name of the field in the template to be mapped to a column in the view for the process template loop.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the field, provided by different sources depending on the template type.</p></td>
</tr>
<tr class="even">
<td><p>MAPPING VALUE</p></td>
<td><p>Displays the field in the view that Integrate maps to the template field unique name. Integrate may automatically generate this value while creating the process template loop, or when using the Auto Generate Database Objects feature and it is usually identical to the <strong>TEMPLATE FIELD UNIQUE NAME</strong>. A user can also update this field manually.</p>
<p><strong>NOTE:</strong> If neither a <strong>MAPPING VALUE</strong> nor a <strong>FIXED VALUE</strong> is set, Integrate will ignore the field during the posting.</p></td>
</tr>
<tr class="odd">
<td><p>FIXED VALUE</p></td>
<td><p>Displays the fixed value assigned to the template field.</p>
<p><strong>NOTE:</strong> If neither a <strong>MAPPING VALUE</strong> nor a <strong>FIXED VALUE</strong> is set, Integrate will ignore the field during the posting</p></td>
</tr>
<tr class="even">
<td><p>RV</p></td>
<td><p>If enabled, the field uses a return value from a template with a lower priority as the value for the field.</p></td>
</tr>
</tbody>
</table>

## <span id="Process_Template_Loop1"></span>Process Template Loop Field Mappings V

[Process Template Loop Field Mappings
H](Process_Template_Loop_Field_Mappings_H)

Field

Description

Field

Template Field Unique Name

Displays the name of the field in the template to be mapped to a column
in the view for the process template loop.

Description

Displays a description of the field, provided by different sources
depending on the template type.

Return Value Mapping

Return Value Template ID

Displays the template selected from the multi-template process that
contains the return value to use with transaction stringing. Available
for process templates based on GUI Script, BDC Script or BAPI/RFC
templates only.

Return Value

Displays the return value from SAP that the template uses with
transaction stringing to map to the selected field in the template.
Available for process templates based on GUI Script or BDC Script or
BAPI/RFC templates only.
