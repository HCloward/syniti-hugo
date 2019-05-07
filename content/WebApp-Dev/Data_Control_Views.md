+++
title = 'Data Control Views'
solution = 'Platform'
+++

# Data Control Views

Data Control Views are created in SQL and define control based on what
is known about the data on the page. For example, a DCV could be used to
determine if a record can be edited or  deleted or if buttons are
disabled based on the state of the record.

Once created in SQL, the view must be registered to the page in DSP®
(**Admin \> WebApps \> Pages \> Vertical View \> Control Views tab**).

Refer to [Control Views](Control_Views.htm) for general information.

The following guidelines should be used when creating Data Control
Views:

  - Use the naming convention **webXXXDcv**, where **XXX** is the name
    of the table registered to the page.
  - Include all key and criteria columns on the page to control.
  - Include all column names for the technical names of the columns on
    the page that contain the control status values   (0, 1 or 2).
  - Prefix the column containing the control status with **boaCtl** when
    assigning a control status to a key column.

As an example, a user could disable the **Product History** and **Order
ID** icons on the *Customers* page where the count on the linked pages
is zero.
