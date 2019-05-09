+++
title = 'Add Logging Modules'
solution = 'Platform'
+++

# Add Logging Modules

Logging modules are used to display lower severity log records on the
*[Log](../Page_Desc/Log)* page than what is dictated by the Storage
Level on the *[Parameters](../Page_Desc/Parameters)* page.

An Administrator can create a module (or category) of logs that displays
information based on what types of errors are logged. The hierarchy is
based on the severity level. For example, if the ABC module logs errors
with the severity 20-Trace, it also logs everything with a priority
above 20.

For instance, if the Storage Level is set to 70 – Error, add a logging
module, set it to 30 – SQL the module displays severity types ranging
from 30 – SQL to 80 – Fatal.

To add a Logging Module in Automate:

1.  Select **Configuration \> Parameters** in the *Navigation* pane.

2.  Click the **Modules** icon.

3.  Click **Add**.
    
    [View the field description for the Logging Modules
    page](../Page_Desc/Logging_Modules)

4.  Enter a category name in the **MODULE** field.

5.  Select a priority from the **SEVERITY** list box.

6.  Click **Save**.
