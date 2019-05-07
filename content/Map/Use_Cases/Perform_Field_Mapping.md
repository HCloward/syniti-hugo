+++
title = 'Perform Field Mapping Overview'
solution = 'Migration'
+++

# Perform Field Mapping Overview

To map a field, at a high level:

1.  [Prepare for Field Mapping](#Prepare_for_Field_Mapping)

2.  [Access the Field Mappings Page](#Access_the_Field_Mappings_Page).

3.  Select the field to be mapped.

4.  Click **Edit**.
    
    [View the field descriptions for the Field Mappings
    page](../Page_Desc/Field_Mappings_H.htm)

5.  [Select an Action](#Select_an_Action).

6.  Complete fields based on the Action.

7.  Click **Save**.

8.  Select the field mapping.

9.  Click <span style="font-weight: bold;">Submit</span> on the Page
    toolbar; Map creates the SQL Objects (depending on the Action
    selected) and sends a notification to the Developer assigned to the
    Target or Source to review the mapping on the
    <span style="font-style: italic;">Mapping Approval</span> page.
    Refer to [Approve or Reject
    Mappings](Approve_or_Reject_Mappings.htm) for more information.

<span style="font-weight: bold;">NOTE:</span> Click
<span style="font-weight: bold;">Submit All</span> to submit all
mappings with a Mapping Status of In Progress and Complete (if that
Mapping Status was set manually by the user but had not yet been
submitted).

**NOTE:** Once the mapping has been approved, the
<span style="font-weight: bold;">RULE STATUS</span> is updated to In
Progress, and the field mapping is considered complete for Gate Wave
Metrics. Refer to [View Metrics](View_Metrics_Map.htm) for more
information. 

Refer to [Mapping Status and Rule
Status](Mapping_Status_and_Rule_Status.htm) for information about how
statuses change throughout the mapping process.

## <span id="Prepare_for_Field_Mapping"></span>Prepare for Field Mapping

Before performing field mapping, perform the following tasks:

  - [Sync Map and Target
    Design](../../Design/Use_Cases/Sync_Map_and_Target_Design_TD.htm)

  - Set a Source Database
Object

### <span id="Set_a_Source_Database_Object"></span>Set a Source Database Object

Before mapping, the Source database must be set for a Target Source (if
it has not already been set). If the
<span style="font-style: italic;">Field Mappings</span> page displays
SELECT Source in the Source DETAILS, then the Source database must be
set.

**NOTE:** The Source Database Object is included in the Source Table and
Source Rules name. It must be set before Source tables or rules can be
built. Users can perform field mappings without a Source table for field
mappings that use the Default, Internal and Not Used action.

<span style="font-weight: bold;">NOTE:</span> When a user sets the
Source database Object and clicks Save, Map validates that the Source
database Object exists in the System Type. If the Source database Object
does not exist:

  - If the user imported a System Type in Target Design for the Target
    Source, the Source database Object is imported into the System Type
  - If the user did not import a System Type in Target Design (as in, an
    Excel file import, database table import, or manual entry was used
    for the Target design), Map displays an error message that the user
    must set a System Type before field mapping can be performed. Add a
    System Type to a Target in Target Design (Design \> Targets
    \>Vertical View for a Target \> System Type ID).

To set the Source database in Map:

1.  Click **ProcessArea** in the *Navigation* pane.

2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map.htm)* page.

3.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.

4.  Click **Vertical View** for a Target Source.

5.  Click **Edit**.
    
    [View the field descriptions for the Target Sources page's Vertical
    View](../Page_Desc/Target_Sources_H_Map.htm)

6.  Select a table or view from the **Source Database Object** list box.

7.  Click
**Save**.

## <span id="Access_the_Field_Mappings_Page"></span>Access the *Field Mappings* Page

Map provides multiple navigation paths to the *[Field
Mappings](../Page_Desc/Field_Mappings_H.htm)* page. Depending on how the
page is accessed, different fields can be mapped.

<table>
<tbody>
<tr class="odd">
<td><p>Navigation</p></td>
<td><p>Fields to be mapped</p></td>
</tr>
<tr class="even">
<td><ol>
<li>Click <strong>ProcessArea</strong> in the <em>Navigation</em> pane.</li>
<li>Click the <strong>Targets</strong> icon on the <em><a href="../Page_Desc/Process_Area_Launch_map.htm">Process Area Launch</a></em> page.</li>
<li>Click the <strong>Sources</strong> icon for a Target.</li>
<li>Click the <strong>Update Row Sources</strong> icon for a Source.</li>
<li>Click the <strong>Secondary Source</strong> icon for an Add Row Source.</li>
<li>Click the <strong>Mappings</strong> icon for an Update Row Source.</li>
</ol></td>
<td><p>All field mappings for the selected Update Row Source.</p></td>
</tr>
<tr class="odd">
<td><ol>
<li>Click <strong>ProcessArea</strong> in the <em>Navigation</em> pane.</li>
<li>Click the <strong>Targets</strong> icon on the <em><a href="../Page_Desc/Process_Area_Launch_map.htm">Process Area Launch</a></em> page.</li>
<li>Click the <strong>Mappings</strong> icon for a Target.</li>
</ol></td>
<td><p>All field mappings for the selected Target.</p>
<p> </p></td>
</tr>
<tr class="even">
<td><ol>
<li>Click <strong>ProcessArea</strong> in the <em>Navigation</em> pane.</li>
<li>Click the <strong>Targets</strong> icon on the <em><a href="../Page_Desc/Process_Area_Launch_map.htm">Process Area Launch</a></em> page.</li>
<li>Click the <strong>Sources</strong> icon for a Target..</li>
<li>Click the <strong>Mappings</strong> icon for a Source.</li>
</ol></td>
<td><p>All field mappings for the selected Source.</p>
<p><strong>NOTE:</strong> This does not include mappings for Add Row or Update Row Sources.</p></td>
</tr>
<tr class="odd">
<td><ol>
<li>Click <strong>ProcessArea</strong> in the <em>Navigation</em> pane.</li>
<li>Click the <strong>Targets</strong> icon on the <em><a href="../Page_Desc/Process_Area_Launch_map.htm">Process Area Launch</a></em> page.</li>
<li>Click the <strong>Field Groups</strong> icon for a Target.</li>
<li>Click the <strong>Mappings</strong> icon for a field group.</li>
</ol></td>
<td><p>All field mappings for the selected field group.</p></td>
</tr>
<tr class="even">
<td><ol>
<li>Click <strong>ProcessArea</strong> in the <em>Navigation</em> pane.</li>
<li>Click the <strong>Targets</strong> icon on the <em><a href="../Page_Desc/Process_Area_Launch_map.htm">Process Area Launch</a></em> page.</li>
<li>Click the <strong>Sources</strong> icon for a Target.</li>
<li>Click the <strong>Update Row Sources</strong> icon for a Source.</li>
<li>Click the <strong>Mappings</strong> icon for an Add Row Source.</li>
</ol></td>
<td><p>All field mappings for the selected Add Row Source.</p></td>
</tr>
</tbody>
</table>

## <span id="Select_an_Action"></span>Select an Action

Each field mapping has an action that determines:

  - Whether Automation builds a rule
  - The type of rule that the Automation process builds

<span style="font-weight: bold;">NOTE:</span> A Rule Where Clause can be
added on the *Field Mappings* page’s vertical view to filter the records
to which a rule is applied.

  - The fields required to save the mapping on the
    <span style="font-style: italic;">Field Mappings</span> page
  - Whether value mapping is necessary to map values in Source fields to
    specific values in Target fields

Regardless of the action selected for a field mapping, the mapping
process is the same.

These options are available in the ACTION list box on the *Field
Mappings* page:

  - [Construction](Construction.htm)
  - [Copy](Copy_Map.htm)
  - [Default](Default_Action.htm)
  - [Internal](Internal.htm)
  - [Manual Rule](Manual_Rule.htm)
  - [Manual Construction](Manual_Construction.htm)
  - [Not Used](Not_Used.htm)
  - [Rule](Rule.htm)
  - [Rule Xref](Rule_Xref.htm)
  - [Xref](Xref.htm)

Depending on the action selected, different fields are required for the
record on the *Field Mappings* page. The following table lists the
Actions that have required fields on the
<span style="font-style: italic;">Field Mappings</span> page. Refer to
the sections corresponding to each action for more information.

|           |              |              |               |
| --------- | ------------ | ------------ | ------------- |
| Action    | SOURCE TABLE | SOURCE FIELD | DEFAULT VALUE |
| Copy      | X            | X            |               |
| Default   |              |              | X             |
| Rule XRef | X            | X            |               |
| XRef      | X            | X            |               |

 

The <span style="font-style: italic;">[Field
Mappings](../Page_Desc/Field_Mappings_H.htm)</span> page is a single
resource that allows users to map fields, view details about mappings,
and perform mapping-related tasks, including:

  - [Update Unmapped Fields to
    NotUsed](Update_Unmapped_Fields_to_NotUsed.htm)
  - [View all Mappings for a Target](View_all_Mappings_for_a_Target.htm)
  - [View Field Mapping History](View_Field_Mapping_History.htm)
  - [Restore Current Field Mapping From
    History](Restore_Current_Field_Mapping_From_History.htm)
  - [Copy a Mapping](Copy_a_Mapping.htm)
