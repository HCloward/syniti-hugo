# <span id="PluginsH"></span>Plugins H

[Plugins (V)](#PluginsV)

<div class="use">

Use this page to [Register the Plugin
Assembly](../Use_Cases/Register%20Plugin%20in%20DSP.htm#RegisterPluginAssembly).

</div>

To access this page:

1.  Select **Admin \> WebApps** in the *Navigation* pane.
2.  Click the **Plugins** icon for the desired WEBAPP NAME.
3.  Click the **Plugins** icon for the desired plugin ASSEMBLY.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PLUGIN NAME</p></td>
<td><p>Displays the unique identifier for the plugin.</p></td>
</tr>
<tr class="odd">
<td><p>PLUGIN TYPE</p></td>
<td><p>Displays the type of plugin. Options are:</p>
<ul>
<li><p><strong>Validation or Business Rule –</strong> Plugin most commonly used with validation or business rules</p></li>
<li><p><strong>List Data Provider –</strong> Plugin used to return list/combo box result values</p></li>
<li><p><strong>File Download Plugin –</strong> Plugin registered as a business rule and used for downloading a file</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a brief description of the plugin.</p></td>
</tr>
<tr class="odd">
<td><p>EVENT MODE</p></td>
<td><p>This field is not used.</p></td>
</tr>
<tr class="even">
<td><p>Business Rules</p></td>
<td><p>Click to open the <em><a href="Plugin%20Business%20Rules.htm">Plugin Business Rules</a></em> page to view all pages within the DSP where the plugin is registered as a business rule.</p>
<p>The count on the icon is the total number of pages in the DSP where the plugin is registered as a business rule.</p></td>
</tr>
<tr class="odd">
<td><p>Validation Rules</p></td>
<td><p>Click to open the <em><a href="Plugin%20Validation%20Rules.htm">Plugin Validation Rules</a></em> page to view all pages within the DSP where the plugin is registered as a validation rule.</p>
<p>The count on the icon is the total number of pages in the DSP where the plugin is registered as a validation rule.</p></td>
</tr>
<tr class="even">
<td><p>List Data Providers</p></td>
<td><p>Click to open the <em><a href="Plugin%20List%20Data%20Providers.htm">Plugin List Data Providers</a></em> page to view all pages within the DSP where the plugin is registered as a list data provider (as in, instances where a plugin is used to determine what is displayed in a list box on a DSP page).</p>
<p>The count on the icon is the total number of pages in the DSP where the plugin is registered as a list data provider.</p></td>
</tr>
</tbody>
</table>

 

## <span id="PluginsV"></span>Plugins V

[Plugins (H)](#PluginsH)

Field

Description

Plugin Name

Displays the unique identifier for the plugin.

Description

Displays a brief description of the plugin.

Basic Properties

Shared

If checked, the plugin can be referenced by other WebApps, not just the
WebApp to which the plugin is registered.

If unchecked, the plugin can only be referenced by the WebApp to which
the plugin is registered. It cannot be referenced by other WebApps.

Back End Authentication

If checked, back end authentication is enabled. The user is forced to
enter their Back End Authentication credentials via the DSP UI when the
plugin is executed.

If unchecked, back end authentication is disabled.

Requires Event Type

This field is not used.

Technical Information

Relative Assembly Path

Displays the plugin assembly name relative to the
UserArea\\\[WebAppID\]\\Processes folder, where UserArea is the DSP
folder on the application server where all assemblies are stored and
WebAppID is the GUID specific to the WebApp. If the DLL is in the
Processes folder, only the assembly name displays. If the DLL is in
another folder or a sub-folder, the assembly name and the path display.
For example, with an assembly called "myassembly.dll" located in the
Processes folder, the Relatively Assembly Path displays
"myassembly.dll." However, if that assembly was in a sub-folder called
"bin," the Relative Assembly Path displays "bin\\myassembly.dill."

Type Name

Displays the technical class type from the plugin.
