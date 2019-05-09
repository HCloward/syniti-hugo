# ISA CTS Overview

To move SAP Information Steward (IS) and SAP Information Steward
Accelerator (ISA) content between development tiers (environments), a
set of steps must be followed in the order specified due to the
interrelationships that exist between the data elements in the two
applications (Projects, Rules, Rule Bindings and other
elements).<span> </span>

The process is performed in:

  - SAP IS by a technical IS user
  - SAP ISA by a user familiar with ISA
  - SAP Central Management Console (CMC) by the Administrator of the CMC
    environment
  - Data Stewardship Platform (DSP)® by an Administrator or technical
    lead

Refer to the
[CTS](../../../Platform/Sys_Admin/Use_Cases/CTS_Overview) section in
System Administration for general information about CTS.

Before the promotion of the code to the target environment:

  - The client environment must be running ISA version 6.5.3 or later.
  - Both the source and target environment must be on the same version
    level.

Additionally, to move the data elements:

  - The user performing the code promotion must be familiar with both IS
    and the ISA.
  - The user must have knowledge of the CTS application used for the
    code promotion of the ISA. Refer to
    [CTS](../../../Platform/Sys_Admin/Use_Cases/CTS_Overview) in
    System Administration for more information.
  - The source environment must have been built out so that the IS and
    ISA configuration is aligned and able to be executed successfully
    for the IS Project that is to be promoted.
  - The source and target Collect environments must have been configured
    to point to the respective IS repository sources.

To CTS ISA objects:

1.  [Export IS Project Content in IS](#Export_IS_Project_Content_in_IS)

2.  [Create the CTS Package of ISA
    Content](#Create_the_CTS_Package_of_ISA_Content)

3.  [Create the CTS Package of
    Schedules](#Create_the_CTS_Package_of_Schedules)

4.  [Create the Target Environment Project and
    Connections](#Create_the_Target_Environment_Project_and_Connections)

5.  [Import the IS Project into the Target IS Environment in
    IS](#Import_the_IS_Project_into_the_Target_IS_Environment)

6.  [Create Users in the Target ISA
    Environment](#Create_Users_in_the_Target_ISA_Environment)

7.  [Align the IS Metadata Repository with
    ISA](#Align_the_IS_Metadata_Repository_with_ISA)

8.  [Run Tasks associated to the IS Project in
    IS](#Run_Tasks_Associated_with_the_IS_Project)

9.  [Import the CTS Package into the Target
    Environment](#Import_the_CTS_Package_of_ISA_Content_into_the_Target_Environment)

10. [Import the CTS Package of Schedules into the Target
    Environment](#Import_the_CTS_Schedules_Package_into_the_Target_Environment)

11. Open the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Project
    Summary</span> page to align the
metadata

## <span id="Export_IS_Project_Content_in_IS"></span>Export IS Project Content in IS

To export the project:

1.  Open the Information Steward Project to be promoted.

2.  Click the **Export project and associated objects** drop-down menu
    and select **Project** from the top right of the Workspace Home
    page.

3.  Export the Project contents and save to a zip file.
    
    **NOTE** Do not update the file name that is automatically generated
    by IS.

4.  Copy the .zip file to a directory that the Target IS environment can
    access.

## <span id="Create_the_CTS_Package_of_ISA_Content"></span>Create the CTS Package of ISA Content

To create the package:

1.  Select
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Admin
    \> CTS</span> in the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Navigation</span>
    pane.

2.  Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Add.</span>

3.  Enter a description in the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">DESCRIPTION</span>
    field.

4.  Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Save</span>.

5.  Enter a comment in the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Comments</span>
    field if necessary.

6.  Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Save</span>.

7.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Items</span>
    icon for the newly created CTS package.

8.  If no records exist, the page displays in add mode. Otherwise, click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Add</span>.
    
    **NOTE**: For each item added, there is a corresponding Project or
    Project Distribution being promoted. For example, if one Project
    that has two Project Distributions is being promoted, add three
    items, one Project and two Project Distribution records.
    
    **NOTE:**It is best practice to create one CTS Package for one
    Project.

9.  Select *dspMonitor\_AccPak – Project* from the **CTS CONFIG ITEM
    ID** list box.

10. Click **Save**.

11. Click **Save** on the *Vertical* View.

12. Select *dspMonitor\_AccPak – Project Distribution* from the **CTS
    CONFIG ITEM ID** list box.

13. Click **Save**.

14. Click **Save** on the *Vertical* View.

15. If no additional items need to be added, click **Cancel**.
    Otherwise, continue to add Project and Project Distributions.

16. Click the **Keys** icon for the Project record.

17. Click **Edit**.

18. Enter the name of the ISA/IS Project being promoted in the **VALUE**
    list box.
    
    **NOTE**: A list of available projects that match the entry display.

19. Select the project name from the list.

20. Click **Save**.

21. Click the back arrow on the browser to return to the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">CTS
    Items</span> page.

22. Click the **Keys** icon of a Project Distribution record.

23. Click **Edit**.

24. Enter the name of the ISA Project Distribution being promoted in the
    **VALUE** list box.
    
    **NOTE:** A list of available project distributions that match the
    entry display.

25. Select the project distribution name from the list.

26. Click **Save**.

27. Click the back arrow on the browser to return to the *CTS Items*
    page.

28. Continue adding Project Distribution keys until all of the Project
    Distributions have been included in the Project being promoted.

29. Click the back arrow to return to the *CTS Build* page.

30. Click the **Build Packing List** icon to build the packing list
    based on the keys entered; a confirmation message displays.

31. Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Ok</span>.

32. After the Packing List build is complete, click the **Build
    Archive** icon; a confirmation message displays.

33. Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">OK</span>.

34. Locate the archive file created in the \<installation
    folder\>\\Archives (e.g., C:\\Program Files
    (x86)\\BOA\\DSP\\Archives) and copy the file to the target
    environment into the same
location.

## <span id="Create_the_CTS_Package_of_Schedules"></span>Create the CTS Package of Schedules

To create the package:

1.  Select **Admin \> CTS** in the *Navigation* pane.

2.  Click **Add**.

3.  Enter a description in the **DESCRIPTION** field.

4.  Click **Save**.

5.  Enter a comment in the **Comments** field if necessary.

6.  Click **Save**.

7.  Click the **Items** icon for the newly created CTS Build.

8.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.
    
    **NOTE:** For each item added, there is a corresponding Schedule
    being promoted. If your ISA Project Distributions reference multiple
    Schedules then add multiple records to the CTS Archive
    
    **NOTE:** All Schedules can be added to a single CTS Archive.

9.  Select *DSPCommon - Schedule* from the **CTS CONFIG ITEM ID** list
    box.

10. Click **Save**.

11. Click **Save** on the *Vertical* View.

12. If no additional items need to be added, click **Cancel**.
    Otherwise, continue to add Schedules.

13. Click the **Keys** icon for the Schedules record.

14. Click **Edit**.

15. Enter the name of the Schedule being promoted in the **VALUE** list
    box.
    
    **NOTE:** A list of available Schedules that match the entry
    display.

16. Select the Schedule name from the list.

17. Click **Save**.

18. Click the back arrow on the browser to return to the
    <span data-xmlns="http://www.w3.org/1999/xhtml">*CTS Items*</span>
    page.

19. Continue adding Schedule keys until all of the Schedules have been
    included in the ISA Content being promoted.

20. Click the back arrow to return to the *CTS Build* page.

21. Click the **Build Packing List** icon to build the packing list
    based on the keys entered; a confirmation message displays.

22. Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Ok</span>.

23. After the Packing List build is complete, click the **Build
    Archive** icon; a confirmation message displays.

24. Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">OK</span>.

25. Once the archive build is complete, the **DATE CREATED** is updated
    and the **LOG** should not show any entries.

26. Locate the archive file created in the \<installation folder\>
    \\Archives (e.g., C:\\Program Files (x86)\\BOA\\DSP\\Archives) and
    copy the file to the target environment into the same
location.

## <span id="Create_the_Target_Environment_Project_and_Connections"></span>Create the Target Environment Project and Connections

**NOTE**: Confirm the names of the Project and connections from the
source instance. These must be entered exactly when creating the project
and connections in the CMC.

To create the target project and source connections in CMC.

1.  Log on to the Central Management Console.

2.  Navigate to the Information Steward area.

3.  Right-click **Manage** and choose **New \> Data Insight Project**.

4.  Enter the name of the Project in the ISA source environment in the
    DSP®.
    
    **NOTE:** The name must match the Project name in the ISA’s source
    instance or the import process will fail to align the source and
    target environments.

<!-- end list -->

1.  Enter a description.
    
    **NOTE:** The description is required.

2.  Click **Save**.

3.  Right-click **Manage** and choose **New \> Connection**.

4.  Enter the connection details to the ISFailedData database on the
    DSP® database server, again ensuring that the name of the
    connection matches the name of the source environment IS failed data
    database.

5.  Right-click **Manage** and choose **New \> Connection**.

6.  Enter the connection details to any other connections required by
    the IS project being exported. Ensure that the name of the
    connections is identical to the name used in the source environment.

7.  Test all of the connections to ensure they connect to the target
    database environment
correctly.

## <span id="Import_the_IS_Project_into_the_Target_IS_Environment"></span>Import the IS Project into the Target IS Environment

The next step in the CTS process for ISA is to import the file that was
exported in IS. .

To import the IS Project content from the source to the target:

1.  Open the Information Steward Project that is being promoted into on
    the target environment.

2.  Click the **Import project and associated objects** button on the
    Workspace Home window.

3.  Click the **Browse** button next to the **Import ZIP file path**
    field on the Import window.

4.  Select the IS export file created in the source environment.

5.  Select the check box to overwrite existing objects.

6.  Select the check box to automatically approve imported rules.
    
    **NOTE:** This step is optional.

7.  Select Select Administrators from the list box with the value
    **Select Default Observer**.

8.  Click **Next**.

9.  Map the connections contained in the Export file to the connections
    created in the target environment.

10. Click **Import**.
    
    **NOTE:** If there are errors during the import that cannot be
    resolved, contact SAP support.

11. Click **Close**.

12. Click
**Finish**.

## <span id="Create_Users_in_the_Target_ISA_Environment"></span>Create Users in the Target ISA Environment

In the CTS process for ISA, the target environment must be set up with
the user accounts required to support the ISA Project Distributions. If
these user accounts do not exist in the target environment, they must be
added by an Administrator user. Refer to [Create User
Accounts](../../../Platform/Sys_Admin/Use_Cases/Create_User_Accounts_in_System_Administration)
in System Administration for more information.

If user accounts that are assigned to ISA Project Distributions in the
source environment are not present in the target environment, then those
users will be automatically removed from the Project Distributions on
import to the target
environment.

## <span id="Align_the_IS_Metadata_Repository_with_ISA"></span>Align the IS Metadata Repository with ISA

To run the Collect process that aligns the metadata:

1.  Select **Collect** in the *Navigation* pane.
2.  Select the **dgRepository\_IS Target** record.
3.  Select the ISSAP Target Source on the *[Target
    Sources](../../../Platform/Collect/Page_Desc/Target_Sources_H_Collect)*
    page.
4.  Click the Refresh icon to pull the latest metadata from IS into the
    ISA repository.

**NOTE:** If this is the first execution in the Target environment then
a Build is required prior to the Refresh. Click the Build and Refresh
icon.

**NOTE**: The Refresh must be successfully completed for all tables in
the Collect ISSAP
package.

## <span id="Run_Tasks_Associated_with_the_IS_Project"></span>Run Tasks Associated with the IS Project

To run tasks associated with the IS project:

1.  Open the Information Steward Data Insight Project that has been
    promoted into on the target environment.
2.  Click the **Tasks** tab on the left side of the window.
3.  Select each of the Tasks and click the **Run Now** button.

<span style="font-weight: bold;">NOTE</span>:To ensure that the Tasks
are pointing to the correct Failed Data Connection, click the
<span style="font-weight: bold;">Edit</span> button to view the Task
properties.

## <span id="Import_the_CTS_Package_of_ISA_Content_into_the_Target_Environment"></span>Import the CTS Package of ISA Content into the Target Environment

Additionally, the CTS package created on the source system must be
transferred to the following directory on the target ISA
environment: \<installation folder\> \\Archives e.g. C:\\Program Files
(x86)\\BOA\\DSP\\Archives.

To import the CTS package:

1.  Select **Admin \> CTS\> Archives** in the *Navigation* pane.
2.  Click the **Detect Archives** icon.
3.  Refresh the Archives page until the CTS Archive created in the
    source environment displays.
4.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Install</span>
    icon for the CTS package containing the ISA content.
5.  Wait for the installation process to complete and check the Log to
    ensure correct import execution has
occurred.

## <span id="Import_the_CTS_Schedules_Package_into_the_Target_Environment"></span>Import the CTS Schedules Package into the Target Environment

Additionally, the CTS package created on the source system must be
transferred to the following directory on the target ISA
environment:<span> </span> \<installation folder\> \\Archives e.g.
C:\\Program Files (x86)\\BOA\\DSP\\Archives

To import the package:

1.  Select **Admin \> CTS\> Archives** in the *Navigation* pane.
2.  Click the **Detect Archives** icon.
3.  Refresh the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Archives</span>
    page until the CTS Archive created in the source environment
    displays.
4.  Click the **Install** icon for the CTS package containing the
    Schedules.
5.  Wait for the installation process to complete and check the Log to
    ensure correct import execution has
occurred.

## <span id="Open_the_Project_Summary_Page_to_Align_the_Metadata"></span>Open the *Project Summary* Page to Align the Metadata

The final step in the CTS process for ISA is to access the
<span style="font-style: italic;">[Project
Summary](../Page_Desc/Project_Summary_H)</span> page.

To complete the CTS process for ISA:

1.  Click **Information Steward Accelerator \> Project Summary** in the
    *Navigation* pane.
    
    **NOTE**: This triggers the alignment process stored procedure that
    runs on loading the project summary.

2.  Review the Project / Project Distribution details to ensure they are
    aligned with the source ISA environment as expected.
