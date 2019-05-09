+++
title = 'Register Tables to Source'
solution = 'Platform'
+++

# Register Tables to Source

Tables are registered to sources so that when a target refresh is
conducted, all active tables are pulled from the source and published to
the target. Tables can be individually added or added as a group through
the publish group feature.

Table names are the same for both source and target systems unless a
table rename option is enabled. Transparent tables use an ODBC
connection to download data. Pool tables use a RFC DLL to pull data from
SAP tables.

There are two ways to register tables to a source:

  - **[**Import a Group Table**](Import_Group_Tables)** – Used to
    import System Type tables delivered with Common. This method
    facilitates the process of registering tables by importing content
    delivered with Common into Collect.
  - **[Manually](Manually_Register_Tables_to_Source)** – Used if the
    source is not a System Type delivered with Common.

A user can also [Use the Manual Data Services Package
Type](Use_the_Manual_Data_Services_Package_Type).

Continue with [Encrypt Columns](Encrypt_Columns).
