# Group Import

<div class="use">

Use this page to [Import System Type Group
Tables](../Use_Cases/Import_Group_Tables.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Collect \> Targets</span> on
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Sources</span> icon for a
    target.
3.  Select a source.
4.  Click <span style="font-weight: bold;">Import Group Tables</span> on
    the Page
toolbar.

|                      |                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                | Description                                                                                                                                                                                                                                                                                                                                                                                                                        |
| System Type Group ID | Displays a System Type group, a logical grouping of tables such as Customer or Vendor, to import as a source.                                                                                                                                                                                                                                                                                                                      |
| Target               | Displays database where downloaded data is stored.                                                                                                                                                                                                                                                                                                                                                                                 |
| Source               | Displays database where data is refreshed from and stored in the target.                                                                                                                                                                                                                                                                                                                                                           |
| Schedule ID          | Displays schedule for when target is refreshed with source data. Refer to [Create Schedules](../../Common/Use_Cases/Create_Schedules.htm) for more information.                                                                                                                                                                                                                                                                    |
| Publish Schema Owner | If checked, the Table Schema Owner is imported to the target database, overriding the default Target Source Schema owner.                                                                                                                                                                                                                                                                                                          |
| Publish Rules        | If checked, rules that are assigned to the tables in the group import load into the rule configuration table and update data in the tables when processed. If unchecked, rules assigned to the tables do not load into the rule configuration table. There are no rules to process against the table. Once a rule is loaded into the table, there is no sync process between the group import and the current Target Source table. |
| Import Group Tables  | Click to import System Type group tables from Common.                                                                                                                                                                                                                                                                                                                                                                              |
