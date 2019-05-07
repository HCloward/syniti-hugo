+++
title = 'Package Types'
solution = 'Platform'
+++

# Package Types

Package Types are ways in which data is downloaded from the source. The
following table outlines the various package types supported in Collect:

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Package Type</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>BOA RFC</p></td>
<td><p>Uses Remote Function Calls from SAP to download data. This is a modified form of SAPRFC, and BackOffice recommends BOARFC over SAPRFC</p></td>
</tr>
<tr class="odd">
<td><p>BOA RFC using Options</p></td>
<td><p>Uses Remote Function Calls  from SAP with the added ability to include extra filters. Only use this if  the BOA RFC options are needed</p></td>
</tr>
<tr class="even">
<td><p>CranPort                             </p></td>
<td><p>Uses a CranPort package.</p>
<p><strong>NOTE:</strong> The component is referred to as Assemble in the help. The package type is still CranPort.</p></td>
</tr>
<tr class="odd">
<td><p>DBMoto Download</p></td>
<td><p>Uses DBMoto® to download the data as a one-time operation.</p></td>
</tr>
<tr class="even">
<td><p>DBMoto Mirror</p></td>
<td><p>Uses DBMoto®’s method of keeping the target table synchronized with the source table.</p></td>
</tr>
<tr class="odd">
<td><p>Excel Import</p></td>
<td><p>Reads the data from an Excel file.</p></td>
</tr>
<tr class="even">
<td><p>IG Universal Connect</p></td>
<td><p>Uses a Boomi Process that executes against the IG Universal Connect data source. This package type is set by default for IG Universal Connect data sources and cannot be edited.</p></td>
</tr>
<tr class="odd">
<td><p>ManualCranPort</p></td>
<td><p>Uses a custom CranPort™ package created by the user.</p></td>
</tr>
<tr class="even">
<td><p>Manual Data Services</p></td>
<td><p>Uses a custom Data Services package created by the user.</p>
<p><strong>NOTE:</strong> The Data Services Job that is run with this package type must follow the naming conventions defined for Collect. Refer to <a href="Use_the_Manual_Data_Services_Package_Type.htm">Use the Manual Data Services Package Type</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>ManualSSIS</p></td>
<td><p>Uses a custom SSIS package created by the user.</p></td>
</tr>
<tr class="even">
<td><p>SAP Data Services</p></td>
<td><p>Uses the Data Services module of SAP. This is the recommended package type.</p>
<p><strong>NOTE:</strong> When using this package type, it is recommended that the Delete Target Table On Build check box be disabled in Collect on the <em><a href="../Page_Desc/Target_Sources_H_Collect.htm">Target Sources</a></em> page’s <em>Vertical</em> View on the Advanced tab. In this case, if the check box is enabled, dspCompose™<span style="font-weight: bold;"> will  delete every record in the target table</span> during the Final Finish process (during which data posted in the target ERP system by the request is downloaded to tables.)</p></td>
</tr>
<tr class="odd">
<td><p>SAP Data Services using RFC</p></td>
<td><p>Uses Remote Function Calls via Data Services to extract data from an SAP Application instance.</p></td>
</tr>
<tr class="even">
<td><p>SAP RFC</p></td>
<td><p>Uses Remote Function Calls from SAP. SAP provides this package, but BOARFC is recommended.</p></td>
</tr>
<tr class="odd">
<td><p>SAP Text</p></td>
<td><p>Uses Remote Function Calls  from SAP to download data only from the tables STXH and STXL with certain parameters that are defined in Collect.</p></td>
</tr>
<tr class="even">
<td><p>SSIS</p></td>
<td><p>Uses an SSIS package (Microsoft).</p></td>
</tr>
</tbody>
</table>
