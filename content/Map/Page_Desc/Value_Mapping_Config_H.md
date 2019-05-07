+++
title = 'Value Mapping (Config) H'
solution = 'Migration'
+++

## <span id="Value_Mapping__Config__H"></span>

# Value Mapping (Config) H

**[Value Mapping (Config) V](#Value_Mapping__Config__V)**

<div class="use">

Use this page to [Build a Remediation
Report](../Use_Cases/Build_a_Remediation_Report.htm).

</div>

To access this page:

1.  Click **dspMigrate** in the *Navigation* pane.
2.  Click **Map** in the Context bar.
3.  Select **Configuration \> Value Mapping (Config)** in *Navigation*
    pane.

|                              |                                                                                                                                                                                                           |
| ---------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                        | Description                                                                                                                                                                                               |
| Target Lookup Table (Config) | Click to open the *[Target Lookup Table](../../Design/Page_Desc/Target_Lookup_Table_H.htm)* page to update configuration for a check table as needed.                                                     |
| VALUE TABLE NAME             | Displays the name of the lookup table added in Target Design or imported with a System Type when it’s imported into Target Design.                                                                        |
| ACTIVE                       | If checked, the check table is active and can be used in value mapping.                                                                                                                                   |
| REMEDIATION VALUE            | Displays a remediation value used to complete mock loads only and never used in the Production environment.                                                                                               |
| VALUES PULLED ON             | Displays the date and time Target values were last retrieved from the Wave Target data source. Target values are retrieved when a user clicks Refresh on the Value Mapping (Config) page's Vertical View. |
| Sources                      | Click to open the [*Value Mapping (Sources)*](Value_Mapping_Sources_H.htm) page to view the number of Sources used in the check table.                                                                    |
| Values                       | Click to open the *[Check Table Values](Check_Table_Values.htm)* page to view the Target values that are mapped to the selected check table.                                                              |
| Refresh                      | Click to refresh Target values in the check table. The language to be refreshed is controlled at the Wave level (Console \> Wave \> Vertical View \> Language field).                                     |

## <span id="Value_Mapping__Config__V"></span>Value Mapping (Config) V

[Value Mapping (Config) H](#Value_Mapping__Config__H)

<div class="use">

Use this page to [Build a Remediation
Report](../Use_Cases/Build_a_Remediation_Report.htm) and [Designate a
System For a Check
Table.](../Use_Cases/Designate_a_System_for_Check_Table.htm)

</div>

Field

Description

Basic Settings

<span id="Lookup Table Type" class="popUpLink">Type</span>

Displays an option indicating whether fields in the check table should
be value mapped.

Active

If checked, the check table is active and can be used in value mapping.

Value Data Source ID

Displays the name of the data source used with this check table.

If the field is blank, the data source set at the Wave level on the
<span style="font-style: italic;">[Process Area:
Object](../../Console/Page_Desc/Process_Area_ObjectH.htm)</span> page’s
<span style="font-style: italic;">Vertical</span> View is used.

**NOTE:** If a data source displays in this field, it overwrites the
data source set at the Wave level.

**NOTE:** Refer to [Designate a System for a Check
Table](../Use_Cases/Designate_a_System_for_Check_Table.htm) for more
information.

Remediation Value

Displays a remediation value used to complete mock loads only and never
used in the Production environment.

Actions and Navigation

Sources

Click to open the [Source Check Table
(Config)](Source_Check_Table_Config_H.htm) page to view the number of
Sources used in the check table.

Values

Click to open the [Check Table Values](Check_Table_Values.htm) page to
view the Target values that are mapped to the selected check table.

Mappings

Click to open the *[Field Mappings](Field_Mappings_H.htm)* page to view
mappings for the value table.

Refresh

Click to refresh Target values in the check table. The language to be
refreshed is controlled at the Wave level (Console \> Wave \> Vertical
View \> Language field).

Value Table

Value Table Column1

Displays the first key field in a complex check table that has multipart
keys.

This value is entered in Target Design on the *Vertical* View of the
*[Target Lookup
Table](../../Design/Page_Desc/Target_Lookup_Table_H.htm)* page.

Value Table Column2

Displays the second key field in a complex check table that has
multipart keys.

This value is entered in Target Design on the *Vertical* View of the
*[Target Lookup
Table](../../Design/Page_Desc/Target_Lookup_Table_H.htm)* page.

Value Table Column3

Displays the third key field in a complex check table that has multipart
keys.

This value is entered in Target Design on the *Vertical* View of the
*[Target Lookup
Table](../../Design/Page_Desc/Target_Lookup_Table_H.htm)* page.

Value Table Column4

Displays the fourth key field in a complex check table that has
multipart keys.

This value is entered in Target Design on the Vertical View of the
*[Target Lookup
Table](../../Design/Page_Desc/Target_Lookup_Table_H.htm)* page.

Value Table Column5

Displays the fifth key field in a complex check table that has multipart
keys.

This value is entered in Target Design on the *Vertical* View of the
*[Target Lookup
Table](../../Design/Page_Desc/Target_Lookup_Table_H.htm)* page.

Value Table Client Column

Displays the name of the field that contains ERP system client
information.

This value is entered in Target Design on the *Vertical* View of the
*[Target Lookup
Table](../../Design/Page_Desc/Target_Lookup_Table_H.htm)* page.

Value Table Language Column

Displays the name of the field that contains the ERP system client
information.

This value is entered in Target Design on the Vertical View of the
*[Target Lookup
Table](../../Design/Page_Desc/Target_Lookup_Table_H.htm)* page.

Multi Value Field Lookup Table Value Column

Displays the column containing the value to use as the key field if more
than one value table column is set as a key field for the value table
(as in, there is data in the Value Field1 and Value Field2 fields)

This value is entered in Target Design on the Vertical View of the
*Target Lookup Table* page.

Description Value Table

Description Table Name

Displays the name of the table that stores the descriptions for the
values in the value table.

This value is entered in Target Design on the Vertical View of the
*[Target Lookup
Table](../../Design/Page_Desc/Target_Lookup_Table_H.htm)* page.

Description Table Column

Displays the name of the column that stores the descriptions for the
values in the value table.

This value is entered in Target Design on the Vertical View of the
*[Target Lookup
Table](../../Design/Page_Desc/Target_Lookup_Table_H.htm)* page.

Description Table Key Column

Displays the key column on the Description table used to uniquely
identify values if the Description table key is different from the Value
table's key column.

This field is used with the lookup table T006.

This value is entered in Target Design on the Vertical View of the
*[Target Lookup
Table](../../Design/Page_Desc/Target_Lookup_Table_H.htm)* page.

Description Table Client Column

Displays the column on the Description Table that stores the Client or
Tenant of the data. Used with SAP only.

Description Language Column

Displays the column on the Description Table that stores the language
identifier column. Used with SAP only.

Details

Description Update SQL

Displays SQL command used to update the Description Language Field.

Status

Values Pulled On

Displays the date and time Target values were last retrieved from the
Wave Target data source during a refresh.

Values Pulled By

Displays the user ID of the user who clicked Refresh on this page during
a refresh.
