+++
title = 'Template H'
solution = 'Platform'
+++

# Template H

[Template V All Tabs](#Template_V_All_Tabs)

<div class="use">

Use this page to [Create a Basic
Template.](../Use_Cases/Create_a_Basic_Template.htm)

</div>

To access this page:

1.  Select **Integrate \> Categories** from the *Navigation pane*.
2.  Click the **Templates** icon for a category.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Category Processes</p></td>
<td><p>Click to open the <em>Process</em> page to add, edit, and delete processes for the category.</p></td>
</tr>
<tr class="odd">
<td><p>TEMPLATE NAME</p></td>
<td><p>Displays the name of the template entered when the template was added.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the template entered when the template was added.</p></td>
</tr>
<tr class="odd">
<td><p>CONNECTION ID</p></td>
<td><p>Displays the connection ID for the target system against which the template type will be created.</p>
<p>The options in this list box are connections registered in Common. Refer to <a href="../../Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm">Establish a Connection to a Target System</a> for more information.</p>
<p><strong>NOTE:</strong> The connections that display are based on the selection in the TYPE list box. For example, if the user selects the template type BODS Execution, the CONNECTION ID list box displays connections to Data Services repositories only.</p></td>
</tr>
<tr class="even">
<td><p>TYPE</p></td>
<td><p>Displays the template type selected when the template was added.</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVATE/DEACTIVATE</p></td>
<td><p>Click to activate the template. The button displays a green icon for active templates and a red icon for inactive templates.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the template is active. If disabled, the template is inactive.</p></td>
</tr>
<tr class="odd">
<td><p>Report</p></td>
<td><p>Click to open the Template report which displays the screens, fields and other data captured during template creation.</p></td>
</tr>
<tr class="even">
<td><p>L</p></td>
<td><p>If enabled, the template contains loops. Looping can be enabled at the template level for BDC Script and GUI Script template types only.</p></td>
</tr>
<tr class="odd">
<td><p>Processes</p></td>
<td><p>Click to open the <em><a href="Template_Processes.htm">Template Processes</a></em> page which lists the processes to which the template is assigned.</p></td>
</tr>
</tbody>
</table>

## <span id="Template_V_All_Tabs"></span>Template V All Tabs

[Template H](Template_H.htm)

This page has the following tabs:

  - [General tab  BDC Script Template Type](#General_Tab_BDC_Script)
  - [Configuration tab  BDC Script Template
    Type](#Configuration_Tab_BDC)
  - [Documentation tab](#Documentation_Tab)
  - [Copy tab](#Copy_Tab)
  - [General tab  BAPI/RFC Template Type](#General_Tab_BAPI_RFC)
  - [Configuration tab  BAPI/RFC Template Type](#Configuration_Tab_BAPI)
  - [General tab  GUI Script Template Type](#General_Tab_GUI_Script)
  - [Configuration tab  GUI Script Template
    Type](#Configuration_Tab_GUI)
  - [General tab IG Universal Connect](#General)
  - [General tab: SAP Data Services Job Template
    Type](#General_Tab_SAP_Data_Services_Job_Template_Type)
  - [General tab  User Defined Template
    Types](#General_Tab_User_Defined)
  - [Configuration tab  User Defined Template
    Type](#Configuration_Tab_User)

## <span id="General_Tab_BDC_Script"></span>General tab  BDC Script Template Type

<div class="use">

Use this page to [Record a BDC
Script](../Use_Cases/Record_a_BDC_Script.htm) and [Import a BDC Script
from a File](../Use_Cases/Import_a_BDC_Script_From_a_File.htm).

</div>

Field

Description

Basic Details

Template Name

Displays the name of the template entered when the template was added.

Connection ID

Displays the SAP connection ID for the system against which the BDC
script will be created.

The options in this list box are connections registered in Common. Refer
to [Establish an SAP Connection in
Common](../../Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
for more information.

**NOTE:** The connections that display are based on the selection in the
Type list box. For example, if the user selects the template type BODS
Execution, the CONNECTION ID list box displays connections to Data
Services repositories only.

Type

Displays the template type selected when the template was added  in this
case BDC Script .

Transaction Code

Displays the SAP transaction code used by the BDC script in recording.
Integrate passes this value to SAP during the recording process.

Integrated Recording

Record

Click to record the BDC script. A recording overwrites all template data
with data from the recording. Depending on Integrate configuration, the
user may be required to enter credential information for the SAP system.

File Import

File Name Upload a file/Download a file

Click to Upload the SHDB recoding file for import. Click Download to
download the file that was uploaded.

Import

Click to import an uploaded SHDB recording file containing a BDC script.
A file must first be uploaded before it can be
imported.

## <span id="Configuration_Tab_BDC"></span>Configuration tab  BDC Script Template Type

Field

Description

Template Configuration

Enable Loop

If enabled, the <span style="color: #000000;">BDC script can be
configured to use looping at the BDC Script Data level and BDC Script
Data rows can be put into and taken out of loops. When processing a loop
during posting,</span> Integrate processes multiple child keys for one
parent key. Looping also allows Integrate to post multiple headers with
infinite details. Enable looping during template creation or after
recording.

BDC Screen

Click to open the *[BDC Screen](BDC_Screen_H.htm)* page to manage the
screens and fields captured during the BDC script recording.

Custom Fields

Click to open the <span style="font-style: italic;">[Custom
Fields](Custom_Fields.htm)</span> page to add custom fields to the BDC
Script template. The count on this icon represents the number of custom
fields that have been added to the template.

## <span id="Documentation_Tab"></span>Documentation tab

Field

Description

Template Documentation

Notes

Displays notes entered about the template.

Report

Click to open the Template report which displays the screens, fields and
other data captured during template creation.

Active

If enabled, the template is active and can be added to a process but
cannot be updated.

If disabled, the template can be edited.

### <span id="Copy_Tab"></span>Copy tab

Field

Description

New Template Settings

Copy Template

Click to open the *[Copy](Copy.htm)* page to create a template based on
a copy of the current template.

Merge BDC Screens

Click to open the *Copy* page to merge the BDC screens captured in the
current template to another template in any category.

**NOTE:** This button displays for BDC Script template types
only.

## <span id="General_Tab_BAPI_RFC"></span>General tab  BAPI/RFC Template Type

<div class="use">

Use this page to [Configure a BAPI
Template](../Use_Cases/Configure_a_BAPI_Template.htm) and [Configure an
RFC Template](../Use_Cases/Configure_a_RFC_Template.htm).

</div>

Field

Description

Basic Details

Template Name

Displays the unique name of the template entered when the template was
added.

Connection ID

Displays the SAP connection ID for the system which contains the
BAPI/RFC.

The options in this list box are connections registered in Common. Refer
to [Establish an SAP Connection in
Common](../../Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
for more information.

The connections that display are based on the selection in the Type list
box. For example, if the user selects the template type BODS Execution,
the CONNECTION ID list box displays connections to Data Services
repositories only.

Type

Displays the template type selected when the template was added  in this
case BAPI/RFC .

Function Name

Displays the RFC/BAPI function that Integrate can call from SAP. This
value is selected when the template is added. The functions are
extracted from SAP using the *SAP Connections* page.

Create BAPI Template

Click to pull the definition of the Function Module listed in the
Function Name field from SAP to complete the template.

<span id="General_Tab_IG_Universal_Connect"></span>

## <span id="General"></span>General tab IG Universal Connect

<div class="use">

Use this page to [Create an IG Universal Connect
Template](../../IGUC/Create%20an%20IG%20Universal%20Connect%20Template.htm).

</div>

Field

Description

Template Name

Displays the unique name of the template.

Connection ID

Displays the name of the data source that contains the Boomi Process
used by the Template.

The options in this list box are connections registered in Common.

Type

Displays IG Universal Connect.

Boomi

Boomi Process ID

Displays the name of the Boomi Process used to post data. This is the
default Process added with the data source, but can be updated to
another Process as needed.

### <span id="General_Tab_SAP_Data_Services_Job_Template_Type"></span>

 

## General tab SAP Data Services Job Template Type

<div class="use">

Use this page to [Create a Template with the SAP Data Services Job
Template
Type](../Use_Cases/Create_an_SAP_Data_Services_Job_template.htm).

</div>

Field

Description

Basic Details

Template Name

Displays the unique name of the template entered when the template was
added.

Connection ID

Displays the connection ID for the target system for posting.

The options in this list box are connections registered in Common. Refer
to [Establish a Connection to a Target
System](../../Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
for more information.

The connections that display are based on the selection in the Type list
box. For example, if the user selects the template type SAP Data
Services Job, the CONNECTION ID list box displays connections to Data
Services repositories only.

Type

Displays the template type selected when the template was added, in this
case SAP Data Services Job.

File Structure

Data Services Job Name

Displays the data source job added to the process post record for
processes based on the SAP Data Services Job template
type.

## <span id="Configuration_Tab_BAPI"></span>Configuration tab  BAPI/RFC Template Type  

Field

Description

BAPI/RFC Configuration

BAPI/RFC Definition

Click to open the *BAPI/RFC Definition* page to view the definitions and
BAPI fields contained in each definition.

**NOTE:** The template must be created for data to display on the page.

**NOTE:** Refer to [Extract RFC
Functions](../Config/Extract_RFC_Functions.htm) for more
information.

## <span id="General_Tab_GUI_Script"></span>General tab  GUI Script Template Type

<div class="use">

Use this page to [Record a GUI
Script](../Use_Cases/Record_a_GUI_Script.htm).

</div>

Field

Description

Basic Details

Template Name

Displays the unique name of the template entered when the template was
added.

Connection ID

Displays the SAP connection ID for the system against which the GUI
script will be recorded.

The options in this list box are connections registered in Common. Refer
to [Establish an SAP Connection in
Common](../../Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
for more information.

The connections that display are based on the selection in the Type list
box. For example, if the user selects the template type BODS Execution,
the CONNECTION ID list box displays connections to Data Services
repositories only.

Type

Displays the template type selected when the template was added  in this
case, GUI Script .

Transaction Code

Displays the SAP transaction code used by the GUI script in recording.
Integrate passes this value, entered when the template was added, to SAP
during the recording process.

Integrated Recording

Record

Click to record the GUI script. The SAP Logon pad must already be open.
A recording overwrites all template data with data from the
recording.

## <span id="Configuration_Tab_GUI"></span>Configuration tab  GUI Script Template Type

Field

Description

Template Configuration

Enable Loop

If enabled, the <span style="color: #000000;">GUI script can be
configured to use looping at the GUI Script Data level and GUI Script
Data rows can be put into and taken out of loops. When processing a loop
during posting,</span> Integrate processes multiple child keys for one
parent key. Looping also allows Integrate to post multiple headers with
infinite details. Enable looping during template creation or after
recording.

GUI Script Data

Click to open the *[*GUI Script Data*](GUI_Script_Data_H.htm)* page to
edit and delete the fields captured during the GUI script
recording.

## <span id="General_Tab_User_Defined"></span>General tab  User Defined Template Types

<div class="use">

Use this page to [Create a Delimited or Fixed Width User Defined
Template](../Use_Cases/CreateDelimFWUD.htm) and [Configure an XML
Template](../Use_Cases/ConfigureXMTemplateStrctrEleAtt.htm).

</div>

Field

Description

Basic Details

Template Name

Displays the unique name of the template entered when the template was
added.

Connection ID

Displays the SAP connection ID for the system that can use data in the
user defined file after it is created and transferred to an FTP server.

The options in this list box are connections registered in Common. Refer
to [Establish an SAP Connection in
Common](../../Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
for more information.

The connections that display are based on the selection in the Type list
box. For example, if the user selects the template type BODS Execution,
the CONNECTION ID list box displays connections to Data Services
repositories only.

Type

Displays the template type selected when the template was added  in this
case User Defined .

File Structure

User Defined Template Type

Displays the template type. Values are Delimited, FixedWidth and XML.

Define

Click to open the *[Structure](Structure%20H.htm)* page to add, edit and
delete structures for the User Defined template. When adding a template,
this button displays after a value is selected in the **User Defined
Template Type** list box and the template is
saved.

## <span id="Configuration_Tab_User"></span>Configuration tab  User Defined Template Type

<div class="use">

Use this page to [Create a Delimited or Fixed Width User Defined
Template](../Use_Cases/CreateDelimFWUD.htm) and [Configure an XML
Template](../Use_Cases/ConfigureXMTemplateStrctrEleAtt.htm).

</div>

Field

Description

File Configuration

Delimiter

Displays the character that separates the values in delimited files.
Displays for a Delimited Template Type only.

Fixed Width Pad Location

Displays whether Integrate will pad the value in the field to its full
length with spaces before or after the value for Fixed Width files. For
XML files, this field should display \[None\].
