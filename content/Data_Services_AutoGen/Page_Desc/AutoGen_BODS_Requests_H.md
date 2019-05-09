+++
title = 'AutoGen BODS Requests H'
solution = 'Migration'
+++

# AutoGen BODS Requests H

[AutoGen BODS Requests V](#AutoGen_BODS_Requests_V)

<div class="use">

Use this page to [Build and Refresh Data Services
Jobs](../Use_Cases/Build_and_Refresh_DS_Jobs).

</div>

To access this page:

1.  Click the **Automation** tab in the Quick Panel.
2.  Select the Object for which the request is being generated.
3.  Click the **Build and Refresh Data Services** icon in the Page
    toolbar; the *[AutoGen Data
    Services](AutoGen_Data_Services)* page displays.
4.  Click the **Auto Gen Requests** icon; the *Autogen BODS
    Requests* page displays.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>OBJECT</p></td>
<td><p>Displays the name of the object as created in Console. This field is populated by the system.</p></td>
</tr>
<tr class="odd">
<td><p>Wave NAME</p></td>
<td><p>Displays the name of the Wave.</p></td>
</tr>
<tr class="even">
<td><p>TARGET</p></td>
<td><p>Displays the name of the target table. This field is populated by the system.</p></td>
</tr>
<tr class="odd">
<td><p>Process Area</p></td>
<td><p>Displays the name of the Process Area.</p></td>
</tr>
<tr class="even">
<td><p>COMMENT</p></td>
<td><p>Displays the name of the request entered by the user.</p></td>
</tr>
<tr class="odd">
<td><p>REQUEST CREATE DATE</p></td>
<td><p>Displays the date the AutoGen request was created. This field is populated by the system when an AutoGen request is created and indicates that the request package is ready to be automatically or manually uploaded to the dspCloud™.</p></td>
</tr>
<tr class="even">
<td><p>REQUEST UPLOAD DATE</p></td>
<td><p>Displays the date the AutoGen request was uploaded to the dspCloud™. This field is populated by the system when an AutoGen request is uploaded to the dspCloud™.</p></td>
</tr>
<tr class="odd">
<td><p>LAST STATUS CHECK DATE</p></td>
<td><p>Displays the date the request status was last checked. This field is populated by the system and indicates the last date on which the system checked to determine if the AutoGen request is ready to be downloaded from the dspCloud™.</p></td>
</tr>
<tr class="even">
<td><p>JOB DOWNLOAD DATE</p></td>
<td><p>Displays the date the request was downloaded from the dspCloud™. This field is populated by the system once the AutoGen request has been generated in the dspCloud™ and downloaded to the DSP®.</p></td>
</tr>
<tr class="odd">
<td><p>AUTO GEN JOB STATUS</p></td>
<td><p>Displays the status of the AutoGen request. Initially the status is New. Once the AutoGen request has been processed in the dspCloud ™ and automatically downloaded, the status is changed to Processing Complete. This field is populated by the system.</p>
<p><strong>NOTE:</strong> If Job Status is set to Request Failed, navigate to the <span style="font-style: italic;">Vertical</span> View of the request. A detailed message displays in the Auto Gen Message field.</p></td>
</tr>
<tr class="even">
<td><p>JOB IMPORT DATE</p></td>
<td><p>Displays the date the jobs were registered in Transform as Data Services rules and automatically imported into Data Services.</p>
<p>This field is populated by the system.</p></td>
</tr>
<tr class="odd">
<td><p>Generate Request</p></td>
<td><p>Click to create the AutoGen request, which contains the metadata required to generate the Data Services Jobs for the specific target for which it is being generated.</p></td>
</tr>
<tr class="even">
<td><p>Upload to Auto Gen Service</p></td>
<td><p>Click to upload the request to the dspCloud™.</p></td>
</tr>
<tr class="odd">
<td><p>Import Into Data Services</p></td>
<td><p>Click to register the Data Services Jobs against the target in Transform and import the jobs into Data Services automatically.</p></td>
</tr>
</tbody>
</table>

## <span id="AutoGen_BODS_Requests_V"></span>AutoGen BODS Requests V

[AutoGen BODS Requests H](#)

<div class="use">

Use this page to [Build and Refresh Data Services
Jobs](../Use_Cases/Build_and_Refresh_DS_Jobs).

</div>

Field

Description

Target Details

Object

Displays the name of the object as created in Console. This field is
populated by the system.

Target

Displays the name of the target table. This field is populated by the
system.

Request

Generate Request

Click to generate the AutoGen request package.

Comment

Displays the name of the request entered by the user.

Request Create Date

Displays the date the AutoGen request was created. This field is
populated by the system when an AutoGen request is created and indicates
that the request package is ready to be automatically or manually
uploaded to the dspCloud™.

Request Upload Date

Displays the date the AutoGen request was uploaded to the dspCloud™.
This field is populated by the system when an AutoGen request is
uploaded to the dspCloud™.

Auto Gen Message

Displays the return message from Data Services.

Offline Mode

AutoGen Request File

Click to download an AutoGen request file. Used in cases where the DSP®
cannot connect to the dspCloud™. When working offline, the downloaded
AutoGen request file is manually uploaded to the dspCloud™, the
resulting job file is retrieved, and then uploaded to the DSP® by
clicking the Import Object icon on the *[AutoGen Data
Services](AutoGen_Data_Services)* page.
