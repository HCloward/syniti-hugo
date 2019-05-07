+++
title = 'Resolve Problem Connecting to the SAP GUI During Template Recording'
solution = 'Platform'
+++

# Resolve Problem Connecting to the SAP GUI During Template Recording

If an error message displays while recording a template (such as “There
was a problem connecting to the SAP GUI”), settings may need to be
configured in Internet Explorer.

<span style="font-weight: bold;">NOTE</span>: Internet Explorer is
required to record a BDC or GUI script.

To troubleshoot the issue:

  - Log in to SAP using the SAP GUI to ensure the connection works.
  - Confirm that the connection information for the SAP instance (Common
    \> Configuration .\> Data Source Registry \> Vertical View of the
    data source associated with the SAP Application Server) matches the
    SAP GUI Connection properties. The SAP GUI connection properties are
    available in the SAP GUI Logon client by right-clicking the
    connection name and selecting Properties.
  - Configure Internet Explorer security settings.

To configure settings in Internet Explorer:

1.  Select <span style="font-weight: bold;">Internet options</span> from
    the <span style="font-weight: bold;">Tools</span> menu.
2.  Click the <span style="font-weight: bold;">Security</span> tab.
3.  Click the <span style="font-weight: bold;">Trusted Sites</span>
    icon.
4.  Click the <span style="font-weight: bold;">Sites</span> button.
5.  Enter the URL for the DSP® in the
    <span style="font-weight: bold;">Add this website to the
    zone:</span> field.
6.  Click <span style="font-weight: bold;">Add</span>.
7.  Click <span style="font-weight: bold;">Close</span>.
8.  Click the <span style="font-weight: bold;">Custom Level. . .</span>
    button.
9.  Enable the option <span style="font-weight: bold;">Initialize and
    script ActiveX controls not marked as safe for scripting.</span>
10. Click <span style="font-weight: bold;">OK
    </span>**<span style="font-weight: normal;">to close the
    </span><span style="font-weight: normal;font-style: italic;">Security
    Settings – Trusted</span>**<span style="font-style: italic;"> Sites
    Zone</span> dialog box. .
11. Click <span style="font-weight: bold;">OK</span> to close the
    <span style="font-style: italic;">Internet Options</span> dialog
    box.
