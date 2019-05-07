+++
title = 'Improve Page Load Performance Related to List Boxes'
solution = 'Platform'
+++

# Improve Page Load Performance Related to List Boxes

List boxes can often be a source of performance degradation due to their
elaborate configurations and lengthy lookup times that may have to occur
at a cell level. Even if disabled, on the loading of the page, the cell
value must be looked up to display to the user. If several list boxes
are located on the *Horizontal* View, page load time can be severely
inflated. An easy solution is to have a read-only view-level resolution
of the list source (assuming it is a view in the same database) on the
*Horizontal* View, and an editable list box on the *Vertical* View. This
keeps the description field visible on the *Horizontal* View of the
page, making it filterable and searchable, while greatly increasing
performance.

Alternatively, the list box on the *Horizontal* View can itself be
simplified when it is disabled. There is no need to include a complex
WHERE clause that may be present in the list box configuration, if it is
only meant to resolve values and not restrict user input or security.
Even this simple change can improve page load.
