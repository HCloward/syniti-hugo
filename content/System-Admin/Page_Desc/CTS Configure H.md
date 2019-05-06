# <span id="CTS_Configure_H">CTS Configure H</span>

[](#CTS)

CTS Configure V

<div class="use">

Use this page to [Set a Baseline CTS Configuration for a Custom
WebApp](../Use_Cases/Set%20a%20Baseline%20CTS%20Configuration%20for%20a%20Custom%20WebApp.htm).

</div>

To access this page, click **Admin \> CTS \> Configuration** in the
*Navigation* pane.

**NOTE:** Do not update the configurations on this page for delivered
WebApps. However, these settings must be configured if you are CTS’ing a
Custom WebApp.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>DATA SOURCE ID</p></td>
<td><p>Displays the name of the data source that stores the shippable items.</p></td>
</tr>
<tr class="odd">
<td><p>Shippable Items</p></td>
<td><p>Click to open the <em><a href="CTS%20Configure%20Shippable%20Items.htm">CTS Configure (Shippable Items)</a></em> page to add and update the tables and columns used for each item.</p>
<p>Shippable items for delivered WebApp components are included by default, but can be updated.</p>
<p>Shippable items for custom WebApps must be set on this page.</p></td>
</tr>
<tr class="even">
<td><p>Registrations</p></td>
<td><p>Click to open the <em><a href="CTS%20Configure%20SQL%20Object%20Registrations.htm">CTS Configure (SQL Object Registrations)</a></em> page to register SQL Objects to CTS Config items.</p>
<p>Object registrations for delivered WebApp components are included by default, but can be updated.</p>
<p>Object registrations for custom WebApps must be set on this page.</p></td>
</tr>
<tr class="odd">
<td><p>SQL Objects</p></td>
<td><p>Click to open the <em><a href="CTS%20Configure%20SQL%20Objects.htm">CTS Configure (SQL Objects)</a></em> page to view and edit individual configurations for SQL Objects.</p>
<p>SQL Objects for delivered WebApps are included in the default configuration and must not be updated.</p>
<p>SQL Objects for custom WebApps are automatically added to the SQL Objects page when a user clicks the Generate Config button on this page’s <em>Vertical</em> View.</p></td>
</tr>
<tr class="even">
<td><p>Dependencies</p></td>
<td><p>Click to open the <em><a href="CTS%20Configure%20SQL%20Object%20Dependencies.htm">CTS Configure (SQL Object Dependencies)</a></em> page to view dependencies among objects for the CTS process.</p>
<p>Object dependencies for delivered WebApps are included in the default configuration and must not be updated.</p>
<p>Dependencies or custom WebApps are automatically added to the <em>CTS Configure (SQL Object Dependencies)</em> page when a user click the Generate Config button on this page’s <em>Vertical</em> View.</p></td>
</tr>
<tr class="odd">
<td><p>Relationships</p></td>
<td><p>Click to open the <a href="CTS%20Configure%20SQL%20Object%20Relationships.htm">CTS Configure (SQL Object Relationships)</a> <em></em> page to view the foreign key and child name for relationships used by the CTS process.</p>
<p>Object relationships for delivered WebApps are included in the default configuration and must not be updated.</p>
<p>Relationships for custom WebApps are automatically added to the <em>CTS Configure (SQL Object Relationships)</em> page when a user clicks the Generate Config button on this page’s <em>Vertical</em> View.</p></td>
</tr>
</tbody>
</table>

## <span id="CTS"></span>CTS Configure V

[CTS Configure H](#CTS_Configure_H)

Field

Description

Data Source ID

Displays the name of the data source that stores the shippable items.

Properties

Trusted Cache

If checked, this data source is for a delivered WebApp, and the
configuration must not be updated.

If unchecked, the data source is for a custom WebApp. The user can
generate the configuration automatically by clicking Generate Config on
this page.

Registration Filter

Displays the naming convention used for items to display in the VIEW
NAME list box on the *[CTS Configure (SQL Object
Registrations)](CTS%20Configure%20SQL%20Object%20Registrations.htm)*
page.

List Filter

Displays the naming convention used for items to display in the LIST
TABLE list box on the [CTS Configure (Shippable Item
Keys)](CTS%20Configure%20Shippable%20Item%20Keys.htm) page.

Maintenance

Generate Config

Click to generate a baseline configuration for SQL Objects for Custom
WebApps, including dependencies and relationships in the specified data
source and in other data sources as dependencies define them.

Prepare To Ship

Click to clean up the data source's CTS configuration prior to shipping
a new version of the custom WebApp. This should be run if the data
source's schema is static once shipped (as in, developers will not be
making changes to the data source schema on site). This operation
deletes all automatically generated views, functions and procedures as
well as object dependencies. These should not be needed if the schema is
going to remain static. Afterwards, the Trusted Cache option is enabled
to speed up CTS operations.
