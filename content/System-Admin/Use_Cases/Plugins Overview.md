# Plugins Overview

The DSP® provides various ways of extending its capabilities with custom
business logic. This section describes how to develop plugins written
using Microsoft’s .NET framework and how to configure DSP to use them.
The plugin extension model is used to provide capabilities that may be
difficult or impossible to express using a stored procedure, for
example, to send a file over FTP or to read encrypted column data.

This section outlines the steps to create a plugin using C\# and Visual
Basic .Net. A basic level of development skills is assumed.

**NOTE:** Plugin development can be disruptive because it often requires
restarting IIS. If the DSP development instance is heavily used, it is
recommended to create a new DSP instance specifically for plugin
development.

## Terminology

One key aspect of working with the plugin application program interface
(API) is the proper use and understanding of development terminology:

  - **Plugin –** C\# or Visual Basic .Net code that is executed via a
    DSP® event. DSP plugins must be created using Microsoft’s .NET
    Framework.
  - **Plugin Assembly –** The deployment container of one or many
    plugins. In the case of the DSP plugins, a plugin assembly is a DLL
    created using a Microsoft .Net compiler (commonly Visual Studio). It
    is the plugin assembly that is registered in DSP.

## <span id="GettingStarted"></span>Getting Started

Every plugin requires the following prerequisites:

  - A reference to the CranBerry.Framework DLL
  - A public class that inherits the CranBerry.Framework.Plugins class
  - A method called OnExecute that overrides the OnExecute method of the
    CranBerry.Framework.Plugin class
  - PluginInstaller attributes
