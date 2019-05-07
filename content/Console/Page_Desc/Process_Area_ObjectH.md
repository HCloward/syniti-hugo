+++
title = ''
solution = 'Migration'
+++

# <span id="Process_Area:_Object_H"></span>Process Area: Object H

[Process Area: Object V](#Process_Area_Object_V)

<div class="use">

Use this page to [Create the Context by Adding a Wave and Creating
Elements](../Use_Cases/Add_a_Wave_and_Create_Elements.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane, or select
    <span style="font-weight: bold;">Console</span> in the Context bar.
2.  Click <span style="font-weight: bold;">Waves</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
3.  Click the <span style="font-weight: bold;">Process Areas</span> icon
    for a Wave.
4.  Click the <span style="font-weight: bold;">Objects</span> icon for a
    Process
Area.

|                 |                                                                                                                                                                                                                                                                  |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                                                                                                                                                      |
| Copy            | Click to open the<span style="font-style: italic;">[Copy Object to Process Area](Copy_Object_to_Process_Area.htm)</span> page where the Process Area to which the Object is to be copied is specified.                                                           |
| Move            | Click to open the *[Move Object to Process Area](Move_Object_to_Process_Area.htm)* page where the Process Area to which the Object is to be moved is specified.                                                                                                  |
| Wave ID         | Displays the name of the Wave, which categorizes the migration project. Examples of Wave names include country names or specific work locations where the migration will be rolled out.                                                                          |
| COMMENT         | Displays user-entered comments about the Object.                                                                                                                                                                                                                 |
| Process Area ID | Displays the name of the Process Area. Combining a Process Area with a Wave creates a context, which can be selected in the Context bar and used throughout the dspMigrate™ Advanced Data Migration (ADM) components while working on a migration project.       |
| OBJECT ID       | Displays a concatenated value that is comprised of the Object name and the description (\<object name\> + ‘-‘ + \<description\>). The Object name is the name of the migration Object.                                                                           |
| PRIORITY        | Displays the data source for the Object, which is based on the name of the Data Source.                                                                                                                                                                          |
| Targets         | Click to open the <span style="font-style: italic;">[Targets](../../Design/Page_Desc/Targets_H_Design.htm)</span> and <span style="font-style: italic;">[Target Fields](../../Design/Page_Desc/Target_Fields_H_Target_Design.htm)</span> pages in Target Design. |

## <span id="Process_Area_Object_V"></span>Process Area: Object V

[Process Area: Object H](#Process_Area:_Object_H)

<div class="use">

Use this page to:

  - [Create a Context by Adding a Wave and Creating
    Elements](../Use_Cases/Add_a_Wave_and_Create_Elements.htm)
  - [Configure Data Services
    Functionality](../Config/Configure_Data_Services_Functionality.htm)

</div>

Field

Description

Basic Data

Object ID

Displays the name of the migration Object.

Data Source ID

Displays the data source for the Object, which is a Transform database.
This database is where all Target tables and all Source tables will be
registered.

**NOTE:** A data source can be added from this page. Click the **+**
sign to open the *[Data Source
Registry](../../../Platform/Common/Page_Desc/Data_Source_Registry_H.htm)*
page.

**NOTE:** DATA SOURCE ID is a hard-required field needed for the
execution of the Business Data Transformation via Transform..

**NOTE:** The options that display in this list box are filtered by the
Transform Database Filter (set on the *[Parameters](Parameters.htm)*
page on the General tab). The default value is dsw% used by Transform
databases.

Report Cache Data Source ID

Displays the name of the database that contains the tables storing the
results of report views.

**NOTE:** REPORT CACHE DATA SOURCE ID is required for the execution of
the Business Data Transformation and Report Delivery via Transform.

Comment

Displays user-entered comments about the Object.

ERP System Values

ERP Instance

Displays the ERP system instance that stores the Object. This is a
free-form text field to store data and is not validated.

ERP Client

Displays the ERP system client name that stores the Object. This is a
free-form text field to store data and is not validated.

**NOTE**: The ERP Client must be set for any reports generated by SQL
AutoGen referencing check tables that contain the Client column.

ERP Database

Displays the ERP system database that stores the Object. This is a
free-form text field to store data and is not validated.

Data Services Configuration

Data Services

Click to enable the Data Services options on DSP® pages for a migration
project.

For the Data Services icons on the
*[Targets](../../Transform/Page_Desc/Targets_H.htm)* page in Transform
to display, a Data Services repository must be assigned to the object
containing the Target in Console.

Refer to [Configure Data Services
Functionality](../Config/Configure_Data_Services_Functionality.htm) for
more information.

Data Services Repository

Displays the name of the Data Services Repository.

A Data Services Repository is a set of tables that stores user-created
and predefined system objects, Source and Target metadata and
transformation rules. Repositories are configured in SAP Data Services,
and then registered in Common in the DSP®. Refer to [Register a Data
Source in
Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
for more information.

For the Data Services icons on the
*[Targets](../../Transform/Page_Desc/Targets_H.htm)* page in Transform
to display, a Data Services repository must be assigned to the Object
containing the Target in Console.
