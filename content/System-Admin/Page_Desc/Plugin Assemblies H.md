+++
title = 'Plugin Assemblies H'
solution = 'Platform'
+++

# Plugin Assemblies H

[Plugin Assemblies (V)](#PluginAssembliesV)

<div class="use">

Use this page to [Register the Plugin
Assembly](../Use_Cases/Register%20Plugin%20in%20DSP.htm#RegisterPluginAssembly).

</div>

To access this page:

1.  Select **Admin \> WebApps** in the *Navigation* pane.
2.  Click the **Plugins** icon for the desired WEBAPP NAME.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>RELATIVE ASSEMBLY PATH</p></td>
<td><p>Displays the plugin assembly name relative to the UserArea\[WebAppID]\Processes folder, where UserArea is the DSP folder on the application server where all assemblies are stored and WebAppID is the GUID specific to the WebApp. If the DLL is in the Processes folder, only the assembly name displays. If the DLL is in another folder or a sub-folder, the assembly name and the path display. For example, with an assembly called &quot;myassembly.dll&quot; located in the Processes folder, the Relatively Assembly Path displays &quot;myassembly.dll.&quot; However, if that assembly was in a sub-folder called &quot;bin,&quot; the Relative Assembly Path displays &quot;bin\myassembly.dill.&quot;</p></td>
</tr>
<tr class="odd">
<td><p>ASSEMBLY PRODUCT</p></td>
<td><p>Displays product information for the assembly.</p></td>
</tr>
<tr class="even">
<td><p>ASSEMBLY TITLE</p></td>
<td><p>Displays the name of the container for one or many plugins.</p></td>
</tr>
<tr class="odd">
<td><p>ASSEMBLY VERSION</p></td>
<td><p>Displays the version number of the assembly.</p></td>
</tr>
<tr class="even">
<td><p>ASSEMBLY COMPANY</p></td>
<td><p>Displays the company name.</p></td>
</tr>
<tr class="odd">
<td><p>Plugins</p></td>
<td><p>Click to open the Plugins page to configure plugins for the assembly and to view where in the DSP plugins are registered.</p>
<p>The count on the icon is the total number of plugins in the assembly.</p></td>
</tr>
</tbody>
</table>

 

## <span id="PluginAssembliesV"></span>Plugin Assemblies (V)

[Plugin Assemblies (H)](#PluginAssembliesH)

<div class="use">

Use this page to [Make Changes to a
Plugin](../Use_Cases/Make%20Changes%20to%20a%20Plugin.htm).

</div>

Field

Description

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

Assembly Information

Assembly Product

Displays product information for the assembly.

Assembly Title

Displays the name of the container for one or many plugins.

Assembly Description

Displays a description of the assembly.

Assembly Version

Displays the version number of the assembly.

Assembly Culture

Displays the culture that the assembly supports.

Assembly Configuration

Displays the configuration of the assembly; for example, Retail.

Assembly Company

Displays the company name.

Public Key Token

Displays the token that references the public key.

Hosting Environment

Hosting Mode

Displays the hosting state of the plugin.

Options are:

  - **InProc –** Indicates the plugin is hosted within the current
    process.
  - **InProcCompatible –** Indicates the plugin is a legacy style
    written in an early version of CranSoft.

Cran Soft Permission Set

This field is not used.

Windows Permission Set

This field is not used.

Actions

Update Assembly

Click to repair the assembly. Once it has been repaired, one or more
events may still reference the missing plugins. The framework looks at
the DLL (assembly) again and checks for any new plugins or changes to
the existing plugins.
