+++
title = 'Append BOA Reserved Columns to Tables'
solution = 'Platform'
+++

# Append BOA Reserved Columns to Tables

BOA reserved columns are (required fields are indicated by an \*):

  - boaStatus\*
  - AddedOn\*
  - AddedBy\*
  - AddedVia\*
  - ChangedBy\*
  - ChangedOn\*
  - ChangedVia\*
  - LockedOn
  - LockedBy
  - boaLockType

The required columns above must be added to every table.

When the user clicks the Append Columns icon on the Page toolbar of the
*Data Sources* page’s *Vertical* View, most of these reserved columns
are appended to all of the tables that do not already have them in the
database. A Designer can also add these columns manually.

**NOTE**: This feature is used for local SQL data sources only.

**NOTE**: **LockedOn** and **LockedBy** must be added manually where
appropriate. Add these columns for any table where multiple users may be
editing the same page at the same time to prevent multiple users from
editing the same record at the same time. 

With the exception of boaStatus, the appended column should not display
on the page so should not be added to the view.

**NOTE**: If the columns exist on the table, they display when a user
hovers the mouse cursor over the row edit pencil icon. This allows the
developer to exclude the columns from the view, but still take advantage
of them.

**NOTE:** Reserved columns are only automatically added to tables when
the Append Columns icon is clicked on the *Data SourcesVertical* View.
Columns are not automatically appended to tables added after this
operation is performed. In other words, if tables are added to the data
source later, click the Append Columns icon again to add the reserved
columns to the new tables.

**NOTE:** If the columns exist on the table, they display in the
Information pane below the Navigation pane when a user hovers the mouse
cursor over a row’s edit pencil icon. This allows the Designer to
exclude the columns from the view, but still display the column's values
on the page.
