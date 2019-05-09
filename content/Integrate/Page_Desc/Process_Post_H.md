+++
title = 'Process Post H'
solution = 'Platform'
+++

# Process Post H

[Process Post V All Tabs](#Process_Post_V_All_Tabs)

<div class="use">

Use this page to:

  - [Use a Process Post Record to Post to SAP for a Process Based on a
    BDC Script
    Template](../Use_Cases/Post_Data_for_a_Process_Based_on_a_BDC_Script_Template)
  - [Use a Process Post Record to Post to SAP for a Process Based on a
    GUI Script
    Template](../Use_Cases/Post_Data_for_a_Process_Based_on_a_GUI_Script_Template)
  - [Use a Process Post Record to Post to SAP for a Process Based on a
    BAPI](../Use_Cases/Post_Data_for_a_Process_Based_on_a_BAPI)
  - [Use a Process Post Record to Post to SAP for a Process Based on an
    RFC](../Use_Cases/Post_Data_for_a_Process_Based_on_an_RFC)
  - [Create and Transfer Delimited or Fixed Width
    Files](../Use_Cases/CreateTransferDelimFWidthFiles)
  - [Create and Transfer XML
    Files](../Use_Cases/Create_and_Transfer_XML_Files)

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Integrate \>
    </span>**Categories** on *Navigation pane*.
2.  Click the **Processes** icon for a category.
3.  Click the **Postings** icon for a process.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the sort order for process posts on the current page.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the process post entered when adding the process post. If the process post is the initial post added by Integrate, the description begins with <strong>Auto Generated Post For</strong>.</p></td>
</tr>
<tr class="even">
<td><p>PROCESS ID</p></td>
<td><p>Displays the name of the process used in the process post entered on the <em>Process</em> page’s <em>Vertical</em> View.</p></td>
</tr>
<tr class="odd">
<td><p>WHERE CLAUSE</p></td>
<td><p>Displays a where clause to apply to the process post. If the field is blank, Integrate uses an empty string. <strong>Important: When posting a BDC, GUI, or BAPI/RFC template with more than 1 loop, the WHERE CLAUSE must apply to ALL views mapped to the loops.</strong></p></td>
</tr>
<tr class="even">
<td><p>Connections</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Process_Post_Connections">Process Post Connections</a></span> page to set the connections for each process template. The Connection ID list box displays the connections added at the process template level on the <a href="Process_Template_Connections">Process Template Connections</a> page..</p>
<p>The count on the icon is the number of connections set for the Process Post record.</p>
<p><strong>NOTE:</strong> There must be one target system connection for each process template in the process.</p></td>
</tr>
<tr class="odd">
<td><p>Post</p></td>
<td><p>Click to post the process post.</p>
<p>This icon does not display if the process is based on a GUI script template, or if the process includes multiple templates and one of them is based on a GUI script.</p></td>
</tr>
<tr class="even">
<td><p>Monitor</p></td>
<td><p>Click to open the <em><a href="Post_Monitor_H">Post Monitor</a></em> page for the selected process post to view the post status.</p></td>
</tr>
<tr class="odd">
<td><p>View Messages</p></td>
<td><p>Click to open the <em><a href="Messages_H">Messages</a></em> page to view messages returned from the process post.</p></td>
</tr>
</tbody>
</table>

## <span id="Process_Post_V_buttons"></span>Process Post V Buttons

[Process Post H](Process_Post_H)

<span style="font-weight: bold;">NOTE</span>: These buttons display
above all
tabs.

|                       |                                                                                                                                                                                                                                                                                            |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field                 | Description                                                                                                                                                                                                                                                                                |
| Post                  | Click to post the process post.                                                                                                                                                                                                                                                            |
| View Messages         | Click to open the *[Messages](Messages_H)* page to view messages returned from the process post.                                                                                                                                                                                       |
| Delete Messages       | Click to delete all messages for the process post. Messages must be deleted manually.                                                                                                                                                                                                      |
| View Posting Defaults | Click to open the *[Posting Defaults](../Use_Cases/Posting_Defaults)* page to view the default posting values for a process post. This values are set in Common on the *[Parameters Integrate](../../Common/Page_Desc/Parameters_Integrate)* page on the **Posting Defaults** tab. |

## <span id="Process_Post_V_All_Tabs"></span>Process Post V All Tabs

[Process Post H](Process_Post_H)

<div class="use">

Use this page to:

  - [Post Data for a Process Based on a BDC Script
    Template](../Use_Cases/Post_Data_for_a_Process_Based_on_a_BDC_Script_Template)
  - [Post Data for a Process Based on a GUI Script
    Template](../Use_Cases/Post_Data_for_a_Process_Based_on_a_GUI_Script_Template)
  - [Post Data for a Process Based on a
    BAPI](../Use_Cases/Post_Data_for_a_Process_Based_on_a_BAPI)
  - [Post Data for a Process Based on an
    RFC](../Use_Cases/Post_Data_for_a_Process_Based_on_an_RFC)
  - [Post Data Using an SAP Data Services
    Job](../Use_Cases/Post_Data_Using_an_SAP_Data_Services_Job_Overview)
  - [Create and Transfer Delimited or Fixed Width
    Files](../Use_Cases/CreateTransferDelimFWidthFiles)
  - [Create and Transfer XML
    Files](../Use_Cases/Create_and_Transfer_XML_Files)

</div>

This page has the following tabs:

  - [General tab](#General_Tab4)
  - [Advanced tab](#Advanced_Tab1)
  - [Posting tab](#Posting_Tab1)

## <span id="General_Tab4"></span>General tab

Field

Description

Post Settings

Priority

Displays the sort order for process posts on the *Process Post* page’s
*Horizontal* View.

Description

Displays a description of the process post entered when adding the
process post. If the process post is the initial post added by
Integrate, the description begins with **Auto Generated Post For**.

Process ID

Displays the name of the process used in the process post entered on the
*Process* page’s *Vertical* View.

Component

Displays the name of the component that is used to post data.

View Primary Loop Data

Click to open the *[Process Post](#)* page to view the data in the
primary loop of the first template in the process post before posting to
SAP. This page can also be used to validate the where clause.

Where Clause

Displays a where clause to apply to the data to limit the records to
post. If the field is blank, Integrate uses an empty string.  The syntax
of the where clause must be valid. If it is not, Integrate displays a
message.  **Important: When posting a BDC, GUI, or BAPI/RFC template
with more than one loop, the WHERE CLAUSE must apply to ALL views mapped
to the loops.**

## <span id="Advanced_Tab1"></span>Advanced tab

Field

Description

Advanced Post Settings

Posting ID

Displays the ID for the process post generated by Integrate.

BDC Post Method

Displays the method Integrate uses when posting. For a process post with
a single BDC Scrip template, all options in the list box can be used.
For any other template type, or for any process post with multiple
templates, select StandardSAP Posting.  

Batch Size

Displays the number of records to be posted at one time. If a value is
not entered, Integrate uses the default of 100 records. In the case of
User Defined templates, a process post creates a file with the name
\[Process Name\] {Template Name\] \[Batch Number\].txt, and the number
is based on the number of records included in each batch.

Comment

Displays information entered about the process post. Integrate includes
this text with every record of the process post.

Transfer Files to Data Source

If enabled, Integrate transfers the files to the data source configured
on the *Vertical* View of the *SAP Connections* page. If disabled,
Integrate creates the file and stores it on the server. This field is
used with User Defined Template Type only.

Debug and Test Options

Start Template Priority

Displays the priority of the template to start with when posting. This
feature is used to debug process posts for process with multiple
templates.

End Template Priority

Displays the priority of the template to end with when posting. This
feature is used to debug process posts for process with multiple
templates.

Create GUI Debug Script

If enabled, Integrate creates a copy of the GUI script run against SAP
and writes it to the Message table along with the results of the post.
Download the debug script from the *[Messages](Messages_H)* page and
run it in the SAP GUI to debug a GUI script posting.

Create Full GUI Debug Script

Click to create a debug script based on the settings for the template
and process. This script is created separately from posting, and can be
used to debug the script prior to upload to ensure it was created
properly. The script can then be run manually in SAP or run when the
record is posted.

Download Full GUI Debug Script

Click to download the GUI Script created when the user clicked Create
Full GUI Debug Script.

BOA Function Module Upload Options

**NOTE:** The settings in this section are not used when the BDC Post
Method is StandardSAPPosting.

Keep Session

If enabled, the session is saved in an SAP SM35 session even after a
successful post. Saving a session is useful in the event it needs to be
rerun. This option is used with the BDC Post Method BOASessionCreation
and BOAPostingWithErrorSessionCreation.

Continue on Commit

If enabled, the script should continue with processing after a commit
has occurred. Whether this option is used depends upon the transactions
being played back in the recording.

No Data Symbol

 

Displays a symbol to represent “no data” in the post. If the field is
blank, Integrate uses an empty string to represent no data.

Group Name

Displays the name that appears in the Group Name column of the SAP SM35
session. If the field is blank, Integrate uses \>BOA.

BOA BDC File Options

**NOTE:** The settings in this section are only used when the BDC Post
Method is BOAFileCreation.

Session File Path

Displays the location on the web server where Integrate creates files to
be used in the /BOA/ZBDCPROCESS program in SE38.

Session File Name

Displays the name of the file Integrate creates.

File Split Interval

Displays an interval to indicate the number of transactions in each file
created during the posting process.

## <span id="Posting_Tab1"></span>Posting tab

Field

Description

Post Methods

Foreground Post

Click to immediately post data in the foreground using the SAP user ID
and password entered on the *[User
Credentials](../../Common/Page_Desc/User_Credentials_H)* page.

This icon does not display if the process is based on a GUI script
template, or if the process includes multiple templates and one of them
is based on a GUI script.

Background Post

Click to schedule a post to run in the background at the time entered in
the **Post Start Time** field. Use this posting method when there is too
much data to post in the foreground without timing out the session and
to avoid putting too much stress on the system. If the **Post Start
Time** is blank, the Background Post will run the next time the
Scheduler Service page runs.

Post Start Time

Displays the date and time the post is scheduled to run when using the
Background Post posting method.

Stored Credentials

User Credentials

Click to open the <span style="font-style: italic;">[User
Credentials](../../Common/Page_Desc/User_Credentials_H)</span> page
to add login credentials to use for the process post for a given data
source.

Credentials Detected

If enabled, the system has user credentials for the process post. Refer
to [User Credentials in
Integrate](../Config/User_Credentials_in_Integrate) for more
information.

Status & Return

Monitor

Click to open the *[Post Monitor](Post_Monitor_H)* page to view
information about the post including the status.

Reset Post

Reset

Click to reset the process post to submit it again. After resetting a
post it can be submitted again regardless of its status prior to the
reset, and regardless of the reason for the failure.
