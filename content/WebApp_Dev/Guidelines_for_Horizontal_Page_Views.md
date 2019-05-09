+++
title = 'Guidelines for Horizontal Page Views'
solution = 'Platform'
+++

# Guidelines for Horizontal Page Views

When creating a *Horizontal* Page View:

  - Make the first column(s) in the views the keys from the table that
    will be registered to the page to which the *Horizontal* View is
    assigned.
  - Limit the number of fields on the view to avoid horizontal scrolling
    in DSP®  
  - Add columns in an order so that the flow of the page processes from
    left to right.
  - Use the naming convention **webXXXHor**, where **XXX** is the name
    of the table.
  - The name of the underlying table, which will be registered to the
    page, must be included in the name of the view.

Use these controls sparingly on large data sets in *Horizontal* Views:

  - List/Combo Boxes (especially with Dynamic WHERE clauses)
  - nvarchar(max)
  - Other extremely lengthy data type fields
