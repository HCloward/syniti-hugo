+++
title = 'Assign Keys to Security Role'
solution = 'Platform'
+++

# Assign Keys to Security Role

Once the role is created, keys are assigned to the role. Keys represent
values defined in the security definition to which users assigned to the
role will have access.

Certain components also require keys be added to security roles when
certain objects are added in the component. For example:

  - When using dspMigrate™, additional steps must be taken when a new
    context (Wave - Process Area etc.) is created. Add the keys for each
    new context to the appropriate dspMigrate™ security role.

  - When using Integrate, any new categories must be assigned as a key
    to the appropriate Integrate security role.

  - When using dspTrack™, any new projects or plans must be assigned as
    a key to the security role.

  - When using Common, establish User-Specific Security Definitions by
    adding the data source to be used in Common as a key to the Analyze
    DataSources description.
    
    **NOTE:**Once the keys are added, the data sources are listed on the
    <span style="font-style: italic;">Analyze</span> page in Common to
    be traced, profiled, or scanned for duplicate data.

  - When using Collect, assign keys to the Collect Targets security role
    definition where the key is the Target name.

To assign keys:

1.  From the *Security Roles* page, click **KEYS** button for NAME; all
    security definitions for the role displays.

2.  Click **Key** for DESCRIPTION.

3.  Click **Add**.
    
    [View the field descriptions for the Role Key Values
    page](../Page_Desc/Role_Key_Values)

4.  Select a key from **SECURITY DEFINITION KEY ID** list box.

5.  Click **Save**.
