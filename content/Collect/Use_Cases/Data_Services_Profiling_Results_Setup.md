# Data Services Profiling Results Setup

This section contains the following topics:

  - [Register the Target and Target
    Source](#Register_the_Target_and_Target_Source)
  - [Add Tables to the Target and Target
    Source](#Add_Tables_to_the_Target_and_Target_Source)
  - [Schedule the Target to
Download](#Schedule_the_Target_to_Download)

## <span id="Register_the_Target_and_Target_Source"></span>Register the Target and Target Source

To register the target and Target Source:

1.  Register the Target (Refer to [Register
    Targets](Register_and_Use_Targets.htm#Register_Targets) in Collect
    for detailed information).
2.  Register the Target Source to the Target. (Refer to [Register
    Sources to
    Target](Register_and_Use_Sources.htm#Register_Sources_to_Target) in
    Collect for detailed information).

**NOTE:** The connection between the Target and the Target Source should
be tested. (Refer to[Test Target
Connection](Register_and_Use_Targets.htm#Test_Target_Connection) and
[Test Source
Connection](Register_and_Use_Sources.htm#Test_Source_Connection) in
Collect for detailed
information.)

## <span id="Add_Tables_to_the_Target_and_Target_Source"></span>Add Tables to the Target and Target Source

To add tables to the target and Target Source:

1.  Select **Targets** from the *Navigation* pane.

2.  Click **Tables** for the SOURCE.

3.  Click **Add**.
    
    [View the field descriptions for the Table’s page Vertical
    View.](../Page_Desc/Tables_H.htm#Tables_V_All_Tabs)

4.  Enter the **TABLE** name.

5.  Click **Save**.

6.  Add additional tables as required.

7.  Select all newly added tables.

8.  Click **Build and Refresh**.
    
    **NOTE:** A package build is immediately scheduled if no package
    exists and then a refresh is performed for this table.

9.  Click **Ok**.

**NOTE:** If the build and refresh is successful, a Job Complete;
Submitted message displays. If it fails, investigate the connection
details.

## <span id="Schedule_the_Target_to_Download"></span>Schedule the Target to Download

To schedule the target to download:

1.  Schedule the Target to download. (Refer to [Set up Schedule
    Groups](../Config/Set_Up_Schedule_Groups.htm) in Collect for more
    information).
2.  The profiling results can be viewed once the download is complete.
