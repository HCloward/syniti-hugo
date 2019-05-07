+++
title = 'Object Columns H'
solution = 'Platform'
+++

# Object Columns H

[Object Columns V](#Object_Columns_V)

<div class="use">

Use this page to [Configure
Columns](../Use_Cases/Configure_Columns.htm).

</div>

To access this page:

1.  Click **Analyze** in the *Navigation* pane.
2.  Click the **Duplicates** icon for the Data Source ID.
3.  Select an object.
4.  Click **Columns** on the Page
toolbar.

|                     |                                                                                                                                                                                                                                                                                                                                                                                                  |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field               | Description                                                                                                                                                                                                                                                                                                                                                                                      |
| COLUMN              | Displays column being searched for duplicates.                                                                                                                                                                                                                                                                                                                                                   |
| ORDER               | Displays sort order of columns within the object.                                                                                                                                                                                                                                                                                                                                                |
| KEY                 | If enabled, the column is marked as the key for the table.                                                                                                                                                                                                                                                                                                                                       |
| DUPLICATE DETECTION | If enabled, column is included in the duplicate detection process.                                                                                                                                                                                                                                                                                                                               |
| SHOW NAME           | If enabled, the column name displays on the *[Results](Results.htm)* page.                                                                                                                                                                                                                                                                                                                       |
| BOLD                | If enabled, the column name is bold on the *Results* page.                                                                                                                                                                                                                                                                                                                                       |
| LINE BREAK          | If enabled, a line break is placed after the column name on the *[Results](Results.htm)* page. This feature allows the fields to be formatted to fit nicely on the *Results* page. For example, a line break would appear after the Name and Address fields, but not after the City and Region fields. The later fields are typically displayed on the same line in an address (City State Zip). |

## <span id="Object_Columns_V"></span>Object Columns V

[Object Columns H](#)

Field

Description

Column

Displays column being searched for duplicates

Duplicate Parameters

Key

Click to signify column is the key for the table.

Duplicate Detection

Click to include column in duplicate detection process.

Dictionary ID

Displays ID associated with dictionary, which contains a list of words
and synonyms used to match words in the duplicate detection process.

Must Match

Click to require two records to match exactly in order to be considered
a duplicate. Must Match is only available if Duplicate Detection is
enabled for the column.

Allow Synonym

Click to indicate that two records may be a duplicate if the field is
not an exact match, but is a match based on a field dictionary synonym,
e.g., ST = STREET. Allow Synonym is only available if a dictionary for
the column is specified and if Must Match is enabled.

Allow SoundEx

Click to indicate that two records may be a duplicate if the field is a
Soundex match rather than an exact match.

Display

Order

Displays sort order of columns within object.

Show Name

Click to display column name on the *[Results](Results.htm)* page.

Bold

Click to bold column name on the *Results* page.

Line Break

Click to place a line break after column name on the *Results* page.
This feature allows the five fields to be formatted to fit nicely on the
*Results* page. For example, a line break would appear after the Name
and Address fields, but not after the City and Region fields. The later
fields are typically displayed on the same line in an address (City
State Zip).
