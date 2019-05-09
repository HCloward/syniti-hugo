+++
title = 'Advanced View Builder H'
solution = 'Platform'
+++

# Advanced View Builder H

[Advanced View Builder V](#Advanced_View_Builder_V)

<div class="use">

Use this page to [Build Advanced
Views](../Use_Cases/Build_Advanced_Views) and [Create Collect Target
Views](../../../Master_Data_Mgmt/dspConduct/Use_Cases/Auto_Generate_Request_related_Objects#Create_Collect_Target_Views)
for dspConduct™.

</div>

To access this page, select <span style="font-weight: bold;">Collect \>
Tools \> Advanced View Builder </span>in
<span style="font-style: italic;">Navigation</span>
pane.

|                       |                                                                                                                                                                                                                                                                                               |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                 | Description                                                                                                                                                                                                                                                                                   |
| Build View            | Click to create views in the database listed in the Database for View field. Views have the same name as the tables provided in the database listed in the Database for Tables field. SAP Client and SAP Language are added to Where clause when those columns are found in the source table. |
| DATABASE FOR VIEWS    | Displays the target database where new rules will be created.                                                                                                                                                                                                                                 |
| DATABASE FOR TABLES   | Displays source database used to create views.                                                                                                                                                                                                                                                |
| TRANSFORM PARAM TABLE | If enabled, the table is a view or a table in Database For Views database, and SQL joins are created in the view, linking Transform Param to the source table.                                                                                                                                |
| SAP CLIENT            | Displays name of the client within the SAP instance that is added to the Where clause.  When Transform Param Table is enabled, the SAP Client field is ignored                                                                                                                                |
| LANGUAGE              | Displays default language of SAP instance that is added to the Where clause. Displays name of client name within SAP instance.  When Transform Param Table is enabled, the Language field is ignored                                                                                          |
| GROUP FOR VIEWS       | Displays group; views are built for all active tables in the group.                                                                                                                                                                                                                           |
| GENERATED             | Displays date and time when view was built.                                                                                                                                                                                                                                                   |

## <span id="Advanced_View_Builder_V"></span>Advanced View Builder V

[Advanced View Builder H](Advanced_View_Builder_H)

<div class="use">

Use this page to [Build Advanced
Views](../Use_Cases/Build_Advanced_Views).

</div>

|                       |                                                                                                                                                                    |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field                 | Description                                                                                                                                                        |
| Database For Views    | Displays target database where new rules will be created.                                                                                                          |
| Database For Tables   | Displays source database used to create views.                                                                                                                     |
| Description           | Displays brief description of the view, e.g., the function of the view.                                                                                            |
| Transform Param Table | If enabled, the table is a view or a table in the Database For Views database, and SQL joins are created in the view, linking Transform Param to the source table. |
| SAP Client            | Displays the name of client within the SAP instance that is added to the Where clause.  When Transform Param Table is enabled, SAP Client is ignored               |
| Language              | Displays default language of SAP instance that is added to the Where clause. When Transform Param Table is enabled, Language is ignored                            |
| Group For Views       | Displays group; views are built for all active tables in the group.                                                                                                |
| Generated             | Displays date and time when view was built.                                                                                                                        |
| View Built Count      | Displays number of views built.                                                                                                                                    |
