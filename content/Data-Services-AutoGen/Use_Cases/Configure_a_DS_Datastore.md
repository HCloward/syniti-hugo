+++
title = 'Configure a Data Services Datastore'
solution = 'Migration'
+++

# Configure a Data Services Datastore

On the *Data Services Datastores Mappings* page, configure the Data
Services datastores to support auto-generation.

A Data Services Repository can be registered at the Process Area: Object
level or at the Process Area level (for example, the same Data Service
Repository can be assigned to different Process Area: Objects). The
level at which the repository is registered influences how Data Services
Projects are organized. In either case, Console is a required data
source, so a pair of datastores must be registered: one for Console and
one for the related dsw\* database.

To configure a Data Services datastore in AutoGen:

1.  Click the **Automation** tab in the Quick Panel.

2.  Select the Object for which the Data Services repository is being
    set up.

3.  Click the **Build and Refresh Data Services** icon in the Page
    toolbar; the *[AutoGen Data
    Services](../Page_Desc/AutoGen_Data_Services.htm)* page's *Vertical*
    View displays.

4.  Select **Configuration \> Data Services Datastores** in the AutoGen
    *Navigation* pane.

5.  Click **Add**; the *Data Services Datastores Mappings* page
    displays.
    
    **NOTE:** If no records exist, the page displays in add mode.
    
    [View the field descriptions for the Data Services Datastores
    Mappings page](../Page_Desc/Data_Services_Datastores_Mappings_H.htm)

6.  Select the data source ID from the **Data Source Id** list box.

7.  Select the data service repository ID from the **Data Services
    Repository ID** list box.

8.  Click **Save**.

To write the datastores into the data sources in Data Services, click
the **Update Data Services Datastore** icon.
