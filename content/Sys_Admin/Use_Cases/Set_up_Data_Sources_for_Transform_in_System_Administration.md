+++
title = 'Set up Data Sources for Transform in System Administration'
solution = 'Platform'
+++

# Set up Data Sources for Transform in System Administration

An Administrator must set up data sources in System Administration
before Transform can be used.

To set up a data source:

1.  Create the data source under **Admin \> Data Sources**.
    
    **NOTE:**For file data source types (Local File, Remote File (FTP),
    Remote File (HTTP) or Remote File (UNC)), create the folder on the
    server and modify the data source to include the folder path. To
    modify the data source with the folder path, navigate to the
    *Vertical* View of the *Data Sources* page and update the Path
    field.

2.  Verify System Views is enabled for the data source
    (<span style="font-weight: bold;">Admin \></span>**Data Sources \>
    Vertical View \> Deprecated Properties**) for non-file data source
    types.

3.  Validate the data source to create the System Views.

4.  Verify the System Views were created, such as dsw\* team databases,
    sdb\*, and the DSW database.
