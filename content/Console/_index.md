+++
title = "Console Overview"
weight = 3
layout = "single"
solution = "Migration"
+++

# Console Overview

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

## Setup and Configuration for Console

To get started:

  - [Set Up Security for
    Console](../dspMigrate/Set_Up_Security_for_dspMigrate)
  - [Access Console](Config/Access_Console)
  - [Context, the Context bar, and
    Navigation](../dspMigrate/Context_Navigation)
  - [Set Parameters for Other
    Components](Config/Set_Parameters_for_Other_Components)
  - [Set up and Register the Object
    Database](Config/Set_up_and_Register_the_Object_Database)
  - [Configure Data Services
    Functionality](Config/Configure_Data_Services_Functionality)
  - [Set the Default Context for a
    User](../../Platform/Sys_Admin/Use_Cases/Set_the_Default_Context_for_a_User)
    (optional, performed by an Administrator)
