# Plugin Functionality

The framework plugin API provides access to information about the
current user session, the page from which the plugin is called, as well
as several additional functions. These properties and functions can be
accessed by the IPluginService object created when the plugin class is
called. This object is referenced by typing Host.

The following are three commonly used classes:

  - **Host.Page. –** Access page properties and functions
  - **Host.Session –** Access session properties and functions
  - **Host.Environment –** Access the DSP environment properties and
    functions. Within the Host object there several useful functions:
      - **Host.WriteMessage –** Writes a message to the screen
      - **Host.Session.Translate –** Translates a string based on the
        current user’s login language
      - **Host.SystemAdministration.DecryptOrPass –** Decrypts an
        encrypted string. Set the encoding property to
        System.Text.Encoding.Unicode.
