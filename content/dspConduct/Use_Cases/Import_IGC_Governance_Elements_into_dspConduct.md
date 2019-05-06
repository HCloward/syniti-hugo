# Import IGC™ Governance Elements into dspConduct™

Business processes built and published in the Information Governance
Cloud™ (IGC™) can be imported into dspConduct™ to create an on premises
instance of these elements. On import, the category, business process,
scenario, role, and task records are registered in dspConduct™.

**NOTE**: Data entered in IGC™ and imported into dspConduct™ cannot be
updated in dspConduct™. Records cannot be deleted, and elements cannot
be activated or deactivated. Some settings that are not set in IGC™ can
be updated for IGC™ elements in dspConduct™. Refer to [Update Custom
Attributes for Governance
Elements](Update_Custom_Attributes_for_Governance_Elements.htm) for more
information.

After tasks are published in IGC™, they are imported into dspConduct™
via a service page that runs every 30 minutes. A user with security can
access the *Services Pages* page in System Administration (Admin \>
Resources \> Service Pages) to change the service page schedule as
needed or to manually run the service page to import tasks immediately.
Refer to [Start and Stop Service
Pages](../../../Platform/Sys_Admin/Use_Cases/Stop_and_Start_Service_Pages.htm)
in System Administration for more information.

If a category is added in IGC™, a WebApp must exist that can be assigned
to the category.

**NOTE**: If the required WebApp does not display in the list box, it
must be added. Refer to System Administration for more information about
[adding a
WebApp](../../../Platform/WebApp_Dev/Create_a_WebApp_in_DSP.htm) and
[registering a data
source](../../../Platform/Sys_Admin/Use_Cases/Register_a_Data_Source.htm).

If tasks were added in IGC™, the Process Designer must assign an
existing dspConduct™ task to it or must create a new task in dspConduct™
to assign to the IGC™ task.

**NOTE**: When IGC™ is installed, connection parameters to IGC™ are
configured in Common. The **From IGC** icon does not display on
dspConduct™ pages until these parameters are configured. Refer to the
*BackOffice Associates® Installation and Upgrade Manual* for more
information.

When importing governance elements into dspConduct™:

  - When importing a category from IGC™, if there is a category in
    dspConduct™ that has the same name, the IGC™ category is
    automatically mapped to the dspConduct™ category. If more than one
    dspConduct™ category has the same name in the database, the IGC™
    category is mapped to the category with the earliest Added On date.
    All business processes, scenarios and roles coming from the IGC™ are
    created as new elements in the matched category. A process Designer
    must then map dspConduct™ tasks to the IGC™ tasks.
  - When a Post role is imported into dspConduct™, if the role has no
    IGC™ tasks assigned to it, one dspConduct™ generic Post task is
    created for the Post role. Additionally, other Post tasks cannot be
    mapped to Post roles that are imported from IGC™.
  - If an IGC™ task has been imported into dspConduct™, and the task is
    then renamed in IGC™ and republished, the task name is updated in
    dspConduct™.
  - If a scenario, role or task is deleted in IGC™ and the business
    process is republished, the items deleted in IGC™ are removed from
    dspConduct™ after the import.

**NOTE**: When an IGC™ business process is imported into dspConduct™,
the business process, scenario and role dependencies are also imported.

**NOTE**: Category owners are maintained in IGC™ but are not imported in
dspConduct™. This required field must be maintained in dspConduct™.
Refer to [Set Up a Category from IGC™ in
dspConduct™](Set_Up_a_Category_from_IGC_in_dspConduct.htm) for more
information.

**NOTE**: When a role is imported from IGC™ and the SLA fields are blank
in dspConduct™ at the scenario role level and the business process
scenario role level, the values entered in IGC™ are used. If the fields
already contain values in dspConduct™, the SLA values are **NOT**
updated at these levels. At the role level, when a role is imported from
IGC™, the SLA values are updated whether the fields have values in
dspConduct™ or not.

After data has been imported into dspConduct™:

  - [Set Up a Category added in IGC™ in
    dspConduct™](Set_Up_a_Category_from_IGC_in_dspConduct.htm), if
    needed
  - [View Tasks Imported from IGC™ in
    dspConduct™](View_Tasks_Imported_from_IGC_in_dspConduct.htm)
  - [Map a dspConduct™ Task to a Task Imported from
    IGC™](Map_a_dspConduct_Task_to_a_Task_Imported_from_IGC.htm)
  - [Update Custom Attributes for Governance
    Elements](Update_Custom_Attributes_for_Governance_Elements.htm), if
    needed
