+++
title = 'Display Data Services Profiling Results'
solution = 'Platform'
+++

# Display Data Services Profiling Results

SAP Data Services has the capability to Profile data in Source or Target
data sources, including databases, application and files. The profiling
results are stored in a Profiler repository and can be shared among the
Data Services developers via the Data Services Designer application. To
expose these results to the wider data migration and governance
audience, BackOffice Associates® has included the ability to view the
results from any Data Services column profiling process within the DSP®.

Data Services profiling will read through the data in any specified file
or table and will look for information about the data values in the
columns. The results of the profiling exercise would include, but not
limited to; minimum value, maximum value, number of null values, maximum
string length, distinct patterns in the data, etc. This information is
very useful when assessing the data quality of a system and its ability
to support the required business process. The profiling results could be
used to assess data for a data migration, data governance or interfacing
project.

The following are prerequisites to displaying Data Services profiling
results in the DSP and are performed by a DS developer (or
Administrator):

  - Setup a repository for profiling
  - Register that Profiler repository in the CMC and against the Data
    Services Job Server
  - Assign the Profiler repository to the specific Data Services local
    repositories that the developers will use
  - Add the tables or files to a Datastore in Data Services that are to
    be profiled
  - Perform the profiling actions in Data Services
  - Run the collect process via a build and refresh option (Refer to
    [Build Package
    Overview](../../Collect/Use_Cases/Build_Package_Overview.htm) and
    [Build Package for
    Source](../../Collect/Use_Cases/Register_and_Use_Sources.htm#Build_Package_for_Source)
    in Collect for detailed information).

 

To display and view the Data Service Profiling Results:

1.  [Import the Data Services Profiling Results into the
    DSP](../../Sys_Admin/Use_Cases/Import_the_Data_Services_Profiling_Results_into_the_DSP.htm)
    (performed by an Administrator)
2.  [Register the Target and Target
    Source](../../Collect/Use_Cases/Data_Services_Profiling_Results_Setup.htm#Register_the_Target_and_Target_Source)
3.  [Add Tables to the Target and Target
    Source](../../Collect/Use_Cases/Data_Services_Profiling_Results_Setup.htm#Add_Tables_to_the_Target_and_Target_Source)
4.  [Schedule the Target to
    Download](../../Collect/Use_Cases/Data_Services_Profiling_Results_Setup.htm#Schedule_the_Target_to_Download)
5.  [View the Profiling Results](View_the_Profiling_Results.htm)
