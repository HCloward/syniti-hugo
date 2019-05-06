# Parameters

<div class="use">

Use this page to [Set Parameters for Other
Components](../Config/Set_Parameters_for_Other_Components.htm)

</div>

This page has the following tabs:

  - [General tab](#General_Tab1)
  - [Map tab](#Map_Tab)
  - [Transform tab](#Transform_Tab)
  - [Construct tab](#Construct_Tab)
  - [Compare Settings tab](#Compare_Settings_Tab)

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane, or select
    <span style="font-weight: bold;">Console</span> in the Context bar.
2.  Select <span style="font-weight: bold;">Advanced Configuration \>
    Parameters</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

## <span id="General_Tab1"></span>General tab

Field

Description

Application Information

Application Name

Displays the name of the component, Console.

Version

*Displays current version of Console.*

Date

Displays date when this version of Console Was released.

Common Options

Migration Source Database Filter

Displays the filter Console uses when displaying options in the **SOURCE
ID** list box on the
*[Source](../../../Platform/Collect/Use_Cases/Register_and_Use_Sources.htm)*
page’s *Horizontal* View and *Vertical* Views. This filter selects the
Source data source as a database that begins with **sdb**.

Migration Object Database Filter

Displays the filter Console uses when displaying options in the
**DATASOURCE ID** list box on the *Process Area: Object* page’s
*Horizontal* View. The default value is dsw% used by Transform
databases.

Email From

Displays the email address from which dspMigrate™ Advanced Data
Migration (ADM) will send workflow emails.

##  <span id="Map_Tab"></span>Map tab

<span style="font-weight: bold;">NOTE</span>: Fields on this page that
are not described in the table below are not used in the product.

Field

Description

Field Options

Key Prefix

Displays the prefix added to a Source key field during the Transform
automation process. These key fields are used to track legacy Source
keys during the migration process to the new key value (often generated
by the new ERP system). The default is zLegacy.

Xref Prefix

Displays the prefix added to a cross reference field during the
Transform automation process. When using a cross reference rule (on the
*[Field Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)* page in Map
by selecting Xref or RuleXref in the **ACTION** list box) that requires
additional or multiple rules to determine a value, Map creates a
**zField** and a **zLegacy** field on the source table used in
Transform. The **zLegacy** is used to complete client data conversions
and the **zField** is used to complete the value mapping Source to
Target check table values. The default is zLegacy.

Xref Source Field Default Status

Displays the default value mapping status for a cross reference Source
field for
<span style="font-family: &#39;Arial CE&#39;, sans-serif;">value
mapping. When the a field mapping’s Action is set to Xref , the Source
field on the *Value Mapping* page will default to this selection</span>

Auto Set Not Used For Multiple Sources

Displays the option that controls how Map updates the ACTION column for
Add Row and Update Row source mappings when the action has not been set
(i.e., the ACTION column is blank). The ACTION column displays on the
*Field Mappings* page in Map.

Options include:

  - <span style="font-weight: bold;">None -</span> The values in the
    ACTION column for the Add Row and Update Row Sources are not changed
    in other Sources.
  - <span style="font-weight: bold;">Primary and Secondary Source
    -</span> When a mapping is saved in a Add Row and Update Row Source,
    Map updates the ACTION column for actions that are not set with
    NotUsed.
  - <span style="font-family: Arial, sans-serif;color: #333333;font-weight: bold;">Secondary
    Source only -</span> When a mapping is saved for an Update Row, the
    ACTION column for all other Update Row source mappings is set to
    NotUsed. In this case, if the Add Row source does not have an ACTION
    set, Map does not update that mapping. The Add Row source’s action
    remains unchanged.

Auto Load Mapping History

If checked, when mapping is deleted and added back the mapping is
automatically restored to the latest mapping from history.

**NOTE:** Enabling this option can affect performance and add overhead
to the sync process.

If unchecked, when mapping is deleted and added back, the user must use
the Restore option on the <span style="font-style: italic;">[Field
Mapping History](../../Map/Page_Desc/Field_Mapping_History.htm)</span>
page to restore the mapping. Refer to [Restore Current Field Mapping
From
History](../../Map/Use_Cases/Restore_Current_Field_Mapping_From_History.htm)
for more information.

Build Xref Target Rules

If unchecked, Map builds cross reference rules at the source level for
those field mappings with an action of Xref or RuleXref.

If checked, Map builds cross reference rules at the target level for
those field mappings with an action of Xref or RuleXref.  By default,
the check box is unchecked.

Build Remediation Rule Reports

If checked, Map builds Transform Remediation Rule reports to display
data audit updates during the Transform Automation process.

**NOTE:** Enabling this feature may affect performance.

If unchecked, Map generates the remediation rule value to process, but
does not build the new view to generate the remediation report.

Reset Field Mapping

Displays the action taken when a user clicks the Reset icon for a field
mapping on the *[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)* page n Map or the
*[Automation SQL Field
Mappings](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H.htm)*
page in SQL AutoGen.

Options are:

  - **Reset all Field Mapping Fields** – All fields are cleared of
    values

**NOTE**: If the mapping is associated with a field group other than the
default field group (\* or “All”), the Target Relationship ID field is
not updated on a reset.

  - **Reset Status Fields only** – All fields retain values except for
    the Mapping Status and Rule Status, which are set to Pending Review.

Reset Value Mapping

Displays the action to take on value mappings for field mappings using
the Xref or RuleXref action when the field mappings are reset.

Reset Transform Rule

Displays the action to take on Transform rules for field mappings using
Copy, Default, Rule, Xref or RuleXref action when the field mappings are
reset.

Metric Options

Metric Daily Retention

Displays the number of days metrics are saved. The default value is 35.

This daily summary is used to build the Snap Shot metrics.

Metric Summary Retention

Displays the number of days metric summary data is saved. The default
value is 180.

Rule Options

Source Delete Rule Priority

Displays the priority Map assigns to a Source delete rule when the rule
is created. The default value is 19999.

Source Insert Rule Priority

Displays the priority Map assigns to a Source insert rule when the rule
is created. The default Value is 20000.

Source Priority Multiplier

Displays the number used to multiply against the field’s priority on the
*[Target
Fields](../../Design/Page_Desc/Target_Fields_H_Target_Design.htm)* page
in Map and the result is the Priority for the Rule in Transform. Source
rules will be registered in Transform using this priority, leaving gaps
in the priority numbers to be used for manual rules. For example, if the
field MEINS is priority 20, and the Source Priority Multiplier is set to
10, then Map would set the Source rule priority to 200 in Transform. The
default value is 10.

**NOTE:** Once a Source rule for a field is registered in Transform, Map
will not adjust the priority.

Target Priority Multiplier

Displays the number used to multiply against the field’s priority on the
*Target Fields* page in Map and the result is the Priority for the Rule
in Transform. Target rules will be registered in Transform using this
priority, leaving gaps in the priority numbers to be used for manual
rules. For example, if the field MEINS is priority 20, and the Source
Priority Multiplier is set to 10, then Map would set the Target rule
priority to 200 in Transform, The default value is 10.

**NOTE:** Once a Target rule for a field is registered in Transform, Map
will not adjust the priority.

Target Report Priority Multiplier

Displays the number used to multiply against the field’s priority on the
*Target Fields* page in Map and the result is the Priority for the Rule
in Transform. Target reports will be built and registered in Transform
using this priority, leaving gaps in the priority numbers to be used for
target reports created manually. For example, if a report is priority 20
and the Target Report Priority Multiplier is set to 10, then Map would
set the target priority to 200 in Transform. The default value is 10.

**NOTE:** Once a Target report is registered in Transform, Map will not
adjust the priority.

Target Report Remediation Priority Multiplier

Displays the number used to multiply against the field’s priority on the
*Target Fields* page in Map and the result is the Priority for the Rule
in Transform. Target reports with remediation will be built and
registered in Transform using this priority, leaving gaps in the
priority numbers to be used for Target reports with remediation created
manually. For example, if a report is priority 20, and the Target Report
Remediation Priority Multiplier is set to 10, then Map would set the
Target report with remediation priority to 200 in Transform. The default
value is 10.

**NOTE:** Once a Target report with remediation is registered in
Transform, Map will not adjust the priority.

## <span id="Transform_Tab"></span>Transform tab

 

Field

Description

Directory Paths

Source Path

Displays the path for the Source directory where Source files (generally
package files) that can be imported into Transform are stored.

Report Path

Displays the path where Transform will create report files. All files
are generated to the path:

C:\\DSW\\Report\\\<Wave Name\>-\<Process Area\>\\\<Target Name\>

For example, if Transform were generating reports for the target ttMARA
in the SouthAmerica Wave, MM Process Area, the reports would be written
to:

C:\\DSW\\Report\\SouthAmerica-MM\\ttMARA

Export Path

Displays the path where Transform will create export files. All files
are generated to the path:

C:\\DSW\\Export\\\<Wave Name\>-\<Process Area\>\\\<Target Name\>

For example, if Transform were generating an export file for the target
ttMARA in the SouthAmerica Wave, MM Process Area, the file  would be
written to:

C:\\DSW\\Export\\SouthAmerica-MM\\ttMARA

Package Path

Displays the path Transform will look in for package files.

Documentation Path

Displays the path where Transform will create documentation files.

Other

Temp Database Name

Displays the name of the temporary database used by Transform.

Audit Reports

If checked, Transform generates audit statistics during processing.

Run Remediation Rules

If checked, Transform runs remediation rules. This field should not be
checked for production loads.

Report File Generation Mode ID

Displays the mode for file system generation.

Values are:

  - **Automatic** – Both file system files and Report Cache are created.
  - **Custom** – Only file systems file are created
  - **On Demand** – Neither file system files nor Report Cache created.

The counts (i.e., the number of rows returned) on
Target/Source/Remediation/Audit Report pages are updated.

If the Report File Generation Mode ID is none, the Report Generation
Mode ID is Custom.

**NOTE:** Report Cache are only created if Publish is enabled.

File system files, sample and segment reports are created in a path on
the application server using folder names based on the Object, Target,
and Source names used in the report. The path displays in the Report
Path field.

The Report Cache is created in the Report Cache Data Source ID for My
Reports

When a user clicks the Access Report icon on the My Reports pages a file
is written to the file system (note that same location as the file
system file above).

Source Active On Build

If checked, Target Sources are auto-generated with a default status of
active in Transform. If unchecked, target sources are auto-generated
with a default status of inactive in Transform.

Filters

Prefix Delimiter

Displays the delimiter used to separate filter prefixes when more than
one filter is defined.

Procedure Filter

Displays the prefix used to filter Transform procedures.

Target Table Filter

Displays the prefix used to filter Target tables.

Target Rule Filter

Displays the prefix used to filter Target rules.

Target Report Filter

Displays the prefix used to filter Target reports.

Target Export Filter

Displays the prefix used to filter Target exports.

Source Table Filter

Displays the prefix used to filter Source tables.

Source Rule Filter

Displays the prefix used to filter Source rules.

Source Report Filter

Displays the prefix used to filter Source reports.

Import Table Filter

Displays the prefix used to filter import tables.

Report Settings

Default Report Format

Displays whether column headings in reports will include field names, a
translation of the field names, or both. Field names in a Target system
are often abbreviated or, in the case of SAP, are abbreviated in German.

Replacement Char

Displays a character to replace the following invalid characters: ? | :
\* ? “ \< \> in reports. The default value is ^.

Report Cache Data Source ID

Displays the name of the database that contains the tables storing the
results of report views.

**NOTE:** REPORT CACHE DATA SOURCE ID is required for the execution of
the Business Data Transformation and Report Delivery via Transform.

Report Header

Displays the header that will appear on all reports as defined on the
*[Report Headers/Footers (Setup)](Report_Headers_Footers_Setup.htm)*
page, accessible from *Navigation* pane in Transform by selecting
**Configuration \> Setup**.

Report Footer

Displays the footer that will appear on all reports as defined on the
*Report Headers/Footers (Setup)* page, accessible from *Navigation* pane
in Transform by selecting **Configuration \> Setup**.

Report Landscape

If checked, the report is printed in landscape format. If unchecked, the
report is printed in portrait format.

Report Generate Empty

If enabled, Transform will generate reports in the **Report Path** (set
in the **Report Path** field on this page) even when there are no
records on the report. If disabled, Transform will only generate a
report if the report contains data.

Report No Rec Count

If checked, reports will not contain a record count. If unchecked, the
record count is included on all reports.

Segment Signal Dir

If checked, Transform outputs Segment By reports to a single directory
with the SegmentBy value appended to the report file name. If unchecked,
Transform creates one directory per SegmentBy value.

Text Format Value

Displays the format for text in reports, either text format or x125.

Add IMEX

If checked, IMEX=1 is automatically added to Excel file connections,
which instructs CranPort or SSIS packages to read intermixed columns
(columns containing a mix of text and numbers) as text columns.

Generate Documentation

If checked, Transform creates technical documentation files.

Transform generates and saves versions of the Technical, Audit and Recon
documents as HTML files every time an object, target or Target Source is
processed.

Refer to [Generate Documentation for Objects, Targets, and Target
Sources](../../Transform/Use_Cases/Generate_Documentation.htm) for more
information.

Report Max Rows

Displays the maximum number of rows to be generated into an Excel file.
If the data contains more than the number of rows indicated by this
field, a delimited file is generated instead.

Report Max Support Rows

Displays the maximum number of records that can be generated into a file
(Excel or delimited).

<span style="font-family: Arial, sans-serif;">Report Column
Delimiter</span>

Displays the delimiter used to separate the report data into columns in
the report when the file is generated.

Report Column Qualifier

Displays the qualifier used to delineate column data containing spaces
or special characters.

Package Properties

Import Suffix

Displays the import suffix for CranPort or SSIS packages.

Export Suffix

Displays the export suffix for CranPort or SSIS packages.

Source Connection

Displays Connection 1 for import CranPort or SSIS packages and
Connection 2 for export CranPort or SSIS packages.

Destination Connection

Displays Connection 1 for export CranPort or SSIS packages and
Connection 2 for import CranPort or SSIS packages.

Temporary Prefix

Displays the prefix used for temporary CranPort or SSIS packages.

Destroy Temp Package

If checked, Transform destroys any temporary CranPort or SSIS packages
generated during report file creation. If disabled, the temporary
packages are saved on the web server for review.

 

## <span id="Construct_Tab"></span>Construct tab

|        |                                           |
| ------ | ----------------------------------------- |
| Field  | Description                               |
| Client | Client value used in views for filtering. |

 

<span id="Compare_Settings_Tab"></span>

## <span id="Compare"></span>Compare Settings tab

**NOTE**: This tab is only accessible if the current user is a member of
the WebApp group Wavesynchronizer in Console or is assigned to a
security role with access to the page. Refer to [Set
Security](../../../Platform/Sys_Admin/Use_Cases/Setting_security.htm) in
System Administration for more information.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Equal Color</p></td>
<td><p>Displays the text color used in the Field Comparison table when values are equal between the baseline Wave and the child Wave.</p>
<p>The table displays on the <em>Vertical</em> View of the results page for each element (Process Area, object, target and field).</p></td>
</tr>
<tr class="odd">
<td><p>Not Equal Color</p></td>
<td><p>Displays the text color used in the Field Comparison table when values are not equal between the baseline Wave and the child Wave.</p>
<p>The table displays on the Vertical View of the results page for each element (Process Area, Object, Target and field).</p></td>
</tr>
<tr class="even">
<td><p>Not IN Baseline Color</p></td>
<td><p>Displays the text color used in the Field Comparison table when a value exists in the child Wave, but not in the baseline Wave. The table displays on the Vertical View of the results page for each element (Process Area, Object, Target and field).</p></td>
</tr>
<tr class="odd">
<td><p>Not IN Child Color</p></td>
<td><p>Displays the text color used in the Field Comparison table when a value exists in the baseline Wave, but not in the child Wave. The table displays on the Vertical View of the results page for each element (Process Area, Object, Target and field).</p></td>
</tr>
<tr class="even">
<td><p>Strike Through Missing</p></td>
<td><p>If checked, if a value exists in one Wave and not the other, the text is formatted as a strikethrough.</p></td>
</tr>
</tbody>
</table>
