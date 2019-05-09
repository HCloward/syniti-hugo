+++
title = 'Configure Debug Logs Settings'
solution = 'Platform'
+++

# Configure Debug Logs Settings

The <span style="font-style: italic;">Debug Logs</span> page allows
users to configure debug logs at the application level.

To configure debug log settings:

1.  Select **Job Monitor \> Debug Logs** in *Navigation* pane.

2.  Click **Edit** for the component.
    
    [View the field descriptions for the Debug Logs
    page](../Page_Desc/Debug_Logs)

3.  Select a debugging level from <span style="font-weight: bold;">TRACE
    LEVEL</span> list box, which corresponds to the severity of the
    message logged. Values are:
    
      - **Disabled** – debugging is disabled
      - **Debug** – a detailed message displays to provide data about
        the process
      - **Information** – an information message displays to mark a
        landmark in the code
      - **Warning** – a message displays to inform the user that a
        problem could surface
      - **Error** – an error message displays while the process is
        executing; processing can continue
      - **Fatal** – an error message displays to indicate an error
        caused the processing to stop

4.  Enter a value in <span style="font-weight: bold;">RETENTION
    INTERVAL</span>  field to control the number of days data is
    retained in the debug log.

5.  Click **Save**.

**NOTE:** To help debug or locate a process causing an error, click
**Clear Debug Logs** to delete all debug logs for the application and
re-run the process to view only the debug log for that process.
