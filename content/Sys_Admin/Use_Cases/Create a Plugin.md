+++
title = 'Create a Plugin'
solution = 'Platform'
+++

# Create a Plugin

There are five basic steps to create a plugin:

1.  [Add a reference to the plugin API](#AddAReferenceToThePluginAPI)
2.  [Define the Plugin](#DefineThePlugin)
3.  [Configure the DSP for Data Binding](#ConfigureDSPPageForDataBindng)
4.  [Add the Data Binding Helper
    Property](#AddTheDataBindingHelperProperty)
5.  [Add the PluginInstaller
Attribute](#AddThePluginInstallerAttribute)

## <span id="AddAReferenceToThePluginAPI"></span>Add a Reference to the Plugin API

Before the plugin can be utilized by DSP, reference the
CranBerry.Framework DLL in the Visual Studio solution.

### C\# Example

The following are the recommended C\# references to include in the
project:

![](../../../Resources/Images/Create%20a%20Plugin.png)

### Visual Basic .Net Example

The following are the recommended Visual Basic .Net references to
include in the project:

![](../../../Resources/Images/Create%20a%20Plugin_1.png)

## <span id="DefineThePlugin"></span>Define the Plugin

A plugin is a public class that inherits from the
Cranberry.Framework.Plugins class. This plugin class must override the
OnExecute method of the CranBerry.Framework.plugins class. The OnExecute
method runs when a DSP page executes a plugin.

### C\# Example

Use the following C\# code to define the plugin.

![](../../../Resources/Images/Create%20a%20Plugin_2.png)

### Visual Basic. Net Example

Use the following Visual Basic .Net code to define the
plugin.

![](../../../Resources/Images/Create%20a%20Plugin_3.png)

## <span id="ConfigureDSPPageForDataBindng"></span>Configure DSP® Page for Data Binding

In order to read data from a DSP page, the plugin must have a subclass
that inherits from the Cranberry.Framework.Plugins.DataRowContract
class.

**NOTE:** It is strongly recommended that the public properties of this
subclass match the column names on the page exactly for the columns
where data is passed to the plugin. This process sets up the ability to
retrieve data from the DSP page.

Verify the page which the plugin is linked to has columns that match the
public properties.

### C\# Example

In this example, the MyDataRowContract subclass inherits the
DataRowContract class. This subclass has a public property called
RequestID that matches a column name on a page in DSP.

Use the following C\# example to configure DSP® page(s) for data
binding.

![](../../../Resources/Images/Create%20a%20Plugin_4.png)

### Visual Basic .Net Example

In this example, the MyDataRowContract subclass inherits the
DataRowContract class. This subclass has a public property called
RequestID that matches a column name on a page in DSP.

Use the following Visual Basic .Net example to configure DSP® page(s)
for
data-binding.

![](../../../Resources/Images/Create%20a%20Plugin_5.png)

## <span id="AddTheDataBindingHelperProperty"></span>Add the Data Binding Helper Property

While it is possible to cast the contract everywhere it is used, in
practice, it is easier to define a helper property that performs that
cast.

In order to read the data from a page, a plugin uses the public
properties of the created subclass. The following examples use the
return of the DataRowContract object populated with information from the
DSP.

### C\# Example

Use the following C\# example to add the data binding helper property.
Note that the call to get the RequestID value from the DataRowContract
subclass uses the function.

![](../../../Resources/Images/Create%20a%20Plugin_6.png)

![](../../../Resources/Images/Create%20a%20Plugin_10.png)

### Visual Basic .Net Example

Use the following Visual Basic .Net example to add the data binding
helper property. Note that the call to get the RequestID value from the
DataRowContract subclass uses the
function.

![](../../../Resources/Images/Create%20a%20Plugin_7.png)

![](../../../Resources/Images/Create%20a%20Plugin_1.jpg)

## <span id="AddThePluginInstallerAttribute"></span>Add the PluginInstaller Attribute

The attributes described in this topic are only used during the
installation of a plugin assembly.

When installing a plugin assembly, DSP expects well-formed plugins to
provide a PluginInstaller attribute that includes various metadata about
how DSP is expected to run the plugin.

### C\# Example

Add the following attributes directly before the class definition of the
plugin class.

![](../../../Resources/Images/Create%20a%20Plugin_8.png)

### Visual Basic .Net Example

Add the following attributes directly before the class definition of the
plugin class.

![](../../../Resources/Images/Create%20a%20Plugin_9.png)
