+++
title = 'CTS Notes Specific to dspConduct™'
solution = 'Master Data Management'
+++

# CTS Notes Specific to dspConduct™

When creating CTS archives to support dspConduct™ objects, if any
objects included in any Packing List reside in a data source/database
that does not exist on the target system, manually create that database
in the target system before the archive can be successfully imported
into the target. The WebApp for the objects should also already exist on
the target system.

This use case includes the following topics:

  - [Shippable Items in Detail](#Shippable_Items_in_Detail)
  - [Supporting Objects for Categories and
    Scenarios](#Supporting_Objects_for_Categories_and_Scenarios)
  - [Include Content Application DSP® Pages Listed on the Task Page
    Page](#Including_Content_Application_DSP_Pages_Listed_on_the_Task_Page)

## <span id="Shippable_Items_in_Detail"></span>Shippable Items in Detail

The dspConduct™ Shippable Items are:

  - 1.Category - Ships the complete Category including all Business
    Process, Scenarios, Roles and Tasks under the Category. The Items
    Key is the CategoryID, which can be selected by the Name of the
    Category.
  - 2.Business Processes - Ships the complete Business Process,
    including Scenarios, Roles and Tasks under the Category. The object
    keys are the CategoryID (as described under Category) and the
    BusinessProcessID selected by the Business Process Name.
  - 3.Scenarios - Ships the complete Scenario, including Roles and Tasks
    under the Category. The object keys are the CategoryID (as described
    under Category) and the ScenarioID selected by the Scenario Name.

**NOTE**: Integrate Processes assigned to the Scenario are first
registered for the Category. A new Integrate Process created for a
scenario wil require that the Category registrations exist on the Target
first. Create a separate CTS for the Category. After the Packing List is
built, exclude all items except the dspConduct - 1.Category Item.

  - 4.Roles - Ships the Role, including Tasks under the Category. The
    object keys are the CategoryID (as described under Category) and the
    RoleID selected by the Role Name.
  - 5.Tasks - Ships the Task, including the DSP® registrations and SQL
    objects used for the Content App page that makes up the top level
    task. The object keys are the CategoryID (as described under
    Category) and the TaskID, selected by the Task’s top level Page
    Name.

**NOTE**: If you plan on including the SQL objects, ensure that all of
the necessary SQL objects are included in the CTS or already exist on
the Target system.

  - 6.Org Units - Ships the Org Unit registrations found under
    dspConduct™ \> Configuration \> Org Units. Key is the OrgUnitID,
    selected by the name of the Org Unit. This only ships the
    registration, ensure that the Org Unit List Source exists on the
    Target system in the database shown as the List Data Source ID.
  - 7.Positions - Ships the Position registrations found under
    dspConduct™ \> Security. Key is the PositionID which can be selected
    by the Position Name.
  - Org Unit Groups - Ships the Org Unit Group registrations found under
    dspConduct™ \> Configuration \> Org Unit Groups. Key is the Org Unit
    Group Name. This requires that the Org Unit registration exists on
    the Target system.
  - Workflow Defaults - Ships the Workflow Default values found under
    dspConduct™ \> Configuration \> Workflow Message Defaults. Key is
    the Event name. Note that the Language Specific Workflows configured
    under Design \> Category \> Vertical \> Workflow Messages are
    shipped with the
Category.

## <span id="Supporting_Objects_for_Categories_and_Scenarios"></span>Supporting Objects for Categories and Scenarios

Supporting objects for templates reside in other data sources than
dspConduct™. The following Integrate objects need to also be included in
a CTS archive:

  - **Integrate Category** - Integrate Processes are registered to a
    dspConduct™ Category and then assigned to Scenarios. The list of
    Integrate Processes can be found on the *[Category
    Process](../Page_Desc/Category_Process)* page. On this page,
    Integrate Processes are listed as Integrate Category : Integrate
    Process.

**NOTE**: Any Integrate Category with Processes used by a dspConduct™
Category should be transferred to the Target system before attempting to
move the dspConduct™ Objects. Be aware that a Packing List that includes
an Integrate Category automatically includes all templates and all
processes in Integrate. Exclude any other templates and processes that
should not be included.

  - **Integrate Process** - On the dspConduct™ on the *[Category
    Process](../Page_Desc/Category_Process)* page determine the
    Integrate Process ID. Build a CTS; select Type of Integrate –
    Integrate Process and enter the Key Value associated with the
    Integrate Process ID. Export to the target system; Import into the
    target system.
  - **Integrate Template** - On the Integrate *[Process
    Templates](../../../Platform/Integrate/Page_Desc/Process_Templates_H)*
    page , determine the Integrate Template ID. Build a CTS; select Type
    of Integrate – Integrate Template and enter the Key Value associated
    with the Integrate Template ID. Export to the target system; Import
    into the target
system.

## <span id="Including_Content_Application_DSP_Pages_Listed_on_the_Task_Page"></span>Including Content Application DSP® Pages Listed on the Task Page

When CTSing a Task, you may want to include all the DSP® pages listed on
the [Task Page](../Page_Desc/Task_Page_H) page in dspConduct™ in the
Packing List.

To include DSP® pages in the CTS:

1.  Create a CTS package that contains a CTS Item for each page and add
    CTS Item Keys. Refer to [Create a CTS Package and Build Archive in
    Source
    Instance](../../../Platform/Sys_Admin/Use_Cases/CreatePckgeBuildArcSrceInstance)
    in System Administration for detailed information.
    
    **NOTE**: When adding CTS Items to the package, select
    **CranSoft-Page** from **CTS CONFIG ITEM ID** list box.:
    
    **NOTE**: When adding the CTS Item Keys for the Items, select the
    WebApp where the page resides from **Value** list box for WebApp ID
    Name. Type the first letters of the page name (e.g., If page is
    named “Request (General),” type “Req”) in the Value combo box for
    Page ID Name and choose one of the pages that has been created on
    the source for the template.

2.  Click **Build Packing List** button.

3.  Click **Packing List** to review what is included. Compare this list
    to the Pages on the *[Task Page](../Page_Desc/Task_Page_H)*
    page.
    
    **NOTE**: Views associated with the pages added in step \#1 are
    automatically included in the Packing List.
    
    **NOTE**: Additional SQL objects may need to be migrated to the
    Target system. This could include Tables, Views and Stored
    Procedures registered to the Content WebApp pages.

4.  Create a separate CTS package for any additional SQL objects.

5.  Import all archives for the dspConduct™ item to the target system.

6.  Recompile objects for the dspConduct™ data source and any other data
    sources affected by the imports (within System Administration, on
    the [Data
    Sources](../../../Platform/Sys_Admin/Page_Desc/Data_Sources_HSysAdmi)
    page, select the DATA SOURCE NAME and click **Recompile Objects**).
    
    **NOTE**: The recompile objects process detects any missing SQL
    objects.
