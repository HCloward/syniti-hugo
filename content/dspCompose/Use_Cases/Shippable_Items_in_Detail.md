# Shippable Items in Detail

The dspCompose™ Shippable Items are:

  -  **Org Units** - allow a package to be created with the specific
    contents of dspCompose™ ttOrgUnit table only

**NOTE**: Supporting List sources for populating OrgUnit values might
reside in a data source other than dspCompose™.  To determine where the
List Source resides for an OrgUnit, view the OrgUnit record in
dspCompose \> Configuration \> Org Units.  Determine the List Data
Source and the List Source.

  - If the List Source is a table and that table definition does not
    already exist in the target system, a table definition needs to be
    created from the source and imported to the target. Using SQL
    Management Studio or a similar tool, script a table definition.
     Then copy and paste that definition into a CTS Item of CranSoft –
    SQL Script. Build a CTS Archive that contains the script and export
    to the target system. Import the script to the target system to
    create the table definition in the target database.

  - Once the table definition has been created in the target system,
    create a CTS Build of Type CranSoft – Data.  Choose the CTS Item
    Keys where DataSourceID = List Data Source of the Org Unit and
    TableName = List Source.

  - **Roles**- allow a package to be created with the specific contents
    of ztRole only.

  - **Team**- allow a package to be created with a specific team and the
    templates contained in that team (see Template description below.)

  - **Template**- allow a package to be created with a specific template
    and its related dspCompose™ objects which are:
    
      - ttTemplateArchive
    
      - ttTemplateEventRule
    
      - ttTemplateExternalRequestScenario
    
      - ttTemplateObject
    
      - ttTemplateOrgUnit
    
      - ttTemplatePostMessageTable
    
      - ttTemplateRequestRetention
    
      - ttTemplateRole
    
      - ttTemplateRoleDependency
    
      - ttTemplateRoleDependencySelect
    
      - ttTemplateRoleEvent
    
      - ttTemplateRoleExcelColumnControl

**NOTE**: A CTSed template cannot be activated until all its components
(within dspCompose™ and other data sources) are available on the target
system.
