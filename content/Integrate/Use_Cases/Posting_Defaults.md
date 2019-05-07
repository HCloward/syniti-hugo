+++
title = 'Posting Defaults'
solution = 'Platform'
+++

# Posting Defaults

<div class="use">

Use this page to view the posting defaults for the selected process
post. Refer to [BDC Post Methods and Settings on the Advanced
tab](../Page_Desc/BDCPostMethodsSettingsAdvTab.htm) for more
information.

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Integrate \>
    </span>**Categories** on *Navigation*<span>pane</span>.
2.  Click the **Processes** icon for a category.
3.  Click the **Postings** icon for a process.
4.  Click the **Vertical View** for a Process Post.
5.  Click the **View Posting Defaults** icon.

Field

Description

BDC Post Method

Displays the method Integrate uses when posting. For a process post with
a single BDC Scrip template, all options in the list box can be used.
For any other template type, or for any process post with multiple
templates, select StandardSAP Posting.  

Batch Size

Displays the number of records to be posted at one time. If a value is
not entered, Integrate uses the default of 100 records.

Comment

Displays information entered about the process post. Integrate includes
this text with every record of the process post.

One File per Structure

If enabled, Integrate creates one flat file for each structure when
creating flat files from a process. Used for  User Defined template
types.

Transfer Files to Data Source

If enabled, Integrate transfers the files to the data source configured
in Common. If disabled, Integrate creates the file and stores it on the
server. This field is used with User Defined Template Type only.

Refer to [Establish an SAP
Connection](../../Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
for more information.

BOA Function Module Upload Options

NOTE: The settings in this section are not used when the BDC Post Method
is StandardSAPPosting.

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

NOTE: The settings in this section are only used when the BDC Post
Method is BOAFileCreation.

File Split Interval

Displays an interval to indicate the number of transactions in each file
created during the posting process.

Session File Path

Displays the location on the web server where Integrate creates files to
be used in the /BOA/ZBDCPROCESS program in SE38.

Session File Name

Displays the name of the file Integrate creates.
