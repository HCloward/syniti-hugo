+++
title = 'Create Packages'
solution = 'Platform'
+++

# Create Packages

To create a package:

1.  Click **Packages** in the *Navigation* pane.

2.  Click **Add**.
    
    [View field descriptions for the Packages Page](Packages_H.htm).

3.  Enter a name in **PACKAGE NAME** field.
    
    **NOTE:** The naming convention for packages is
    \#Database\#%\#Source\#%, for example
    dswBRAZIL.stKNA1\_QALegacyData\_Customer.imp for an import or
    dswBRAZIL.stKNA1\_QALegacyData\_Customer.exp for an export.

4.  Select a value from the **SOURCE DATA SOURCE ID** list box.
    
    **NOTE:** The **SOURCE DATA SOURCE ID** list box contains Data
    Sources registered in Common. They are arranged in database and file
    sections in the list. The type of data source selected in this box
    determines the options available in the SOURCE TYPE list box.

5.  Select a value from the **SOURCE TYPE** list box.
    
    **NOTE:** The options in the **SOURCE TYPE** list box vary depending
    on the type of data source selected in the **SOURCE DATA SOURCE ID**
    list box. If the source data source is a database, the options in
    the SOURCE TYPE list box are SQL or Table. For file path data
    sources, options are File Delimited, File Excel, File Start-End and
    File Width.

6.  Select a value from **TARGET DATA SOURCE ID** list box.
    
    **NOTE:** The **TARGET DATA SOURCE ID** list box contains Data
    Sources registered in Common. They are arranged in database and file
    sections in the list. The type of data source selected in this box
    determines the options available in the TARGET TYPE list box.

7.  Select a value from **TARGET TYPE** list box.
    
    **NOTE:** The options in the **TARGET TYPE** list box vary depending
    on the type of data source selected in the **TARGET DATA SOURCE ID**
    list box. If the source data source is a database, the options in
    the TARGET TYPE list box are SQL or Table. For file path data
    sources, options are File Delimited, File Excel, File Start-End and
    File Width.
    
    **NOTE:** The **S** column is checked when the Source connection has
    been tested. It’s tested when the record is saved. If the connection
    fails, there is no check mark.
    
    **NOTE:** The **T** column is checked when the Target connection has
    been tested. It’s tested when the record is saved. If it fails,
    there is no check mark.

8.  Click **Save**; the *Vertical* View displays.
    
    *[View the field descriptions for the Package 's page Vertical
    View](Packages_H.htm#Packages_V)*

9.  Complete the general and advanced properties tabs depending on the
    Source and Target Type.

10. Click **Save**.
    
    **NOTE:** The fields that display on the *Vertical* View differ
    according to the Source and Target Type. Each data source type has
    its own set of Advanced Properties.
