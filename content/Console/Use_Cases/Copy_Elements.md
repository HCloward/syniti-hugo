# Copy Elements

A Wave, Process Area or Object can be created based on a copy of an
existing element.

This functionality can be accessed on the
*[Waves](../Page_Desc/Waves_H.htm)* page, and by navigating to
**Elements \> \[Element Name\]**. The Copy functionality is not
available when working in a specific hierarchy, such as when working on
the *[Wave: Process Areas](../Page_Desc/Wave_Process_Areas.htm)* page.

This use case includes the following topics:

  - [Copy a Wave](#Copy)

  - [Copy a Process Area](#Copy2)

  - [Copy or Move an Object](#Copy3)

## <span id="Copy"></span>Copy a Wave

A Migration Developer can copy a Wave. When a Wave is copied, all data
stored in Console and Target Design for the Wave is copied, along with
all objects, targets and sources in the Wave.

<span style="font-weight: bold;">NOTE</span>: When a Wave is copied, any
approved mappings in the original Wave are copied to the new Wave as
complete but not approved. These fields are not copied for the mapping
that is complete:

  - Approved On
  - Approved By
  - Created On
  - Created By
  - Rejected On
  - Rejected By
  - Submitted On
  - Submitted By

<span style="font-weight: bold;">NOTE</span>: Security settings for a
Wave are also copied. Any users who have security for the original Wave
can also access the copy of the Wave.

To copy a Wave:

1.  Click **Waves** in the *Navigation* pane.

2.  Select a Wave on the *[Waves](../Page_Desc/Waves_H.htm)* page.
    
    **NOTE**: If multiple Waves are selected, the copy function will
    only copy the first Wave selected.

<!-- end list -->

3.  Click the **Copy Wave** icon on the Page toolbar.

4.  Click **Edit**.

<!-- end list -->

5.  Enter a name for the copied Wave in the **New Name** field.
    
    **NOTE**: A Wave name can be a maximum of 10 characters long.

<!-- end list -->

6.  Click **Save**.

## <span id="Copy2"></span>Copy a Process Area

Copying a Process Area copies the Process Area description.

To copy a Process Area:

1.  Select **Elements \> Process Area** from the *Navigation* pane.

2.  Select a Process Area.
    
    **NOTE**: If multiple Process Areas are selected, the copy function
    will only copy the first Process Area selected.

3.  Click the **Copy Process Area** icon on the Page toolbar.

4.  Click **Edit**
    
    [View the field descriptions for the Copy Process Area
    page](../Page_Desc/Copy_Process_Area.htm)

5.  Enter a name for the copied Process Area in the **New Process Area**
    field.
    
    **NOTE**: A Process Area name can be a maximum of 15 characters
    long.

6.  Click **Save**.

## <span id="Copy3"></span>Copy or Move an Object

A user can:

  - [Copy an object to be used as the basis for a new object in the same
    process area](#To_copy_an_object_t)
  - [Copy an object to another process
    area](#To_copy_an_object_to_another)
  - [Move an object to another process area](#To_move_an_object_)

Copying an object copies the object owner, the object status, and the
description. History and metrics are not copied.

Moving an object between wave process areas retains all the history and
metrics for the object in the wave.

<span id="To_copy_an_object_t"></span>To copy an object to the same
process area:

1.  Select **Elements \> Object** from the *Navigation* pane.

2.  Select an object.

**NOTE**: If multiple objects are selected, the copy function only
copies the first object selected.

3.  Click the <span style="font-weight: bold;">Copy Object</span>icon on
    the Page toolbar.

4.  Click <span style="font-weight: bold;">Edit</span>.
    
    *[View the field descriptions for the Copy Object
    page](../Page_Desc/Copy_Object.htm)*

5.  Enter a name for the copied object in the **New Object** field.

6.  Enter a value in the **New Priority** field.
    
    **NOTE**: The priority sets the sort order for the object on the
    *[Object](../Page_Desc/Objects_H.htm)* page’s *Horizontal* View.

7.  Click **Save**.

<span id="To_copy_an_object_to_another"></span>To copy an object to
another process area:

1.  Select <span style="font-weight: bold;">Waves</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Process Areas</span> icon
    for a Wave.

3.  Click the <span style="font-weight: bold;">Objects</span> icon for a
    Process Area.

4.  Click the <span style="font-weight: bold;">Copy</span> icon.

5.  Click **Edit**.
    
    [View the field descriptions for the Copy Object to Process Area
    page](../Page_Desc/Copy_Object_to_Process_Area.htm)

6.  Select the new Process Area from the **Copy To Process Area** list
    box. 

7.  Click **Save**.

8.  Click the <span style="font-weight: bold;">Copy Object</span> icon
    on the Page toolbar.

**NOTE:** The Copy Object icon is disabled until a Process Area is
chosen in the Copy To Process Area list box.

<span id="To_move_an_object_"></span>To move an object to another
process area:

1.  Select <span style="font-weight: bold;">Waves</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Process Areas</span> icon
    for a Wave.

3.  Click the <span style="font-weight: bold;">Objects</span> icon for a
    Process Area.

4.  Click the <span style="font-weight: bold;">MOVE </span>icon on the
    Page toolbar.

5.  Click **Edit**.
    
    [View the field descriptions for the Move Object to Process Area
    page](../Page_Desc/Move_Object_to_Process_Area.htm)

6.  Select the new Process Area from the **Move To Process Area** list
    box.

7.  Click **Save**.

8.  Click the <span style="font-weight: bold;">Move Object</span> icon
    in the Page toolbar of the child pane.

**NOTE**: The Move Object icon is disabled until a Process Area is
chosen in the Move to Process Area list box.
