+++
title = 'Report Repositories H'
solution = 'Data Quality'
+++

# Report Repositories H

[Report Repositories V](#Report_Repositoriess_V)

<div class="use">

Use this page to Register Report Repositories in dspMonitor™.

</div>

To access this page, select **Configuration \> Report
Repositories** in the
*Navigation* pane.

|                 |                                                                                                                                         |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                             |
| REPOSITORY      | Displays name of database where reports reside.                                                                                         |
| Reports         | Click to manage reports within the report repository.                                                                                   |
| Collect Targets | Click to open the *[Repository Collect Target](Repository_Collect_Target.htm)* page to register Collect targets to a report repository. |

## <span id="Data_Sources_V"></span>Report Repositories V

[Report Repositories H](#Report_Repositories_H)

<div class="use">

Use this page to:Register Report Repositories in dspMonitor™

</div>

Field

Description

Repository

Displays name of database where reports reside.

Report Filter

Displays naming convention for reports within the report repository.

Opportunity View Filter

Displays the view that filters the selection options in the Opportunity
View list box on the *[Repository Reports](Repository_Reports_H.htm)*
page.

**NOTE:** The recommended value is tv\*OptSel. If this value is entered,
when configuring reports on the *Repository Reports* page, only views
that follow the naming convention of tv\*OptSel are available to choose
as an Opportunity View from the drop down list. If no value is selected,
the Default Opportunity View Filter from the *Parameters* page is used.

Cache Database Name

Displays name of separate report repository used for cache tables.

Data Quality Scoring Threshold

Threshold ID

Displays the threshold ID used for data quality scoring.

**NOTE:** If no threshold is selected, the threshold ID set on the
*Parameters* page is used in the data quality score status calculation.
Refer to [Register Data Quality Score
Thresholds](../Use_Cases/Populate_Configuration_Tables.htm#Register_Data_Quality_Score_Thresholds)
for more information.
