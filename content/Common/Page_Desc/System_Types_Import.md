# System Types Import

<div class="use">

Use this page to:

  - [Import a Data Source](../Use_Cases/Import_a_Data_Source.htm).
  - [Import a Model](../Use_Cases/Import%20a%20Model.htm)
  - [Export Translations to a
    Catalog](../Use_Cases/Export_Translations_to_a_Catalog.htm)

</div>

To access this page:

1.  Select<span style="font-weight: bold;">Common \> System Types</span>
    in the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Vertical View</span> icon
    for a System Type.
3.  Click <span style="font-weight: bold;">Import from Data Source or
    Model</span>.

Field

Description

Model

Click the *[System Types Models](System_Types_Models_H.htm)* page to
document in which tables must be populated when building the System
Type. Refer to [Manage System Types With System Type
Models](../Use_Cases/Manage_System_Types_with_System_Type_Models.htm)
for more information.

Data Source

Data Source ID

Displays name of data source being imported into the System Type.

**NOTE:** The data source selected must be a database on the local SQL
server (as in, a dg\* or sdb\* data source).

Import

Click to import the data source.

Model

System Type Model

Displays the name of the System Type Model to be used. JDE and SAP
System Type Models are pre-delivered with the product.

Language ID

Displays the language to pull for the Table Description and Field
Description views. It also determines the Language ID to export to the
Catalog.

**NOTE:** If a Language ID is not set, the default language defined in
the platform is used.

Import Model Option

Displays the location to use to import the System Type. Values are:

  - Import tables from the Selected Model
  - Import tables from the Selected Model Group

**NOTE:** If this option is selected the **Import Model Group** field is
required.

Import Model Group

Displays the name of the model group to use to import the System Type.

**NOTE:** All tables in the model group along with their associated
description and lookup tables are imported when the model is imported.

Exclude Client Fields

If checked, the SAP client fields are not imported. If unchecked, the
fields are imported.

**NOTE:** This field only applies to SAP System Types.

Import Model

Click to import the System Type Model.

Catalog Update

Catalog ID

Displays the name of the catalog to which registrations from
translations from the System Type are exported.

Refer to [Export Translations to a
Catalog](../Use_Cases/Export_Translations_to_a_Catalog.htm) for more
information.

Export

Click to export translation registrations in the selected System Type to
the catalog ID.

Refer to [Export Translations to a
Catalog](../Use_Cases/Export_Translations_to_a_Catalog.htm) for more
information.

**NOTE**: This can result in a large number of records being imported
into the catalog. Use caution when using this feature.
