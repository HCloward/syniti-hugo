# Process Templates H

[Process Templates V](#Process_Templates_V)

<div class="use">

Use this page to [Add Templates to a
Process](../Use_Cases/Add_Templates_to_a_Process.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Integrate \>
    </span>**Categories** from *Navigation* pane.
2.  Click the **Processes** icon for a category.
3.  Click the **Templates** icon for a process.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the process templates are processed.</p></td>
</tr>
<tr class="odd">
<td><p>TEMPLATE ID</p></td>
<td><p>Displays the name of the template associated with the process.</p></td>
</tr>
<tr class="even">
<td><p>Allowed Connections</p></td>
<td><p>Click to open the <a href="Process_Template_Connections.htm">Process Template Connections</a> page to modify the connections for the process template.</p>
<p>The count on the icon is the number of connections that exist for the selected process template.</p></td>
</tr>
<tr class="odd">
<td><p>Loops</p></td>
<td><p>Click to open the<a href="Process_Template_Loop.htm"><em>Process Template Loop</em></a> page to view and edit the loops in this process template. The number is the total number of loops in the template process  whether the loops are included or not.</p></td>
</tr>
<tr class="even">
<td><p>After Post Rules</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="../../../Master_Data_Mgmt/dspConduct/Page_Desc/Process_Templates_After_Post_Rules_H.htm">Process Templates: After Post Rules</a></span> page to register rules that run after the selected process template finishes posting.</p></td>
</tr>
</tbody>
</table>

## <span id="Process_Templates_V"></span>Process Templates V

[Process Templates H](Process_Templates_H.htm)

<div class="use">

Use this page to:

  - [Configure Process Template Loops for an XML
    Template](../Use_Cases/ConfigureProcessTemplateLoopsXML.htm)
  - [Configure Process Template Loops for a Delimited or User Defined
    Template](../Use_Cases/ConfigureProcessTemplateLoopsDelimited.htm)

</div>

This page has the following tabs:

  - [General tab](#General_Tab)
  - [Copy tab](#Copy_Tab)

## <span id="General_Tab"></span>General tab

Field

Description

Basic

Template ID

Displays the name of the template associated with the process.

File Creation Settings

Folder

Displays the path and folder name of the folder on the server where the
files should be stored. The default value is set in Common, on the
*Integrate – Parameters* page. Displays for  User Defined template types
only.

Data Source ID

Displays the ID of the data source to which files should be transferred
after they are created.

Flat File Submit Settings

No Data Symbol

Displays a symbol to represent “no data” in the process post. If the
field is blank, Integrate uses an empty
string.

## <span id="Copy_Tab"></span>Copy tab

|                       |                                                                                                                                                                                                                                                                                                                                                                                                          |
| --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                 | Description                                                                                                                                                                                                                                                                                                                                                                                              |
| Copy Process Template | <span style="font-size: 11.0pt;line-height: 107%;font-family: Calibri, sans-serif;">Click to open the </span><span style="font-size: 11.0pt;line-height: 107%;font-family: Calibri, sans-serif;font-style: italic;">[Copy](Copy.htm)</span><span style="font-size: 11.0pt;line-height: 107%;font-family: Calibri, sans-serif;"> page to create a process template based on this process template.</span> |
