# View ISA Log

The Log displays information to trace that status of jobs as they
capture failed data, apply user filters to data, and generate reports to
use while debugging.

<span style="font-weight: bold;">NOTE</span>:<span> </span> For the ISA
Log to display information the Trace level must be set in **Information
Steward Accelerator \>**Configuration \> Parameters \> Basic Settings \>
Trace Level. The default Trace level is set to **Disabled**, so no
records are  written to the Log until the Trace level is set.

The Trace level
<span style="font-family: Arial, sans-serif;">corresponds to the
severity of the message logged.</span><span> </span>Values are:

<span style="font-weight: bold;">Disabled</span> – debugging is disabled

<span style="font-weight: bold;">Debug</span> – a detailed message
displays to provide data about the process

<span style="font-weight: bold;">Information</span> – an information
message displays to mark a landmark in the code

<span style="font-weight: bold;">Warning</span> – a message displays to
inform the user that a problem could surface

<span style="font-weight: bold;">Error</span> – an error message
displays while the process is executing; processing can continue

<span style="font-weight: bold;">Fatal</span> – an error message
displays to indicate an error caused the processing to stop

To view the Log, either select
**<span style="font-weight: normal;">Information Steward Accelerator
\></span>**Advanced \> Log from the *Navigation* pane, or select
**<span style="font-weight: normal;">Information Steward Accelerator
\></span>**Configuration \> Parameters \> Basic Settings \> Log.

**NOTE:** To help debug or locate a process causing an error, click
**Clear Logs** on the
<span style="font-style: italic;">[Log](../Page_Desc/Log_ISA.htm)</span>
page to delete all debug logs for the application and re-run the process
to view only the debug log for that process.
