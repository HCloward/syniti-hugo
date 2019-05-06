# Table Naming Conventions

Across the applications, a common naming convention is to name a table
with the singular form of the underlying data. For instance, if the
table is meant to store a data set representing customers, name the
table “Customer.” Additionally, prefixes are commonly attached to the
table name. “zt” represents application configuration data, whereas “tt”
represents expected user data. Configuration data may include user data,
but it’s still utilized by the application as configuration. For the
Customer example, the full table name is “ttCustomer.” This allows
developers to quickly identify and filter tables to learn and develop
the application further.

Refer to [Create Tables in SQL](Create_Tables_in_SQL.htm) for general
information.

When naming tables:

  - Consistently name tables with small data prefix (2 characters)
    followed by a descriptive name of the contents of the table.
  - Capitalize the first letter of each word, if multiple words are used
    in the table name, e.g., OrderDetail.
  - Do not abbreviate.
  - Use singular table names.
  - Do not use hyphens (“-“), spaces or slashes (“/”, “\\”) in the table
    name. Underscores are acceptable.

**NOTE:  ** Special characters in SQL Object names will break
functionality in DSP®.

The following table outlines the basic table naming conventions:

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Condition</p></td>
<td><p>Convention</p></td>
<td><p>Example</p></td>
</tr>
<tr class="even">
<td><p>Tables delivered with the application without data.</p>
<p><strong>NOTE</strong>: These tables often store user-entered data.</p></td>
<td><p>ttXXX, where tt defines the application and XXX describes the purpose of the table.</p></td>
<td><p>nwOrder</p></td>
</tr>
<tr class="odd">
<td><p>Tables delivered with the application with configuration data.</p></td>
<td><p>ztXXX, where XXX describes the purpose of the table.</p></td>
<td><p>ztParam</p></td>
</tr>
<tr class="even">
<td><p>Dynamic cross reference tables used as a base and configured onsite.</p></td>
<td><p>xtXXX, where XXX describes the purpose of the table.</p></td>
<td><p>xtControlStatus</p></td>
</tr>
<tr class="odd">
<td><p>Archive tables</p></td>
<td><p>rtXXX, where XXX describes the purpose of the table.</p></td>
<td><p>rtRequst</p></td>
</tr>
</tbody>
</table>
