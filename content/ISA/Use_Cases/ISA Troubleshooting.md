# ISA Troubleshooting

This section contains the following topics:

  - [Confirm the Data Services Connection URL if the Test Connection
    Fails](#Confirm_the_Data_Services_Connection_URL_if_the_Test_Connection_Fails)
  - [Troubleshoot Project not displaying on the *Project Summary*
    page.](#Troubleshoot_Project_not_displaying_on_the_Project_Summary_page)

## <span id="Confirm_the_Data_Services_Connection_URL_if_the_Test_Connection_Fails"></span>Confirm the Data Services Connection URL if the Test Connection Fails

The URL for the Data Services server must be set correctly in Common or
the connection will fail.

To confirm the URL in Common:

1.  Click <span style="font-weight: bold;">Common
    \></span>**Configuration \> Data Source Registry** in the
    *Navigation* pane.
2.  Click **Vertical View** for the ISA repository.
3.  Confirm the URL in the **Web Services URL** field is correct and
    uses an IP address for the server where Data Services is installed.

**NOTE**: The path should contain the IP address of the server. For
example, a valid path should look like
http://192.168.90.86:8080/DataServices/servlet/webservices?ver=2.1. If
the path begins with C://Program Files(x86), it is not
valid.

## <span id="Troubleshoot_Project_not_displaying_on_the_Project_Summary_page"></span>Troubleshoot Project not displaying on the *Project Summary* page

If a project does not display on the *[Project
Summary](../Page_Desc/Project_Summary_H)* page in the ISA, refresh
the tables in the dgRepository\_IS database in Collect.

To refresh the tables in Collect:

1.  Select <span style="font-weight: bold;">Collect \></span>**Targets**
    in the *Navigation* pane.
2.  Select the dgRepository\_IS target.
3.  Click **Refresh** in the Page toolbar.

After the tables are successfully downloaded, the project displays on
the *Project Summary* page in the ISA.
