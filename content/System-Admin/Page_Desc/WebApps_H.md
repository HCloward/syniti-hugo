# <span id="WebApps_H"></span>WebApps H

[WebApps V](#WebApps_V)

<div class="use">

Use this page to [Create a
WebApp](../../WebApp_Dev/Create_a_WebApp.htm).

</div>

To access this page, select **Admin \> WebApps** in
the *Navigation* pane.

|                |                                                                                    |
| -------------- | ---------------------------------------------------------------------------------- |
| Field          | Description                                                                        |
| WEB APP NAME   | Displays the name of the WebApp.                                                   |
| DATA SOURCE ID | Displays the name of the WebApp’s data source, a database.                         |
| Pages          | Click to open the *[Pages](Pages_H.htm)* page for the selected WEB APP NAME.       |
| Menus          | Click to open the *[Menus](Menus.htm)* page for the selected WEB APP NAME.         |
| Catalogs       | Click to open the *[Catalogs](Catalogs_H.htm)* page for the selected WEB APP NAME. |
| Groups         | Click to open the [Groups](Groups.htm) page for the selected WEB APP NAME.         |
| Plugins        | Click to open the *Plugins* page for the selected WEB APP NAME.                    |

## <span id="WebApps_V"></span>WebApps V

[WebApps H](#WebApps_H)

This page contains the following tabs:

  - [Web App Properties tab](#WebApp_V_Properties)
  - [Translation tab](#WebApp_V_Translation)
  - [Naming Options tab](#WebApp_V_Naming)
  - [Naming Conventions tab](#WebApp_V_Naming_Conventions)

## <span id="WebApp_V_Properties"></span>WebApp Properties tab

<div class="use">

Use this tab to view WebApp properties.

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Data Source ID</p></td>
<td><p>Displays the data source used by the WebApp.</p></td>
</tr>
<tr class="odd">
<td><p>Version</p></td>
<td><p>Displays the version number of the WebApp.</p></td>
</tr>
<tr class="even">
<td><p>Release Date</p></td>
<td><p>Displays the latest release date for the component.</p></td>
</tr>
<tr class="odd">
<td><p>Home Page ID</p></td>
<td><p>Displays the name of the page that displays when the user initially accesses the WebApp.</p></td>
</tr>
<tr class="even">
<td><p>Documentation Location</p></td>
<td><p>Displays the path where the help documentation is stored.</p>
<p><strong>NOTE:</strong> This field is not used for custom applications.</p></td>
</tr>
<tr class="odd">
<td><p>Web App Toolbar View</p></td>
<td><p>Displays the name of the SQL view for a toolbar if one is used on the page.</p></td>
</tr>
</tbody>
</table>

## <span id="WebApp_V_Translation"></span>Translation tab

Use this tab to enable page phrases tracking.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Track Page Phrases</p></td>
<td><p>If checked, a table in the DSP populates with phrases from the WebApp, such as column names and other translatable items. These are made available on the <em><a href="Catalog%20Page%20Phrases.htm">Catalog Page Phrases</a></em> page to help the application developer find and translate all the phrases for the application.</p>
<p>Using this feature helps build a catalog for your WebApp so you can ship it empty and/or translate it.</p>
<p><strong>NOTE:</strong> BackOffice recommends that this feature be disabled as it has a large impact on performance.</p></td>
</tr>
</tbody>
</table>

## <span id="WebApp_V_Naming"></span>Naming Options tab

Use this tab to [Enforce Strict
Naming](../../WebApp_Dev/Naming_Conventions_and_the_Enforce_Strict_Naming_Feature.htm).

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p><br />
Enforce Strict Naming</p></td>
<td><p>If enabled, the DSP® filters applicable list boxes based on the naming conventions listed on the Naming Conventions tab. For example, a WebApp has a page using the nwEmployee table. With Enforce Strict Naming enabled, all views registered to this page must contain the word Employee within the name of the view and with the proper naming convention prefix and suffix. For a <em>Horizontal</em> View, web is the prefix and Hor is the suffix. For a <em>Vertical</em> View, web is the prefix and Ver is the suffix.</p></td>
</tr>
<tr class="odd">
<td><p>Table Prefix Size</p></td>
<td><p>Displays the number of characters in the table name’s prefix for the WebApp for registration purposes. The prefix is not included as part of the table name for consideration with Enforce Strict Naming. For example, the tables in Northwind are prefixed with nw, xt or zt. The nw is ignored when filtering any views based for a page where the nwEmployee table is registered.</p>
<p>The default Table Prefix Size is 2.</p></td>
</tr>
<tr class="even">
<td><p>Date Format Pattern</p></td>
<td><p>Displays the date format used for a column when the user selects “Formatted Date” in the Format list box on the <em><a href="Page_Columns_H.htm">Page Columns</a></em> page <em>Vertical</em> View.</p></td>
</tr>
<tr class="odd">
<td><p>Time Format Pattern</p></td>
<td><p>Displays the time format used for a column when the user selects “Formatted Time” in the Format list box on the <em>Page Columns</em> page <em>Vertical</em> View.</p></td>
</tr>
</tbody>
</table>

## <span id="WebApp_V_Naming_Conventions"></span>Naming Conventions tab

Use this tab to update [Naming
Conventions](../../WebApp_Dev/Naming_Conventions_and_the_Enforce_Strict_Naming_Feature.htm).

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p><br />
Table Filter</p></td>
<td><p>Displays the filter applied in the table combo box when selecting a table. The default value is <strong>*</strong>, indicating there is no filter for a table name.</p></td>
</tr>
<tr class="odd">
<td><p>Horizontal Filter</p></td>
<td><p>Displays the filter used to reduce the number of elements shown in <em>Horizontal</em> View combo boxes. The default value is web*Hor, where the view name begins with “Web” and ends with “Hor.”</p>
<p><em>Horizontal</em> Views must be named in the database following this naming convention or they do not display as options in combo boxes in the DSP®.</p></td>
</tr>
<tr class="even">
<td><p>Vertical Filter</p></td>
<td><p>Displays the filter used to reduce the number of elements shown in <em>Vertical</em> View combo boxes. The default value is web*Ver, where the view name begins with “Web” and ends with “Ver.”</p>
<p><em>Vertical</em> Views must be named in the database following this naming convention or they do not display as options in combo boxes in the DSP®.</p></td>
</tr>
<tr class="odd">
<td><p>Report Filter</p></td>
<td><p>Displays the filter used to select views shown in <em>Report Page</em> Views. The default registered value is usr*, where the view name begins with “user” and the remaining text may be any character.</p>
<p>Report views must be named following this naming convention or they do not display in the DSP®.</p></td>
</tr>
<tr class="even">
<td><p>Chart Filter</p></td>
<td><p>Displays the filter used to select views shown in <em>Chart Page</em> Views. The default registered value is web*Chart.</p>
<p>Chart views must be named following this naming convention or they cannot be selected when creating a chart in the DSP®.</p>
<p>Refer to <a href="../../WebApp_Dev/Create_a_Chart.htm">Create a Chart</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Service Filter</p></td>
<td><p>Displays the filter used to select views for service pages. The default value is web*Ser, where the filter begins with &quot;web&quot; and ends with &quot;Ser.&quot;</p></td>
</tr>
<tr class="even">
<td><p>List Filter</p></td>
<td><p>Displays the filter used to reduce the number of elements shown in Value fields or the Descriptive fields when building a list box with Column Properties. The default value is web*List, where the view name begins with “Web” and ends with “List.”</p>
<p>Refer to <a href="../../WebApp_Dev/Add_List_Boxes_and_Combo_Boxes.htm">Add List Boxes and Combo Boxes</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Procedure Filter</p></td>
<td><p>Displays the filter used to help identify procedures. The default value is web*, where the filter name begins with “web&quot; and the remaining text may be any character. Due to the complexity in naming a procedure, only the prefix is defined.</p></td>
</tr>
<tr class="even">
<td><p>Validation Filter</p></td>
<td><p>Displays the filter used to reduce the number of elements shown in Validation combo boxes. The default value is web*Val, where the view name begins with “Web” and ends with “Val.”</p>
<p>Refer to <a href="../../WebApp_Dev/ValidationRules.htm">Register a Validation Rule to a Page</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Workflow Filter</p></td>
<td><p>Displays the filter used to reduce the number of elements shown in Workflow combo boxes. The default value is web*Flow, where the view name begins with “Web” and ends with “Flow.”</p>
<p>Refer to <a href="../Use_Cases/Register_Workflow_Views.htm">Register Workflow Views</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Event Parameter Filter</p></td>
<td><p>Displays the filter used to select views applicable to event parameters. The default value is web*Evt, where the filter begins with &quot;web&quot; and ends with &quot;Evt.&quot;</p></td>
</tr>
<tr class="odd">
<td><p>Defaults Filter</p></td>
<td><p>Displays the filter used to define the naming convention for <em>Default</em> Views, and is used to populate the Default View list box on the <em><a href="Pages_H.htm">Pages</a></em> page. The default value is web*Def, where the filter begins with &quot;web&quot; and ends with &quot;Def.&quot;</p></td>
</tr>
<tr class="even">
<td><p>User Control Filter</p></td>
<td><p>Displays the filter used to define the naming convention for <em>User Control</em> Views, and is used to populate the User Control View list box on the <em>Pages</em> page in System Administration (on the Vertical View &gt; Control Views tab, where the Page Type is &quot;Dynamic&quot;). The default value is web*Ucv, where the filter begins with &quot;web&quot; and ends with &quot;Ucv.&quot;</p>
<p>Refer to <a href="../../WebApp_Dev/User_Control_Views.htm">User Control Views</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Page Control Filter</p></td>
<td><p>Displays the filter used to define the naming convention for <em>Page Control</em> Views, and is used to populate the Page Control View list box on the <em>Pages</em> page in System Administration (on the Vertical View &gt; Control Views tab, where the Page Type is &quot;Dynamic&quot;). The default value is web*Pcv, where the filter begins with &quot;web&quot; and ends with &quot;Pcv.&quot;</p>
<p>Refer to <a href="../../WebApp_Dev/Page_Control_View.htm">Page Control Views</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Data Control Filter</p></td>
<td><p>Displays the filter used to define the naming convention for <em>Data Control</em> Views, and is used to populate the Data Control View list box on the <em>Pages</em> page in System Administration (on the Vertical View &gt; Control Views tab, where the Page Type is &quot;Dynamic&quot;). The default value is web*Dcv, where the filter begins with &quot;web&quot; and ends with &quot;Dcv.&quot;</p>
<p>Refer to <a href="../../WebApp_Dev/Data_Control_Views.htm">Data Control Views</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>List Control Filter</p></td>
<td><p>Displays the filter used when selecting <em>List Control</em> Views. The default value is web*Lcv, where the filter begins with &quot;web&quot; and ends with &quot;Lcv.&quot;</p></td>
</tr>
<tr class="even">
<td><p>Parameter Filter</p></td>
<td><p>Displays the filter used when selecting <em>Page Parameter</em> Views. The default value is web*PV, where the filter begins with &quot;web&quot; and ends with &quot;PV.&quot;</p></td>
</tr>
<tr class="odd">
<td><p>Toolbar Filter</p></td>
<td><p>Displays the filter used when selecting <em>Toolbar</em> Views. The default value is web*Tbv, where the filter begins with &quot;web&quot; and ends with &quot;Tbv.&quot;</p></td>
</tr>
<tr class="even">
<td><p>Tooltip Filter</p></td>
<td><p>Displays the filter used when using the tooltip feature.</p>
<p>Refer to <a href="../../WebApp_Dev/Add_a_Tooltip.htm">Add a Tooltip</a> for more information.</p>
<p><strong>NOTE:</strong> This field is hard coded to limit the number of characters displayed to 32.</p></td>
</tr>
<tr class="odd">
<td><p>Watermark Filter</p></td>
<td><p>Displays the filter used when using the watermark feature.</p>
<p>Refer to <a href="../../WebApp_Dev/Add_a_Watermark.htm">Add a Watermark</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Control View Field Prefix</p></td>
<td><p><em>Field is deprecated.</em></p></td>
</tr>
</tbody>
</table>
