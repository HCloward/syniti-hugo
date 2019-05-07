+++
title = 'Security Definitions'
solution = 'Platform'
+++

# Security Definitions

<div class="use">

Use this page to [Register Security
Definitions](../Use_Cases/Register_Security_Definition.htm).

</div>

To access this page, select **Admin \>Security \> Security Definitions
\> Security Definitions** in the *Navigation*
pane.

|                          |                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                    | Description                                                                                                                                                                                                                                                                                                                                                                                              |
| SECURITY DEFINITION NAME | Displays name of the security definition. Use the naming convention WebAppName.SecViewTables.Columns.                                                                                                                                                                                                                                                                                                    |
| DATA SOURCE ID           | Displays name of the data source where security definition is created.                                                                                                                                                                                                                                                                                                                                   |
| DATA VIEW                | Displays view used to drive the security definition. This view must reside in the selected data source and must be named as web\*Sec. The columns in this view are used to restrict user access on pages where the security definition is applied. The view can also contain a column named "FriendlyName" that is used as a display value by on-site administrators when selecting specific key values. |
| DESCRIPTION              | Displays a descriptive name for the security definition intended to supplement the Security Definition Name.                                                                                                                                                                                                                                                                                             |
| KEYS                     | Click to manage columns for the \*Sec view that will be mapped to columns in the pages that invoke the security definition.                                                                                                                                                                                                                                                                              |
