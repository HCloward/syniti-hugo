+++
title = 'Organize Quick Links'
solution = 'Platform'
+++

# Organize Quick Links

Quick Links can be put in a specific order and grouped together.

To organize quick links into groups, populate the **GROUP** field on the
*Quick Links* page. A heading for the group is automatically created in
the drop down list of quick links that displays when users click the
Quick Link icon on the Site toolbar.

To configure quick links in a specific order, modify the **Priority**
field on the *Quick Links* page.

When groups are used, the Priority field is considered to organize the
groups and quick links within the group. The lowest prioritized quick
link displays at the top of the quick links list (accessible when
clicking the Quick Links icon on the Site toolbar). If a group is
assigned to a quick link, the lowest prioritized quick link with a group
displays above higher Priority values.

Consider the following example:

|          |              |           |
| -------- | ------------ | --------- |
| **Page** | **Priority** | **Group** |
| Target   | 15           | Migrate   |
| Report   | 25           | Monitor   |
| Source   | 35           | Migrate   |
| Admin    | 10           | \<null\>  |

 

The quick link list displays as follows:

 

Admin

Migrate

<span>               </span> Target

<span>               </span> Source

Monitor

<span>               </span> Report

 

“Admin” displays first because it has the lowest Priority. The group
“Migrate” displays next because one of the links within the group
(“Target”) has the next lowest Priority. “Source” displays next, even
though it has the highest Priority, because it belongs to a group that
has already been ordered based on the Priority of another quick link
within the group. And finally, the group “Monitor” displays last because
the Priority of “Report” (25) is greater than the Priority of “Target”
(15).
