+++
title = 'Register a Data Source in Common'
solution = 'Platform'
+++

# Register a Data Source in Common

While data sources can be registered by an Administrator in System
Administration, registering a data source in Common is the preferred
method.

When a data source is registered in System Administration, it is
available in Common on the <span style="font-style: italic;">Data Source
Registry</span> page.  

However, after the initial record is added to Common, changes made to
data sources in System Administration are not applied to data sources in
Common. Changes made to data sources in Common are reflected in data
sources in System Administration.  

Refer to [Sync Data Sources in Common and System
Administration](Sync_Data_Sources_in_Common_and_System_Administration)
for more information.

<span style="font-weight: bold;">NOTE</span>: Data Services data sources
must be registered in Common.

The following Application Data Source Types can be registered:

  - Data Services Repository
  - External System Connection
  - IG Universal Connect
  - Local Utility Database
  - Migration Object Database
  - Migration Source Database
  - SAP Application Server
  - Target System Database

The general process for registering a data source is outlined below.
Configuration settings specific to Application Data Source Types are
described in the field description for the *[Data Source
Registry](../Page_Desc/Data_Source_Registry_H#Data_Source_Registry_V)*
page’s *Vertical* View.

To register a data source in Common:

1.  Select **Configuration \> Data Source Registry** in the *Navigation*
    pane.

2.  Click **Add**.
    
    *<span style="color: #0000ff;">[View the field descriptions for the
    Data Source Registry
    page](../Page_Desc/Data_Source_Registry_H)</span>*

3.  Enter the data source name in the **DATA SOURCE NAME** field.

4.  Select an option from the **APPLICATION DATA SOURCE TYPE** list box.
    
    **NOTE:** The application data source type can be a database,
    external system connection, or a Data Services repository.

5.  Click **Save**; the *Vertical View* displays.

6.  Enter data on the General and Advanced Settings tab as needed.
    
    **NOTE:** The fields that display on the
    <span style="font-weight: bold;">Vertical View</span> of the *Data
    Source Registry* page depend on the Application Data Source Type
    selected. View the field descriptions for the
    [<span style="font-style: italic;">Data Source
    Registry</span>](../Page_Desc/Data_Source_Registry_H#Data_Source_Registry_V)
    page’s
    [<span style="font-style: italic;">Vertical</span>](../Page_Desc/Data_Source_Registry_H#Data_Source_Registry_V)
    View for information about the fields available for each Application
    Data Source Type.
    
    **NOTE:** Configure settings on the Advanced Settings tab for data
    sources with an Application Data Source Type of External System
    Connection and a Data Source Type of OleDb or ODBC.

7.  Click **Save**.

8.  Click the Test Connection icon on the Page toolbar to confirm the
    data source settings are correct.
    
    **NOTE:** When a Data Services data source is added in the
    DataSourceRegistry, Process Adapters are automatically added for
    that data source in <span style="font-weight: bold;">Common \>
    Configuration \> Process Adapters</span>.
