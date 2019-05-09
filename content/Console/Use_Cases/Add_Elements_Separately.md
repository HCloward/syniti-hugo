+++
title = 'Add Elements Separately'
solution = 'Migration'
+++

# Add Elements Separately

One method for creating a context is to add a Process Area and Object
separately, then assign them to a Wave.

  - [Add a Wave](#Add2)

  - [Add a Process Area](#Add)

  - [Add an Object](#Add3)

  - [Add Elements to a Wave](#Add4)

## <span id="Add2"></span>Add a Wave

Add a Wave on the *[Waves](../Page_Desc/Waves_H)* page, the first
page that opens when Console opens (also accessible by clicking
**Waves** on the *Navigation* pane).

A *Wave* is a categorization for a migration project and is the first
level of the hierarchy. A migration project must have at least one Wave,
but can have multiple Waves. A Wave could be a country where a migration
project is rolled out or a specific work location.

A Wave contains a data source which contains the target tables
downloaded from an ERP system.

To add a Wave in Console:

1.  Click **Add** on the *Waves* page.
    
    *[View the field descriptions for the Waves
    page](../Page_Desc/Waves_H)*

2.  Enter a Wave name in **NAME** field.
    
    **NOTE:** This name and the name of the Process Area are combined to
    create a context.
    
    **NOTE:** A Wave name can be a maximum of 10 characters long.
    
    **NOTE:** The **ACTIVE** check box is checked by default. If the
    check box is not checked for a Wave, the contexts that use this Wave
    will not display in the Context bar and cannot be used in
    dspMigrate™.

3.  Add a description of the Wave in the **DESCRIPTION** field.

4.  Click **Save**; the *Vertical* View displays.

5.  Select an option from the **Target System** list box.
    
    **NOTE:** A Wave can have multiple target systems. Refer to [Add
    Multiple Target Systems at the Wave-Process Area
    Level](Add_Multiple_Target_Systems) for more information.
    
    **NOTE:** To use IGC’s Migration dashboard, set the Start Date and
    End Date. Refer to [Configure the IGC Migration
    Dashboard](../../../Platform/Agent_Int/Use_Cases/Configure_the_Migration_Dashboard)
    for more information.

6.  Click **Save**.

A Wave can also be added by copying an existing Wave. Refer to [Copy
Elements](Copy_Elements) for more information.

**NOTE:** If a user is currently working in a context (as in, that
context displays on the user’s Context bar), neither the Wave nor
Process Area in the context can be deleted.

Continue with Add a Process Area.

## <span id="Add"></span>Add a Process Area

A <span style="font-style: italic;">Process Area</span> is used to group
an ERP system’s objects. It is the second level of the hierarchy and is
assigned to a Wave.

**NOTE**: The combination of a Wave and Process Area is a context and is
used on the Context bar to drive the work in other components. Refer to
[Context, the Context Bar, and Navigation in
dspMigrate™](../../dspMigrate/Context_Navigation) for more
information.

Examples of Process Areas for an ERP integration are Sales and
Distribution (SD), Purchase to Pay (P2P) or Human Capital Management
(HCM).

To add a Process Area to be used in a hierarchical structure:

1.  Select **Elements \> Process Area** from the *Navigation* pane.

2.  Click **Add**.
    
    [View the field descriptions for the Process Area
    page](../Page_Desc/Process_Area)

3.  Enter a Process Area name in the **Process Area** field.
    
    **NOTE:** A Process Area name can be a maximum of 15 characters
    long.

4.  Enter a description of the Process Area in the **DESCRIPTION**
    field.

5.  Click **Save**.

The Process Area displays in the Process Area ID list box on the *[Wave
: Process Areas](../Page_Desc/Wave_Process_Areas)* page, and can be
assigned to a Wave to create a context.

A Process Area can also be added by copying an existing Process Area.
Refer to [Copy Elements](Copy_Elements) for more information.

**NOTE**: If a user is currently working in a context (i.e., that
context displays on the user’s Context bar), neither the Wave nor
Process Area in the context can be deleted.

Continue with Add an Object.

## <span id="Add3"></span>Add an Object

An <span style="font-style: italic;">Object</span> is a migration
object, and is assigned to a Wave-Process Area combination. Examples of
Objects include customers, basic materials, price lists or sales orders.

An Object can also have contacts and decisions and its history can be
tracked.

To add a migration object: 

1.  Select **Elements \> Object** from the *Navigation* pane.

2.  Click **Add**; the *Vertical* View displays.
    
    *[View the field descriptions for the Objects
    page](../Page_Desc/Objects_H)*

3.  Enter an object name in the **NAME** field.

4.  Enter an object description in the **DESCRIPTION** field.

5.  Enter a value in the **PRIORITY** field.
    
    **NOTE:** The value is the order the object displays on the
    *Objects* page’s *Horizontal* View.
    
    **NOTE: **When a Wave-Process Area uses the object, the object
    priority cascades down to Target Design. Once the target that
    belongs to the object is synced with Map, the priority is also
    available in Map and displays on the
    <span style="font-style: italic;">Objects</span> page. The priority
    is also used in Transform, but can be updated in Transform on the
    <span style="font-style: italic;">Targets</span> page to change the
    order the object is processed.

6.  Enter a **COMMENT** if necessary.

7.  Click **Save**.

The object displays in the **OBJECTID** list box on the *[Process Area:
Object](../Page_Desc/Process_Area_ObjectH)* page, and can be
assigned to a Process Area.

An object can also be added by copying an existing object. Refer to
[Copy Elements](Copy_Elements) for more information.

Once an object is added in Console, it can be viewed in Map and
Transform.  If the object is deleted in Console, it no longer displays
in Map and Transform. An object cannot be deleted if it is being used in
Map or Transform in a data migration project.

Continue with Add Elements to a Wave.

## <span id="Add4"></span>Add Elements to a Wave

Once the Process Area and object have been added, they can be assigned
to a Wave.

To add existing elements to a Wave:

1.  Click **Waves** on the *Navigation* pane.

2.  Click the **Process Areas** icon for a Wave.

3.  Click **Add**.
    
    *[View the field descriptions for the Wave: Process Areas
    page](../Page_Desc/Wave_Process_Areas)*

4.  Select a Process Area from the **Process Area ID** list box.
    
    Or
    
    Click the **+** icon to open the *[Process
    Area](../Page_Desc/Process_Area)* page to manually create a new
    Process Area ID. Refer to [Create the Context by Adding a Wave and
    Creating Elements](Add_a_Wave_and_Create_Elements) for more
    information.

5.  Click **Save**.

6.  Click the **Objects** icon for the Process Area.

7.  Click **Add**.
    
    [View the field descriptions for the Process Area: Object
    page](../Page_Desc/Process_Area_ObjectH)

8.  Select an object from the **OBJECT ID** list box.
    
    Or
    
    Click the **+** icon to open the
    *[Objects](../Page_Desc/Objects_H)* page to manually create a
    new OBJECT ID. Refer to [Create the Context by Adding a Wave and
    Creating Elements](Add_a_Wave_and_Create_Elements) for more
    information.

9.  Select a data source from the **DATA SOURCE ID** list box.
    
    **NOTE**: The DATA SOURCE ID is the data source where target tables
    and Target Source tables are registered

10. Click **Save**.
