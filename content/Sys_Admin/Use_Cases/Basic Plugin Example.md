+++
title = 'Basic Plugin Example'
solution = 'Platform'
+++

# Basic Plugin Example

With the four prerequisites listed in [Getting
Started](Plugins%20Overview#GettingStarted) satisfied, a basic
plugin can be created to display the message “Hello, World\!” to the
user. The following is an example of a basic plugin that shows a class
named HelloWorldPlugin that inherits from the Plugin class. This Plugin
class is accessed via the inclusion of the CranBerry.Framework.Plugins
class.

In the example, the HelloWorldPlugin class has one method called
OnExecute. This method overrides the OnExecute method of the
CranBerry.Framework.Plugins class. In the OnExecute method, a message is
logged to the DSP log tables and the message “Hello, World\!” displays
to the user. Finally, the HelloWorldPlugin class has a PluginInstaller
attribute set, thereby making it visible to DSP.

Beyond the required assemblies previously mentioned, there are many
other features that can be implemented in a plugin. The assemblies and
steps necessary to create a plugin that takes data from a DSP page and
reads and writes to the database is outlined in the [Advanced Plugin
Example](Advanced%20Plugin%20Example) section.

### C\# Example

The following is an example of a basic plugin in C\#.:

![](../../../Resources/Images/Basic%20Plugin%20Example.png)

### Visual Basic.Net Example

The following is an example of a basic plugin in Visual Basic .Net:

![](../../../Resources/Images/Basic%20Plugin%20Example_1.png)
