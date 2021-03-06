# Template (ISA External Request Scenario) H

[Template (ISA External Request Scenario)
V](#Template__ISA_External_Request_Scenario__V)

<div class="use">

Use this page to [Create an External Request Scenario for an Information
Steward-initiated
Request](../Use_Cases/Create_an_External_Request_Scenario_for_an_Information_Steward%20initiated_Request)<span class="MsoHyperlink">.</span>

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspCompose \> Team</span> on
    the *Navigation pane*.
2.  Click <span style="font-weight: bold;">Templates</span> for a team.
3.  Click the <span style="font-weight: bold;">ISA External Request
    Scenarios</span> icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>RULE ID</p></td>
<td><p>Displays the rule name (e.g., NoRegion).</p></td>
</tr>
<tr class="odd">
<td><p>RULE BINDING ID</p></td>
<td><p>Displays the name of the ISA rule the scenario applies to (e.g., Customers – Region) listed on the Report Data Viewer page in ISA.</p></td>
</tr>
<tr class="even">
<td><p>REQUEST DESCRIPTION FORMAT</p></td>
<td><p>Displays the format used for the request description for a request created from this external request scenario. The DESCRIPTION field on the Request page defaults to Request from ISA - #Date# where the Date is the date a user clicked the Create Compose Request button on the Report Data Viewer page in the ISA.</p>
<p><strong>NOTE:</strong> A value preceded and followed by # is a dynamic substitution value for replacement at run time  A user can add these variables to the description.</p>
<ul>
<li>#ISAProjectID# - ISAProjectID (ISA Project ID)</li>
<li>#ISARuleBindingID# - ISARuleBindingID (ISA Rule Binding ID)</li>
<li>#ISARuleID# - ISARuleID (ISA Rule ID)</li>
<li>#RuleID# - ExternalRequestAlias (Rule ID)</li>
<li>#RuleBindingID# - Scenario (Rule Binding ID)</li>
<li>#RequestConnectionID# - RequestConnectionID (RequestConnectionID)</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Connections</p></td>
<td><p>Click to open the <em><a href="../../dspCompose/Page_Desc/Template_External_Request_Scenarios_Connections">Template (External Request Scenarios Connections)</a></em> page to set a connection to a target system for each process template.</p></td>
</tr>
</tbody>
</table>

 

## <span id="Template__ISA_External_Request_Scenario__V"></span>Template (ISA External Request Scenario) V

[Template (ISA External Request Scenario) H](#)

<div class="use">

Use this page to [Create an External Request Scenario for an Information
Steward-initiated
Request](../Use_Cases/Create_an_External_Request_Scenario_for_an_Information_Steward%20initiated_Request)<span class="MsoHyperlink">.</span>

</div>

Field

Description

Definition

ISA Project ID

Displays the name of the project that contains the IS rule that, when
run, generates a report. The data on this report can be used as the
basis for a request.

ISA Rule Binding ID

Displays the unique identifier for the ISA view on which the report is
based.

ISA Rule ID

Displays the ISA Rule Binding Description once the scenario has been
saved.

Rule ID

Displays the rule name (e.g., NoRegion).

Rule Binding ID

Displays the name of the ISA rule the scenario applies to (e.g.,
Customers – Region) listed on the Report Data Viewer page in ISA.

Connections

Click to open the *[Template (External Request Scenarios
Connections)](../../dspCompose/Page_Desc/Template_External_Request_Scenarios_Connections)*
page to set a connection to a target system for each process template

Advanced

Staging Data Source ID

Displays the name of the data source where the staging table will be
created and stored. The default dspCompose\_Data data source is the
recommended selection.

Staging Table Name

Displays the name of the table that will be used to import Information
Steward report data.

The name is automatically generated by dspCompose™ in the format st
\[Template Name\] \[Scenario\]\_ISAStaging.

**NOTE:** Data is moved from the ISA report to this staging table where
custom rules can then be run against the data before the data is moved
to the Data Entry table of a request.

Build Staging Area

Click to create the staging table in the data source identified in the
Staging Data Source ID field with the name in the Staging Table Name
field.

**NOTE:** If the template has not been generated, this icon is disabled.

Map Columns

Click to open the Template (External Request Scenario Column) page to
map columns from the staging table to columns in the template.

**NOTE:** If the template has not been generated, this icon is disabled.

**NOTE:** The count on this icon represents the number of columns that
have been mapped from the Information Steward report to the staging
table.

External Request Create Rules

Click to open the Template (Event Rule) page to add, edit and delete
rules. Refer to [Create Custom Rules for Information Steward-initiated
Requests](../Use_Cases/Create_Custom_Rules_for_Information_Steward%20initiated_Requests)
for more information.

**NOTE:** The count on this icon represents the number of rules that
have been added to the external request scenario. These rules run on
data in the staging table before it is moved to the data entry table.

Clear Staging Area

Click to clear the staging area, allowing the staging table to be
rebuilt if the ISA report must be rerun after the scenario was saved.
