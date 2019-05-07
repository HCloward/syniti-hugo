+++
title = 'Avoid Timeouts When Building a DBMoto® Target Connection'
solution = 'Platform'
+++

# Avoid Timeouts When Building a DBMoto® Target Connection

When building a target connection to DBMoto, each package built will
stop and start the Data Replicator Service in DBMoto automatically
(depending on a parameter setting in Common).

At a high level, to avoid the timeout and processing issues inherent
with multiple stops and starts:

1.  Disable the Start Replicator parameter setting in Common.
2.  Stop the DBMoto Data Replicator service manually.
3.  Build target connections in Collect.
4.  Start the DBMoto Data Replicator service manually.
5.  Enable the Start Replicator parameter setting in Common.

 

Step one: To disable the DBMoto setting in Common:

1.  Select **Configuration \> Modules \> Parameters – Collect** in the
    *Navigation* pane.

2.  Select the **DBMoto Settings** tab.

3.  Click **Edit**.
    
    [View the field descriptions for the Parameters – Collect page’s
    DBMoto Settings
    tab](../../Common/Page_Desc/Parameters_Collect.htm#DBMoto_Settings_Tab)

4.  Click the **Start Replicator** check box to disable it.
    
    **NOTE:** When this check box is disabled, the Data Replicator must
    be stopped and started manually.

5.  Click **Save**.

 

<span style="font-weight: bold;">Step two: Stop the DBMoto Data
Replicator service manually on the DBMoto server.</span> Stop the
service from the DBMoto Service Monitor icon in the Windows Notification
Area or from **Control Panel** \> **Administrative Tools** \>
**Services**.

**NOTE**: Only one Data Replicator service is used per DSP® instance.
When the service is stopped, it is stopped for all tables across all
targets.

 

<span style="font-weight: bold;">Step three: Build all target
connections in Collect.</span> Refer to [Register
Targets](Register_and_Use_Targets.htm#Register_Targets) for more
information.

 

**Step four: Start the DBMoto Data Replicator service manually on the
DBMoto server.** Start the service from the DBMoto Service Monitor icon
in the Windows Notification Area or from **Control Panel** \>
**Administrative Tools** \> **Services**.

 

Step five: To enable the DBMoto setting in Common:

1.  Select **Configuration \> Modules \> Parameters – Collect** in the
    *Navigation* pane.

2.  Select the **DBMoto Settings** tab.

3.  Click **Edit**.
    
    [View the field descriptions for the Parameters – Collect page’s
    DBMoto Settings
    tab](../../Common/Page_Desc/Parameters_Collect.htm#DBMoto_Settings_Tab)

4.  Click the **Start Replicator** check box to enable it.
    
    **NOTE:** When this check box is enabled, the Data Replicator is
    stopped and started automatically.

5.  Click **Save**.
