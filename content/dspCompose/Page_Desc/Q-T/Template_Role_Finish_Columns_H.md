+++
title = 'Template Role (Finish Columns) H'
solution = 'Data Quality'
+++

# Template Role (Finish Columns) H

[Template Role (Finish-Columns) V](#Template_Role_Finish1)

<div class="use">

Use this page to [Register Tables for Download as a Finish
Process](../Use_Cases/Register_Tables_to_Download_as_a_Finish_Process_Using_Collect.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspCompose \>
    Team</span> on *Navigation *pane.
2.  Click <span style="font-weight: bold;">Templates</span> for a team.
3.  Click <span style="font-weight: bold;">Roles</span> for a template.
4.  Click <span style="font-weight: bold;">Vertical View</span> for the
    Post role.
5.  Click the <span style="font-weight: bold;">Approve and Finish
    Settings</span> tab.
6.  Click <span style="font-weight: bold;">Finish Tables</span>.
7.  Click the <span style="font-weight: bold;">Source Filter
    Columns</span> or the <span style="font-weight: bold;">Target Filter
    Columns</span>
icon.

|        |                                                                                             |
| ------ | ------------------------------------------------------------------------------------------- |
| Field  | Description                                                                                 |
| FILTER | Displays filter placed on the source or target database table to download specific columns. |

## <span id="Template_Role_Finish1"></span>Template Role (Finish-Columns) V (All Tabs)

[Template Role (Finish-Columns) H](Template_Role_Finish_Columns_H.htm)

<div class="use">

Use this page to [Set a Filter
Column](../Use_Cases/Register_Tables_to_Download_as_a_Finish_Process_Using_Collect.htm#Set_a_Filter_Column)
and [Use Custom
Syntax](../Use_Cases/Register_Tables_to_Download_as_a_Finish_Process_Using_Collect.htm#Use_Custom_Syntax).

</div>

This page contains the following tabs:

  - [Column Filter tab](#Column_Filter_Tab)

  - [Where Clause Filter tab](#Where_Clause_Filter_Tab)

## <span id="Column_Filter_Tab"></span>Column Filter tab

Field

Description

Column

Column Name

Displays name of column being filtered on when the table is downloaded
from the source database during the Finish process. The column name
contains the values to use for the Where clause.

Data Source ID

Displays name of the database that contains the table where the column
is located.

Table Name

Displays name of the table that contains the column being filtered.

Mapped Value

Displays mapped value for the column. If a mapped value is selected,
when the Finish process runs, dspCompose™ selects all values from the
mapped value binding on RequestID and RoleID (if they exists in the
database object) and forms an IN statement for selection from the source
to the target database.

Fixed Value

Displays the value used as the condition of the matching value for
download.

Custom

If enabled, custom syntax can be entered for the finish process. These
settings are used in the case that the schema cannot be determined for
either the source or the target.

Custom Settings

Beginning Qualifier

Displays character placed around the values
<span style="font-size: 11.0pt;font-family: Arial, sans-serif;">downloaded
during the finish process when custom syntax must be used</span>.

Ending Qualifier

Displays character placed around the values
<span style="font-size: 11.0pt;font-family: Arial, sans-serif;">downloaded
during the finish process when custom syntax must be used.</span>

Separator

Displays character used for data values
<span style="font-size: 11.0pt;font-family: Arial, sans-serif;">downloaded
during the finish process when custom syntax must be used.</span>

Where Statement

Displays format of the where clause. dspCompose™ allows two dynamic
substitution values to be used in the Where Statement: \#ColumnName\# is
the name of the column and \#Data\# is the list of values separated by
the character in the Separator field.

## <span id="Where_Clause_Filter_Tab"></span>Where Clause Filter tab

<div class="use">

Use this tab to [Enter a Where
Clause](../Use_Cases/Register_Tables_to_Download_as_a_Finish_Process_Using_Collect.htm#Enter_a_Where_Clause).

</div>

Field

Description

Manual Where Clause

Where Clause

Displays where clause used to limit columns downloaded during the Finish
process.
