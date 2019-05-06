# Create a Custom Assembly

A developer creates an assembly that is used by the Custom template when
posting.

To create the assembly:

1.  Create a new Class Library Project in Visual Studio targeting .NET
    Framework 4.0.

2.  Add the following project reference to the project:
    
      - CranSoft.DSP.Integrate.dll
      - CranBerry.Framework.dll
      - RAD.Common.dll

3.  Create a new class that implements the CranSoft.DSP.Integrate
    IProcessTemplate Interface and
     CranSoft.DSP.Integrate.CustomProcesstemplate. Right-click the
    IProcessTemplate Interface and select
    <span style="font-weight: bold;">Implement Interface</span>.

4.  Create a constructor that takes in a parameter of type
    CustomPostParameter. The CustomPostParameter has the properties
    “Host“ which is the Plugin Service host, and
     “IntegrateDataRowContract” which provides enough information to
    implement the execution of a custom template.
    
    **NOTE:** The constructor must call the base constructor and pass in
    the CustomPostParameter.Host.

5.  Add an implementation for each of the properties and methods of the
    Interface.

6.  Build Project.

7.  Take note of the full class name (Namespace + Class Name), for
    example, SampleProcessTemplate.SampleProcessTemplate.

8.  Take note of the assembly name that contains the
    CustomProcessTemplate class, for example SampleProcessTemplate.dll.

Continue with [Copy the Assembly File to the Integrate Process
Folder](Add_the_Assembly_File_to_the_Integrate_Process_Folder.htm).
