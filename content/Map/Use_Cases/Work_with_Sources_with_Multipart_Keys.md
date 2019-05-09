+++
title = 'Work with Sources with Multi-part Keys'
solution = 'Migration'
+++

# Work with Sources with Multi-part Keys

Map allows a user to map multiple sources to one target, and to map
multiple sources with multi-part keys to a target.

The sources are assigned to the target in Target Design.

ZLegacy\<KeyFieldName\> is the key for the target table. Map the keys on
the source table to the ZLegacy\<KeyFieldName\> on the
<span style="font-style: italic;">Field Mappings</span> page.

If a source has more keys or a different number of keys than the target,
add a mapping that uses a Rule action to concatenate key values on the
source table into a single target key field beginning with ZLegacy.

To map multiple sources to a target when each source has one key, the
key can be mapped to the primary key in the target, and the source
tables are brought into Map and mapped to a target using the same
procedures as with a single source to single target mapping.  In this
case, the primary keys from multiple sources are mapped to the same
primary key in the target.

Map also allows a user to map a source (or multiple sources) that has
multi-part keys to a target with one key.

A user can map a multi-part key from a source to a single key in a
target using the <span style="font-style: italic;">Field Mappings</span>
page in Map or a view created from the source table.  

To map a multi-part key in a source to a single key in a target using
the <span style="font-style: italic;">[Field
Mappings](../Page_Desc/Field_Mappings_H)</span> page:

1.  Assign the source to the target in Target Design.
2.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map)* page in Map.
3.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.
4.  Click the <span style="font-weight: bold;">Mapping</span> icon for
    the Target Source with the multi-part key.
5.  Enter <span style="font-weight: bold;">zLegacy {Key Field
    Name}</span> in the <span style="font-weight: bold;">Search</span>
    field and press <span style="font-weight: bold;">Enter</span>.
6.  Click <span style="font-weight: bold;">Edit</span> for the
     zLegacy{Key Field Name\].
7.  Select <span style="font-weight: bold;">Rule</span> from the
    <span style="font-weight: bold;">Action</span> list box.
8.  Enter the concatenated names of the multi-part key in the
    <span style="font-weight: bold;">Rule SQL </span>field, with a **+**
    sign between each part of the field. For example, enter
    ProductID+Plant.
9.  Click <span style="font-weight: bold;">Save</span>.
10. Click the <span style="font-weight: bold;">Submit</span> icon in the
    Page toolbar.
