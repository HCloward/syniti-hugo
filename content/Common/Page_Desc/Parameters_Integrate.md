# Parameters – Integrate

<div class="use">

Use this page to [Configure Integrate
Parameters](../Use_Cases/Configure_Integrate_Parameters.htm).

</div>

To access this page, select <span style="font-weight: bold;">Common \>
Configuration \> Modules \> Parameters - Integrate</span> in the
<span style="font-style: italic;">Navigation</span> pane.

This page contains the following tabs:

  - [General tab](#General_Tab3)
  - [Posting Defaults tab](#Posting_Defaults_Tab)

## <span id="General_Tab3"></span>General tab

Field

Description

Application Information

Version

Displays current release version of the component, Integrate.

Release Date

Displays date when the component version was released.

Integrate Settings

Background Posting Queue ID

Displays the queue ID in which a post submitted using the Background
Post method is scheduled. Values are Background Events, General,
Indexing and Service Pages.

Import File Location

Displays the location on the server where import files are stored. A
user can upload and import a script when creating a BDC Script template.
Once the script is uploaded, Integrate saves the file to this location.

Posting Default Folder

Displays the location on the server where post files are stored. This
default value can be overridden at the process template level.

View Name Filter

Displays the prefix used for views that Integrate creates using the Auto
Generate Database Object feature.

Foreground Warning Threshold

Displays the value of the threshold for posting records in the
foreground using the Foreground Post posting method. If the number of
records in a posting exceeds the threshold, Integrate displays a warning
that the foreground posting may time out, and that a background posting
is recommended. The default value is **1000**.

Post File Archiving

Post File Archive Folder

Displays the location on the server where post archives are stored.

Post File Archive Retention Interval

Displays the number of days archive files are stored in the Post File
Archive Folder before they are deleted.

## <span id="Posting_Defaults_Tab"></span>Posting Defaults tab

Field

Description

Advanced Post Settings

BDC Post Method

Displays the method Integrate uses when posting. For a process post with
a single BDC Script template, all options in the list box can be used.
For any other template type, or for any process post with multiple
templates, select StandardSAP Posting.  This setting can be overridden
at the process post level.

Batch Size

Displays the number of records to be posted at one time. If a value is
not entered, Integrate uses the default of 100 records. In the case of
User Defined templates, a process post creates a file with the name
\[Process Name\] {Template Name\] \[Batch Number\].txt, and the number
is based on the number of records included in each batch. This setting
can be overridden at the process post level.

Comment

Displays comments about the advanced posting method or setting.

One File Per Structure

If enabled, Integrate creates one flat file for each structure when
creating flat files from a process. Used for Batch Load, Direct Load,
IDOC and User Defined template types.

Transfer Files To Data Source

If enabled, Integrate creates one flat file for each structure when
creating flat files from a process. Used for Batch Load, Direct Load,
and User Defined template types.

BOA Function Module Upload Options

Keep Session

If enabled, the session is saved in an SAP SM35 session even after a
successful post. Saving a session is useful in the event it needs to be
rerun. This option is used with the BDC Post Method BOASessionCreation
and BOAPostingWithErrorSessionCreation. This setting can be overridden
at the process post level.

Continue On Commit

If enabled, the script continues with processing after a commit has
occurred. Whether this option is used depends on the transactions being
played back in the recording. This setting can be overridden at the
process post level.

No Data Symbol

Displays a symbol to represent “no data” in the post. If the field is
blank, Integrate uses an empty string to represent “no data.” This
setting can be overridden at the process post level.

Group Name

Displays the name that appears in the Group Name column of the SAP SM35
session. If the field is blank, Integrate uses \>BOA. This setting can
be overridden at the process post level.

BOA BDC File Options

File Split Interval

Displays an interval to indicate the number of transactions in each file
created during the posting process. This setting can be overridden at
the process post level.

Session File Path

Displays the location on the web server where Integrate creates files to
be used in the /BOA/ZBDCPROCESS program in SE38. This setting can be
overridden at the process post level.

Session File Name

Displays the default name of the session file Integrate creates for all
session files. This setting can be overridden at the process post level.
