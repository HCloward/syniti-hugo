# Add a Debug Log to a Custom WebApp

Debug logs display information, such as error messages and the date and
time errors occurred to assist in troubleshooting issues with a
component. The DSP® is installed with debug logs for delivered
applications.

After a custom WebApp has been added to the platform, a user can add a
debug log to it.

After the log has been added, the platform creates:

  - Table:  ttDebugLog
  - Page:  Debug Log
  - Views:
      - webTraceLevelSel
      - webDebugLogHor
      - webDebugLogVer

To view the debug log from within the custom WebApp, the user must add
the debug log as a page to the custom WebApp. The log can also be viewed
in the table ttDebugLog.

To add a debug log:

1.  Select <span style="font-weight: bold;">Common \> Job Monitor \>
    Debug Logs</span> in
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Add</span>.
    
    <span style="font-style: italic;">[View the field descriptions for
    the Debug Logs page.](../Page_Desc/Debug_Logs.htm)</span>

3.  Select the name of the custom WebApp from the
    <span style="font-weight: bold;">COMPONENT</span> list box.
    
    **NOTE:** A component can have only one debug log.

4.  Select an option in the <span style="font-weight: bold;">TRACE
    LEVEL</span> list box to designate the type of messages to be
    displayed in the debug log. :
    
    Options are:
    
      - **Disabled** – Debugging is disabled.:
      - **Debug** – dAll logs returned during execution of the process
        display on the debug log. :
      - **Information** – Only Information messages display on the debug
        log.
      - **Warning** – Warning, Error and Fatal messages display on the
        debug log.
      - **Error** – Error and Fatal messages display on the debug log.
      - **Fatal** – Fatal messages display on the debug log.

<!-- end list -->

1.  Enter a value in <span style="font-weight: bold;">RETENTION
    INTERVAL</span> field to control the number of days data is retained
    in the debug log. After the number of days has passed, the data is
    deleted.
    
    To clear all logs regardless of the retention interval, click the
    Clear Debug Log icon in the Page toolbar. This icon is not active if
    the Trace Level for a component is Disabled.

2.  Click <span style="font-weight: bold;">Save</span>.
