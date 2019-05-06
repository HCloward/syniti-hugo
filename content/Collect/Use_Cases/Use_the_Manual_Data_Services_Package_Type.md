# Use the Manual Data Services Package Type

Use this package type to use advanced features within Data Services
Jobs, for example change data capture.

Prior to adding this package type configure the connection information
used by SAP Data Services at the Target Source level. Refer to
[Configure Source for SAP Data
Services](Register_and_Use_Sources.htm#Configure_Source_for_SAP_Data_Services)
for more information.

To use the package type:

1.  Create the job, dataflow, source, transformation and target in SAP
    Data Services.

**NOTE:** Use the naming conventions for Collect listed in Common.
Select <span style="font-weight: bold;">Common \> Configuration \>
Modules \> Collect \> Parameters – Collect \> Click Data Services
Settings tab</span>. Use the naming conversion in the table below.

 

Download Job Settings

Download Job Name Format

Displays name format for the job that executed a download of source
table to a target table. Default value is
**\#SOURCE\#\_\#TARGET\#\_\#SOURCETABLE\#\_imp**.

Download Job Data Flow Name Format

Displays the format for the Data Flow object in a Download job. Default
value is **DF\_\#SOURCE\#\_\#TARGET\#\_\#SOURCETABLE\#**.

Download Job Source Table Data Flow Display Name Format

Displays the format for the source table display name in a Data Flow
object of a Download job. Default value is
**\#SOURCETABLE\#\_\#SOURCE\#**.

Download Job Target Table Data Flow Display Name Format

Displays the format for the target table display name in a Data Flow
object of a Download job. Default value is
**\#TARGETTABLE\#\_\#TARGET\#**.

Download Job Source Table Description Format

Displays the format of the source table description in a Download job.
Default value is **\#SOURCETABLE\# table from \#SOURCE\#**.

Download Job Target Table Description Format

Displays the format of the target table description in a Download job.
Default value is **\#TARGETTABLE\# table from \#TARGET\#**.

Download Job Schema Name Format

Displays the format of the Schema Name object in a Download job. Default
value is **TFM\_\#TARGETTABLE\#**.

1.  Add a table to the Source. Refer to [Manually Register Tables to
    Source](Manually_Register_Tables_to_Source.htm) for more
    information.
2.  Select **Manual Data Services** in the **Package Type** list box.
3.  Click **Save**.
4.  Click **Vertical View** for the registered table package.
5.  Click the **Advanced Setting** tab.
6.  Click **Edit**.
7.  Select the Data Services job from the **Package Name** list box.
8.  Click **Save**.

**NOTE**: The Build process should not be run for any manual package
types.

**NOTE**: The Manual Data Services package type does not execute against
an SAPAPPSERVER source.

**NOTE**: The table must exist in the Collect target database for the
package refresh to work.
