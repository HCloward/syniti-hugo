# Test a BackOffice IGC Agent Connection in DSP

The BackOffice IGC Connector Agent’s connection status can be checked in
the DSP.

To test the Connector Agent’s Connection Status in DSP:

1.  Navigate to **Agent Interface \> Configuration \> APIs \> API Ping
    Agent** in the *Navigatio*n pane.
2.  Click the **Ping Agent** icon to test the connection.

**NOTE:** The Connector Agent runs as a Windows service, so you can
check to see if the service is still running as you would any other
Windows Service.

![](../../../Resources/Images/windowsService.png)

Once installed and connected to an IGC tenant, the Connector Agent
delivers dspMigrate metrics to the Migration Dashboard. However,
sometimes the connection may require troubleshooting. There are multiple
reasons the Agent’s connection may be interrupted, such as if the
Agent’s default Configuration Parameters were altered or the Agent’s
Windows service has stopped.
