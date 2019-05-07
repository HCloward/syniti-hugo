+++
title = ''
solution = 'Platform'
+++

## Register the Object Database (dsw\*) in System Administration

<span style="font-weight: bold;">NOTE</span>: Databases should not be
added before consulting the on-site DBA or technical lead on the
project. Database and server settings and parameters play into the
creation of every database and if not set up correctly can lead to
severe performance issues.

To register the object database:

1.  Select <span style="font-weight: bold;">Admin \> Data Sources</span>
    in <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Data Sources
    page](../Page_Desc/Data_Sources_HSysAdmi.htm)

3.  Enter a name for the data source that contains the newly created
    database in <span style="font-weight: bold;">DATA SOURCE NAME</span>
    field.

4.  Select <span style="font-weight: bold;">SqlServer</span> from the
    <span style="font-weight: bold;">DATA SOURCE TYPE</span> list box.

5.  Click <span style="font-weight: bold;">Save</span>;
     <span style="font-style: italic;">Vertical</span> View displays.

6.  Enter the database’s server address in
    <span style="font-weight: bold;">Server Address</span> field.

7.  Enter the name of the database in the
    <span style="font-weight: bold;">Database</span> field.
    
    **NOTE:** This name begins with dsw.

8.  Enter SQL SERVER user id used to log in to CranSoft SQL SERVER
    Database in <span style="font-weight: bold;">User ID field</span>.
    (example: Cransoft)

9.  Enter SQL SERVER password used to log in to CranSoft SQL SERVER
    Database in <span style="font-weight: bold;">Password</span> field.
    (example: Cransoft)

10. Click <span style="font-weight: bold;">Advanced Properties</span>
    tab.

11. Click <span style="font-weight: bold;">System Views</span> check box
    to enable it.
    
    **NOTE**: This step creates BackOffice views that are used in list
    boxes within Transform. These views are required for the dsw\*
    Transform database.

12. Click <span style="font-weight: bold;">Save</span>.

13. Click <span style="font-weight: bold;">Back</span> button on browser
    to return to the <span style="font-style: italic;">Data
    Sources</span> page’s
    <span style="font-style: italic;">Horizontal</span> View.

14. Select the Data Source.

15. Click <span style="font-weight: bold;">Test Connection</span> on
    Page toolbar to test the connectivity to the data source.
