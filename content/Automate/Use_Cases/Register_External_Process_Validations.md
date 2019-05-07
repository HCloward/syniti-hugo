+++
title = 'Register External Process Validations'
solution = 'Platform'
+++

# Register External Process Validations

An external process is a plugin. The DSP utilizes plugins to provide
capabilities that may be difficult or impossible to express using a
stored procedure, for example, to send a file over FTP or to read
encrypted column data. Before registering an external process
validation, create the plugin. Refer to [Plugins
Overview](../../Sys_Admin/Use_Cases/Plugins%20Overview.htm) in System
Administration help for more information.

To register external process validations in Automate:

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click the **Interfaces** icon for the desired interface to add an
    external process validation at the interface level.
    
    OR
    
    Click the **Events** icon for the desired interface.

3.  Click the **Validations** icon for the desired event to add an
    external process validation at the event level.

4.  Click **Add**.
    
    [View the field description for the Interface Validations
    page](../Page_Desc/Interface_Validations.htm)

5.  Enter a value in the **PRIORITY** field to indicate the order in
    which the interface’s external processes run.

6.  Select **ExternalProcess** from the **VALIDATION TYPE** list box.

7.  Select a purpose from the **VALIDATION PURPOSE** list box to
    determine why the validation is needed. Options are:
    
      - **Requirement –** Interface is not run if the view returns
        records
    
      - **Validation–** If the view returns a value, then the validation
        has failed.

8.  Select a value from the **VALIDATION WHEN** list box to define when
    the validation runs in relation to the event. Options are:
    
      - **Pre–** Validation runs before the event runs.
    
      - **Post –** Validation runs after the event runs. This option is
        typically used to determine if an event has run to completion.

9.  Select a disposition from the **DISPOSITION** list box. If the event
    fails the event validation rule, the disposition defines what
    happens next. Options are:
    
      - **Abort –** Unexpected condition. If the validation fails, the
        interface is turned off, and workflow emails are sent to the
        business and technical roles.
    
      - **Consider Complete–** Expected condition. The interface does
        not retry, the event is considered complete and the next event
        runs.
    
      - **Retry–** Expected condition. The interface retries this
        event/validation until there are no more event validation
        failures.

10. Click **Save**; the *Vertical* View displays.
    
    **NOTE:** The VALIDATION TYPE selected on the *Horizontal* View
    determines the configuration of the *Vertical* View.'
    
    [View the field description for the Interface Validations page’s
    Vertical
    View](../Page_Desc/Interface_Validations.htm#InterfaceValidationsV)

11. Click the **Validation Plugin** list box to select a registered
    plugin.

12. Enter a descriptive comment in the **Comment** field.

13. Click **Save**.
