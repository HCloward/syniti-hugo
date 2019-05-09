+++
title = 'Wave Compare for Object Results H'
solution = 'Migration'
+++

# Wave Compare for Object Results H

[Wave Compare for Object Results
V](Wave_Compare_for_Object_Results_H#Wave_Compare_for_Object_Results_V)

<div class="use" data-xmlns="">

Use this page to [Synchronize Target Designs Across
Waves](../Use_Cases/Synchronize_Target_Designs_Across_Waves).

</div>

**NOTE**: This page is only accessible if the current user is a member
of the WebApp group WaveSynchronizer in Console or is assigned to a
security role with access to the page. Refer to [Set
Security](../../../Platform/Sys_Admin/Use_Cases/Setting_security) in
System Administration for more information.

To access this page:

1.  Select
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">dspMigrate</span>
    in the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Navigation</span>
    pane, or select
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Console</span>
    in the Context bar.
2.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">
    Build Comparison</span> icon in the Page toolbar.
3.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Objects</span>
    icon.

|                          |                                                                                                                                                                                                                                                                |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                    | Description                                                                                                                                                                                                                                                    |
| Hide Identical           | Click to hide or unhide all matching comparisons in the Objects (as in, those comparisons that do not need to be synced) to make comparisons easier to review.                                                                                                 |
| Sync Object              | Click to sync the Target design in the selected Object between the child Wave and the baseline Wave.                                                                                                                                                           |
| Sync All Objects         | Click to sync the Target design in all Objects between the child Wave and the baseline Wave.                                                                                                                                                                   |
| Process Area             | Displays the Process Area in the child Wave that has been compared to the baseline Wave.                                                                                                                                                                       |
| OBJECT                   | Displays the Object in the child Wave that has been compared to the baseline Wave.                                                                                                                                                                             |
| DATA SOURCE ID           | Displays the data source for the Object, which is a Transform database. This database is where all Target tables and all Source tables will be registered.                                                                                                     |
| DATA SERVICES REPOSITORY | Displays the name of the repository, a set of tables that stores user-created and predefined system Objects, Source and Target metadata and transformation rules. Repositories are configured in SAP Data Services, and then registered in Common in the DSP®. |
| Targets                  | Click to open the *[Wave Compare for Target Results](Wave_Compare_for_Target_Results)* page to review differences and sync the baseline and child Wave Target design at the Target level.                                                                  |
| Fields                   | Click to open the *[Wave Compare for Target Field Results](Wave_Compare_for_Target_Field_Results)* page to review differences and sync the baseline and child Wave Target design at the Target field level.                                                |

## <span id="Wave_Compare_for_Object_Results_V"></span>Wave Compare for Object Results V

[Wave Compare for Object Results
H](Wave_Compare_for_Object_Results_H)

|                  |                                                                                                                                                                |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field            | Description                                                                                                                                                    |
| Hide Identical   | Click to hide or unhide all matching comparisons in the Objects (as in, those comparisons that do not need to be synced) to make comparisons easier to review. |
| Process Area     | Displays the Process Area in the child Wave that has been compared to the baseline Wave.                                                                       |
| Object           | Displays the Object in the child Wave that has been compared to the baseline Wave.                                                                             |
| Field Comparison | Displays a table that lists the fields in the baseline Wave and the child Wave and the differences between them for the selected Object.                       |
