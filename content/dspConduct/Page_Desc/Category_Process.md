# Category Process

[Category Process V](#Category)

<div class="use">

Use this page to [Set Allowed Processes at the Category
Level](../Use_Cases/Set_Allowed_Processes_at_the_Category_Level.htm).

</div>

To access this page:

1.  Click **dspConduct \> Design** in the *Navigation* pane.
2.  Click **Vertical View** for a category.
3.  Click the **Posting Processes** icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>INTEGRATE PROCESS ID</p></td>
<td><p>Displays the name of the Integrate process. Click the name link and the <span style="font-style: italic;"><a href="../../../Platform/Integrate/Page_Desc/Process_H.htm">Process</a></span> page in Integrate displays with details about the process.</p>
<p><strong>NOTE:</strong> Only active processes display.</p></td>
</tr>
<tr class="odd">
<td><p>Rules</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Category_Process_Rule.htm">Category Process Rule</a></span> page to assign stored procedures that need to execute before the process is used for posting. </p>
<p>Rules are optional. Every process does not require a rule.</p>
<p>The stored procedures are written by the Designer.</p>
<p>The count on the icon represents the number of rules that exist for the category process.</p></td>
</tr>
</tbody>
</table>

## <span id="Category"></span>Category Process V

[Category Process H](#)

<div class="use">

Use this page to [Set Posting Options at the Category
Level](../Use_Cases/Set_Posting_Options_at_the_Category_Level.htm).

</div>

Field

Description

BOA Function Module Upload Options

**NOTE**: The settings in this section are not used when the BDC Post
Method is StandardSAPPosting.

Keep Session

If enabled, the session is saved in an SAP SM35 session even after a
successful post. Saving a session is useful in the event it needs to be
rerun. This option is used with the BDC Post Method BOASessionCreation
and BOAPostingWithErrorSessionCreation.

Continue on Commit

If enabled, the script continues with processing after a commit has
occurred. Whether this option is used depends upon the transactions
being played back in the recording.

No Data Symbol

Displays a symbol to represent "no data"? in the post. If the field is
blank, Integrate uses an empty string to represent no data.

BDC Post Method

Displays the method used for posting the request. Refer to [BDC Post
Methods and Settings on the Advanced
tab](../../../Platform/Integrate/Page_Desc/BDCPostMethodsSettingsAdvTab.htm)
for more information.

Group Name

Displays the name that appears in the Group Name column of the SAP SM35
session. If the field is blank, Integrate uses \>BOA.

BOA BDC File Options

**NOTE**: The settings in this section are only used when the BDC Post
Method is BOAFileCreation.

Session File Path

Displays the location on the web server where Integrate creates files to
be used in the /BOA/ZBDCPROCESS program in SE38.

Session File Name

Displays the name of the file Integrate creates.

File Split Interval

Displays an interval to indicate the number of transactions in each file
created during the posting process.
