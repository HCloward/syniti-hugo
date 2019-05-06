# Setup and Configuration for Console

Before beginning work on a migration project, the hierarchical migration
structure must be set up in Console so it can be passed in to each
component. Waves, Process Areas and Objects must be added in Console,
which will pass them to the other dspMigrate™Advanced Data Migration
(ADM) components. For example, a Wave is registered once in Console, and
then passed to Map and Transform. Elements should also be deleted in
Console, but cannot be deleted if they are used in a migration project
in Map or Transform.

The structure contains the following elements set up in this order, the
wave and process area combination is referred to as a Contex:

  - Wave
  - Process Area
  - Object

To get started:

  - [Set Up Security for
    Console](../../dspMigrate/Set_Up_Security_for_dspMigrate.htm)
  - [Access Console](Access_Console.htm)
  - [Context, the Context bar, and
    Navigation](../../dspMigrate/Context_Navigation.htm)
  - [Set Parameters for Other
    Components](Set_Parameters_for_Other_Components.htm)
  - [Set up and Register the Object
    Database](Set_up_and_Register_the_Object_Database.htm)
  - [Register the Object Database in System
    Administration](../../../Platform/Sys_Admin/Use_Cases/Register_the_Object_Database_\(dsw_\)_in_System_Administration.htm)
  - [Configure Data Services
    Functionality](Configure_Data_Services_Functionality.htm)
  - [Set the Default Context for a
    User](../../../Platform/Sys_Admin/Use_Cases/Set_the_Default_Context_for_a_User.htm)
    (optional, performed by an Administrator)
