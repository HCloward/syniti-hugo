+++
title = 'Page Control View'
solution = 'Platform'
+++

# Page Control View

Business requirements may require edit and delete capabilities to be
disabled, depending on the state of the page as a whole. **Page Control
Views** (PCV) are created in SQL to determine if records can be added,
edited and deleted based on the state of the page.

Once created in SQL, the view needs to be registered to the page in DSP®
(**Admin \> WebApps \> Pages \> Vertical View \> Control Views tab**).

Refer to [Control Views](Control_Views) for general information.

When creating Page Control Views:

  - Use the naming convention **webXXXPcv**, where **XXX** is the table
    name on the calling page.
  - Use a PCV when the control status determinations are to be made
    based on what is known of the page as a whole (e.g. binding
    criteria, shared criteria or boaPageID).
  - Include all key and criteria columns on the page to control.
  - Include all column names for the technical names of the columns on
    the page that contains the control status values (0, 1 or 2).
  - Prefix the column containing the control status with **boaCtl** when
    assigning a control status to a key column.
