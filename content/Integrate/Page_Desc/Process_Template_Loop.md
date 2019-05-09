+++
title = 'Process Template Loop'
solution = 'Platform'
+++

# Process Template Loop

<div class="use">

Use this page to:

  - [Configure a Process Template Loop for a BDC Script Template with a
    Single Loop](../Use_Cases/ConfigureProcTempLpBDCSingLp)
  - [Configure Process Template Loops for a BDC Script Template with
    Looping Enabled](../Use_Cases/ConfigureProcTempLoopsBDCLoopEn)
  - [Configure a Process Template Loop for a GUI Script Template with a
    Single Loop](../Use_Cases/ConfigProcTmpLpGUISingLp)
  - [Configure Process Template Loops for a GUI Script Template with
    Looping Enabled](../Use_Cases/ConfigureProcTemplLoopsGUILoopgEn)
  - [Configure Process Template Loops for a BAPI
    Template](../Use_Cases/ConfigureProcessTemplateLoopsBAPI)
  - [Configure Process Template Loops for an RFC
    Template](../Use_Cases/ConfigureProcess_emplate_LoopsRFC)
  - [Configure Process Template Loops for an XML
    Template](../Use_Cases/ConfigureProcessTemplateLoopsXML)
  - [Configure Process Template Loops for a Delimited or User Defined
    Template](../Use_Cases/ConfigureProcessTemplateLoopsDelimited)

</div>

<span style="font-weight: bold;">NOTE</span>: This page displays fields
based on the template type associated with the Process template.

To access this page:

1.  Select <span style="font-weight: bold;">Integrate
    \></span>**Categories** from *Navigation pane*.
2.  Click the **Processes** icon for the category.
3.  Click the **Templates** icon for a Process.
4.  Click the **Loops** icon for the template.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Template</p></td>
<td><p>Click to open the <em>Template</em> page with the template from the Process Template Loop displayed.</p></td>
</tr>
<tr class="odd">
<td><p>Relationships</p></td>
<td><p>Click to open the <em>Process Template Loop View Relationship</em> page to view or edit relationships for the loops generated from looped BDC Script or GUI Script templates or from BAPI/RFC templates. Integrate can create these relationships automatically using the Auto Generate Database Objects feature.</p></td>
</tr>
<tr class="even">
<td><p>Auto Generate Database Objects</p></td>
<td><p>Click to have Integrate automatically generate tables and views for the Process Template Loops for any template type and relationships for Process templates based on BDC Script, GUI Script, and BAPI/RFC template types.</p></td>
</tr>
<tr class="odd">
<td><p>INCLUDE</p></td>
<td><p>If enabled, Integrate will include the loop when posting data. If disabled, the loop is excluded.</p>
<p>If enabled, the user can set the <strong>VIEW NAME</strong> and <strong>PRIMARY KEY COLUMN NAME</strong>. If disabled, these fields cannot be edited. This check box is not available when the template type is BDC Script, GUI Script or BAPI.</p></td>
</tr>
<tr class="even">
<td><p>LOOP NAME</p></td>
<td><p>Displays the name of the loop Integrate generated, if the template is based on a BDC Script or GUI Script template. . For User Defined Templates, the structure names defined during template creation become the loop names.  The loop names for a BAPI/RFC template type are based on the structure definitions.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays the description of the loop which is supplied by different sources depending on the template type.</p></td>
</tr>
<tr class="even">
<td><p>VIEW NAME</p></td>
<td><p>Displays the name of the view selected when the process was created or the name of the view that Integrate automatically generated when using the Auto Generate Database Objects feature. A user can also manually set the view if the view exists in the database. This view contains the data that will be posted.</p></td>
</tr>
<tr class="odd">
<td><p>PRIMARY KEY COLUMN NAME</p></td>
<td><p>Displays the column name of the view that uniquely identifies a record in the view.  This column is selected when the process was created or is automatically generated when using the Auto Generate Database Objects feature. This column must be set and can be overwritten by the user.</p></td>
</tr>
<tr class="even">
<td><p>FLAT FILE OBJECT KEY</p></td>
<td><p>Displays the column that contains the key value that links a unique object across multiple structures used for flat file creation. The Flat File Object Key is a unique value for an object that Integrate uses to join the data stored in different tables to make a complete data set for the object. The data set has two loop levels, the header and the details. For example, Integrate uses the flat file object key of 1 in the first loop  the header  to join the header with detail records stored in tables that also have the flat file object key of 1. When posting, batch sizes are based on the number of header records as set by the flat file object key. The Flat File Object Key is used with  User Defined Fixed Width and Delimited template types only.</p></td>
</tr>
<tr class="odd">
<td><p>DOWNLOAD TABLE</p></td>
<td><p>Displays the table where output from SAP will be written.</p>
<p>Displays for process templates based on BAPI/RFC template types only.</p></td>
</tr>
<tr class="even">
<td><p>DOWNLOAD PRIMARY KEY</p></td>
<td><p>Displays the Primary Key Column on the Download table.  The Download Primary Key <strong><span class="underline"><span style="color: #ff0000; text-decoration: none;">must</span></span></strong> be set up to be auto-incrementing to be unique in the database using either an IDENTITY column or a UNIQUEIDENTIFIER column with a default of NEWID  . </p>
<p>Displays for process templates based on BAPI/RFC template types only.</p></td>
</tr>
<tr class="odd">
<td><p>FIELD MAPPINGS</p></td>
<td><p>Click to open the <em>Process Template Loop Field Mappings</em> page to edit field mappings for the Process Template Loop.</p></td>
</tr>
</tbody>
</table>
