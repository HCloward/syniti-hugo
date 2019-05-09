# Lock Records

A user that has the ability to add or edit the contents of the page can
perform this task.

For locking to occur on the page when an Excel template has been
downloaded containing that data, the reserved columns Locked By, Locked
On and boaLockType must be manually added to the underlying table(s) for
the page. Refer to [Add BOA Reserved Columns to
Tables](../WebApp_Dev/Add%20Reserved%20Columns%20%20to%20Tables) for
more information.

When records are locked, the data in those records cannot be edited or
imported until the record is unlocked. Refer to [Unlock
Records](Unlock_Records) for more information.

When a record is locked, the following columns are populated and the
information is viewable by hovering over the padlock symbol that
replaces the pencil icon used for editing:

  - **Locked By** — Displays the user that has the record locked.
  - **Locked On** – Displays the date and time the record was locked.
  - **boa Lock Type** – Displays the locking level used. The locking
    levels prevent simultaneous editing of the data to prevent
    inconsistency. The locking levels are:
      - **Locked via the UI** — The record is being edited by another
        user via the page in the UI.
    
      - **Locked via Excel Integration** — The record is being edited
        via a downloaded record set.
        
        **NOTE:** Only records locked via Excel integration can be
        unlocked via the Excel Integration panel.

Records remain locked until one of the following occurs:

  - The user who has the record locked uploads the spreadsheet

  - The **Unlock Records icon** in the Excel Integration panel is
    clicked

  - The time duration noted in the Record Lock Timeout field on the
    [Parameters](../Sys_Admin/Page_Desc/Parameters_All_TabsSysAdmin)
    page has expired.
    
    **NOTE:** The Record Lock Timeout only applies to records locked via
    the UI.
