+++
title = 'Create a CTS Package and Build Archive in Source Instance'
solution = 'Platform'
+++

# Create a CTS Package and Build Archive in Source Instance

A package is the record and configuration created on the CTS pages in
the DSP®. An *archive* is built from a package and is the actual item(s)
and configurations moved via the CTS process.

The CTS Configuration for DSP WebApps is included by default and must
not be updated on the CTS Configure pages.

The CTS Configuration for custom WebApps must be created before objects
can be moved via the CTS process. Refer to [Set a Baseline Configuration
for a Custom
WebApp](Set%20a%20Baseline%20CTS%20Configuration%20for%20a%20Custom%20WebApp).

To create a CTS package and build an archive for a delivered WebApp:

1.  Log in to the DSP® source instance.

2.  Select **Admin \> CTS \> Build** in the *Navigation* pane.

3.  Click **Add**.
    
    *[View the field descriptions for the CTS Build
    page](../Page_Desc/CTS_Build_H)*

4.  Enter a unique name for the CTS package in the **DESCRIPTION**
    field.
    
    **NOTE:** Since the CTS process for all applications on the system
    is managed within the System Administration Component, it is
    recommended to include the name of the component (for example,
    Collect) in the description to easily identify the application(s)
    relevant to the contents of an archive once it is created. **As a
    best practice, create one package per component.**

5.  Click **Save**; the *Vertical* View displays.

6.  Verify the **Include Objects** check box is checked.
    
    **NOTE:** If checked, objects added on the
    [<span style="font-style: italic;">CTS Configure (SQL Object
    Registrations)</span>](../Page_Desc/CTS%20Configure%20SQL%20Object%20Registrations)
    page are included in the package.

7.  Click the **Show Hidden Items** check box to check it.
    
    **NOTE:** If checked, CTS items defined as “hidden” (CTS \>
    Configuration \> Shippable Items \> Vertical View) are visible in
    the packing list.

8.  Enter additional documentation in the **Comments** field, for
    example, a description of what the package contains.

9.  Select a value from the **Trace Level** list box. The default value
    is <span style="font-style: italic;">Warning</span>. Values are:
    
      - **Debug —** A detailed message displays to provide data about
        the process.
      - **Message —** An information message displays to mark a landmark
        in the code.
      - **Warning —** A message displays to inform the user that a
        problem could surface.
      - **Error —** An error message displays while the process is
        executing; processing can continue.
    
    **NOTE:** The Trace Level indicates the amount or level of detail of
    information that is provided in the log (which is accessed by
    clicking the **Log** icon on the *[CTS
    Build](../Page_Desc/CTS_Build_H)* page's
    <span style="font-style: italic;">Horizontal View</span>) if an
    error occurs when building the packing list and the archive. The
    order of details provided is Error, Warning, Message and Debug,
    where Error provides the least amount of information and Debug
    provides the greatest amount of information.

10. Click **Save**.

11. Click **Items** on the *Horizontal View* to specify the item(s) to
    include in the package.

12. Click **Add**. If no records exist, the page automatically opens in
    add mode.
    
    [View the field descriptions for the CTS Items
    page](../Page_Desc/CTS_Items_H)

13. Select an item to include in the package from the **CTS CONFIG ITEM
    ID** list box.
    
    **NOTE:** To move the wave initially, select **Console – Wave** from
    this list box, then select the wave’s key on the *[CTS Item
    Keys](../Page_Desc/CTS_Item_Keys)* page.
    
    **NOTE:** The CTS CONFIG ITEM ID list box displays every item
    available to be moved via the CTS process for every component.
    
    **NOTE:** Items in this list box display with the following names:
    
      - DataGarage refers to Collect objects
      - DSW refers to Transform objects
      - DataDialysis refers to dspMonitor™ objects
      - DSPCommon refers to Common objects
      - CranSoft refers to platform objects
    
    Use the following table to add the pre-defined items from the CTS
    CONFIG ITEM ID list box to the CTS package for each application.
    
    **NOTE:** The transport of SQL Inline Table-Valued functions is not
    supported.
    
    **NOTE:** Follow the order in which the applications are listed in
    this table when adding applications and items.
    
    <table>
    <tbody>
    <tr class="odd">
    <td><p>Application</p></td>
    <td><p>Items to add to the CTS package</p></td>
    </tr>
    <tr class="even">
    <td><p>Common</p></td>
    <td><p>DSPCommon — dspCommon System Type</p>
    <p>DSPCommon — Common System Type Table</p>
    <p>DSPCommon — Common System Type Group</p>
    <p>DSPCommon — Common System Type Table Index</p>
    <p>DSPCommon — Schedule</p>
    <p>DSPCommon — Common Automation Instructions</p>
    <p>DSPCommon — Common Automation Instruction Task</p>
    <p>DSPCommon — Common Automation Instruction Task Group</p>
    <p>DSPCommon — Common Automation Engine Action</p></td>
    </tr>
    <tr class="odd">
    <td><p>Collect</p></td>
    <td><p>DataGarage — Collect Target</p>
    <p>DataGarage — Collect – Target Source</p>
    <p>DataGarage — Target Source Table</p>
    <p>DataGarage — Target Source Table Rule</p>
    <p>DataGarage — Target Source Table Index</p></td>
    </tr>
    <tr class="even">
    <td><p>Console</p></td>
    <td><p>Console — Field Group</p>
    <p>Console — Metric Group</p>
    <p>Console — Process Area</p>
    <p>Console — Object</p>
    <p>Console — Target</p>
    <p>Console — Source</p>
    <p>Console — Wave</p>
    <p>Console — Wave Process Area</p>
    <p>Console — Wave Process Area Object</p>
    <p>Console — Wave Process Area Object Target</p>
    <p>Console — Wave Process Area Object Target Source</p>
    <p>Console — Execution Stage</p>
    <p>Console — Complex Rule</p>
    <p>Console — Simple Rule</p>
    <p>Console — Rule Condition</p>
    <p>Console — Target Lookup Table</p></td>
    </tr>
    <tr class="odd">
    <td><p>Map</p></td>
    <td><p>cMap — Wave Process Area Object</p>
    <p>cMap — Value Mapping Check Table</p>
    <p>cMap — Wave Process Area Object Target</p></td>
    </tr>
    <tr class="even">
    <td><p>ISA</p></td>
    <td><p>dspMonitor_AccPak — Project</p>
    <p>dspMonitor_AccPak — Project Distribution</p></td>
    </tr>
    <tr class="odd">
    <td><p>Assemble</p></td>
    <td><p>CranPort Packages</p></td>
    </tr>
    <tr class="even">
    <td><p>Automate</p></td>
    <td><p>InterfaceServer — File Operation</p>
    <p>InterfaceServer — Interface</p>
    <p>InterfaceServer — Logical Path</p></td>
    </tr>
    <tr class="odd">
    <td><p>dspCompose™</p></td>
    <td><p>dspCompose — Team</p>
    <p>dspCompose — OrgUnits</p>
    <p>dspCompose — Roles</p>
    <p>dspCompose — dspCompose Template</p></td>
    </tr>
    <tr class="even">
    <td><p>dspMonitor™</p></td>
    <td><p>DataDialysis — Group</p>
    <p>DataDialysis — Object</p>
    <p>DataDialysis — Report Repository</p>
    <p>DataDialysis — Report</p>
    <p>DataDialysis — Filter</p></td>
    </tr>
    <tr class="odd">
    <td><p>Integrate</p></td>
    <td><p>Integrate — Integrate Category</p>
    <p>Integrate — Integrate Template</p>
    <p>Integrate — Integrate Process</p>
    <p>Integrate — Integrate Process Template Connection</p></td>
    </tr>
    <tr class="even">
    <td><p><span>Transform</span></p></td>
    <td><p>DSW — Object</p>
    <p>DSW — Target</p>
    <p>DSW — Target Report</p>
    <p>DSW — Target Rule</p>
    <p>DSW — Target Export</p>
    <p>DSW — Target Data Services Report</p>
    <p>DSW — Target Data Services Rule</p>
    <p>DSW — Target Source</p>
    <p>DSW — Target Source Report</p>
    <p>DSW — Target Source Rule</p></td>
    </tr>
    <tr class="odd">
    <td><p>dspConduct™</p></td>
    <td><p>dspConduct — 1.Category</p>
    <p>dspConduct — 2.Business Processes</p>
    <p>dspConduct — 3.Scenarios</p>
    <p>dspConduct — 4.Roles</p>
    <p>dspConduct — 5.Tasks</p>
    <p>dspConduct — 6.Org Units</p>
    <p>dspConduct — 7.Positions</p>
    <p>dspConduct — Org Unit Groups</p>
    <p>dspConduct — Workflow Defaults</p></td>
    </tr>
    <tr class="even">
    <td><p>Platform</p></td>
    <td><p>CranSoft — Archive</p>
    <p>CranSoft — Audit</p>
    <p>CranSoft — Catalog</p>
    <p>CranSoft — Color</p>
    <p>CranSoft — CTS Configuration</p>
    <p>CranSoft — Data</p>
    <p>CranSoft — Data Source</p>
    <p>CranSoft — Database Type</p>
    <p>CranSoft — Dictionary</p>
    <p>CranSoft — File</p>
    <p>CranSoft — Folder</p>
    <p>CranSoft — Group</p>
    <p>CranSoft — Image</p>
    <p>CranSoft — Language</p>
    <p>CranSoft — Layout</p>
    <p>CranSoft — Menu</p>
    <p>CranSoft — Message Types</p>
    <p>CranSoft — Page</p>
    <p>CranSoft — Page Column Property</p>
    <p>CranSoft — Page Event</p>
    <p>CranSoft — Plugin</p>
    <p>CranSoft — Queue</p>
    <p>CranSoft — Search</p>
    <p>CranSoft — Security Definition</p>
    <p>CranSoft — Security Role</p>
    <p>CranSoft — SQL Object</p>
    <p>CranSoft — SQL Script</p>
    <p>CranSoft — Stop Word List</p>
    <p>CranSoft — Style</p>
    <p>CranSoft — Translation</p>
    <p>CranSoft — WebApp</p></td>
    </tr>
    </tbody>
    </table>

14. Update the **Include** check box if the default value is not
    applicable.
    
    **NOTE:** If checked, the relevant item is included when the packing
    list is built. If unchecked, the item is ignored when the packing
    list is built. Default value is enabled.

15. Click **Save**; the *Vertical* view displays.
    
    [View the field descriptions for the CTS Items page's Vertical
    View](../Page_Desc/CTS_Items_H)

16. Update the **Purge** check box if the default value is not
    applicable.
    
    **NOTE:** If checked, any child items related to the item that had
    Purge enabled are deleted when the archive is installed.

17. Click **Save**.

18. Add additional items from the **CTS CONFIG ITEM ID** list box or
    click **Cancel** to configure keys for the items.

19. Click the **Keys** icon for the <span style="font-weight: bold;">CTS
    CONFIG ITEM ID</span>.
    
    **NOTE:** All required keys for the item display. Multiple keys may
    display, depending on the type of item included in the package. The
    keys required for each item are set in the CTS Configuration.

20. Click **Edit** for the key.
    
    [View the field descriptions for the CTS Item Keys
    page](../Page_Desc/CTS_Item_Keys)

21. Select the specific item from the **VALUE** combo box.

22. Click **Save**.
    
    **NOTE:** Each specific item included in the package has to be added
    individually to the <span style="font-style: italic;">[CTS
    Items](../Page_Desc/CTS_Items_H)</span> page. There is no
    process to add all items to a CTS package.

23. Click **Build** in the *Navigation* pane.

24. Click the **Build Packing List** icon to create a list of items and
    dependencies to include in the package; a confirmation message
    displays.

25. Click **OK**.

26. Click **Log** to view any messages or errors.

Continue with [Add Attributes](Add_Attributes) (optional) or [Review
Packing List to Exclude Specific
Items](Review_Packing_List_to_Exclude_Specific_Items).
