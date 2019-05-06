# Make Changes to a Plugin

Changes may need to be made to the plugin. Once the assembly has been
created, verify plugins were created. If plugins are missing:

  - Check the assembly to be sure the Plugin Installer attributes were
    sent and that the plugin classes are Public.

  - Ensure the correct DLL file is referenced in the Relative Assembly
    Path.
    
    **NOTE:** The Relative Assembly Path displays the plugin assembly
    name relative to the UserArea\\\[WebAppID\]\\Processes folder, where
    UserArea is the DSP folder on the application server where all
    assemblies are stored and WebAppID is the GUID specific to the
    WebApp. If the DLL is in the Processes folder, only the assembly
    name displays. If the DLL is in another folder or a sub-folder, the
    assembly name and the path display. For example, with an assembly
    called "myassembly.dll" located in the Processes folder, the
    Relatively Assembly Path displays "myassembly.dll." However, if that
    assembly was in a sub-folder called "bin," the Relative Assembly
    Path displays "bin\\myassembly.dill."

To make changes to the plugin:

1.  Copy the new file to the User Area folder.

2.  Log in to the DSP.

3.  Select **Admin \> WebApps** in the *Navigation* pane.

4.  Click the **Plugins** icon for the desired WEBAPP NAME.

5.  Click **Vertical View** for the ASSEMBLY.

6.  Click **Repair**.
    
    **NOTE:** Once the assembly has been repaired, one or more events
    may still reference the missing plugins. The framework looks at the
    DLL (assembly) again and check for any new plugins or changes to the
    existing plugins.
