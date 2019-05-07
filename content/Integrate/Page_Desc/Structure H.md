+++
title = 'Structure'
solution = 'Platform'
+++

# Structure

**NOTE**: The fields that display on this page are based on the selected
type. This page is available for [User Defined Fixed Width and Delimited
Template Types](#Structur) and for [XML template
types](#StructureHUser_Defined_XML_Template_Type).

## <span id="Structur"></span>Structure H User Defined Fixed Width and Delimited Template Types

[Structure V  User Defined Template Type](#Structure_V_User_Defined1)

<div class="use">

Use this page to [Create a Delimited or Fixed Width User Defined
Template](../Use_Cases/CreateDelimFWUD.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Integrate \>
    Categories</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Templates</span> icon.
3.  Click <span style="font-weight: bold;">Vertical View</span> for a
    User Defined Template Type of Fixed Width or Delimited.
4.  Click the <span style="font-weight: bold;">Define</span>
icon.

|             |                                                                                                                       |
| ----------- | --------------------------------------------------------------------------------------------------------------------- |
| Field       | Description                                                                                                           |
| PRIORITY    | Displays the order the structure should appear in the flat file.                                                      |
| NAME        | Displays the name of the structure that should appear in the flat file.                                               |
| DESCRIPTION | Displays the description of the structure that should appear in the flat file.                                        |
| FIELDS      | Click to open the *[Structure Field](Struture%20Field.htm)* page to add, edit and delete the fields in the structure. |

###  

## <span id="Structure_V_User_Defined1"></span>Structure V  User Defined Fixed Width and Delimited Template Types

[Structure H  User Defined Template Type](#Structur)

<div class="use">

Use this page to [Create a Delimited or Fixed Width User Defined
Template](../Use_Cases/CreateDelimFWUD.htm).

</div>

Field

Description

Structure Information

Name

Displays the name of the structure that should appear in the flat file.
 

Description

Displays the description of the structure that should appear in the flat
file.

Definition

Fields

Click to open the *[Structure Field](Struture%20Field.htm)* page to add,
edit and delete the fields in the
structure.

 

## <span id="StructureHUser_Defined_XML_Template_Type"></span>Structure H User Defined XML Template Type

[Structure V  User Defined XML Template Type](#Structure_V_User_Defined)

<div class="use">

Use this page to [Configure an XML Template with Structures, Elements
and Attributes](../Use_Cases/ConfigureXMTemplateStrctrEleAtt.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Integrate \>
    Categories</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Templates</span> icon.
3.  Click <span style="font-weight: bold;">Vertical View</span> for a
    User Defined Template Type of XML.
4.  Click the <span style="font-weight: bold;">Define</span> icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the structure appears in the XML file. The Priority field indicates which child structures are below others in the hierarchy. Integrate assigns priority based on the parent structure and order the child structure was added. Priority cannot be updated manually.</p></td>
</tr>
<tr class="odd">
<td><p>NAME</p></td>
<td><p>Displays the structure name.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the structure.</p></td>
</tr>
<tr class="odd">
<td><p>ELEMENT NAME</p></td>
<td><p>Displays the name of the Element in the resulting XML file.  After the structure is saved, the Element name displays surrounded by the tag characters &lt;&gt;. </p>
<p>Because XML is a hierarchical structure, each Element added to the template must be added as a child of an existing structure. </p></td>
</tr>
<tr class="even">
<td><p>Fields</p></td>
<td><p>Click to open the <em><a href="Struture%20Field.htm">Structure Field</a></em> page to add, edit or delete attributes and elements to the child structure.</p></td>
</tr>
<tr class="odd">
<td><p>Add Child Structure</p></td>
<td><p>Click to open the <em><a href="../Use_Cases/AddChildStrXML.htm">Add Child Structure</a></em> page to add a child structure to an existing structure.</p></td>
</tr>
</tbody>
</table>

###  

## <span id="Structure_V_User_Defined"></span>Structure V  User Defined XML Template Type  

[Structure H  User Defined XML Template
Type](#StructureHUser_Defined_XML_Template_Type)

<div class="use">

Use this page to [Configure an XML Template with Structures, Elements
and Attributes](../Use_Cases/ConfigureXMTemplateStrctrEleAtt.htm).

</div>

 

Field

Description

Structure Information

Name

Displays the structure name.

Description

Displays a description of the structure.

Definition

Element Name

Displays the name of the Element in the resulting XML file.  After the
structure is saved, the Element name displays in the *Horizontal* View
surrounded by the tag characters \<\>. 

Because XML is a hierarchical structure, each Element added to the
template must be added as a child of an existing structure. 

Fields

Click to open the *[Structure Field](Struture%20Field.htm)* page to add,
edit or delete attributes and elements to the child structure.
