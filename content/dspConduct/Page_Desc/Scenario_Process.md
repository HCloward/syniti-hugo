+++
title = 'Scenario Process H  '
solution = 'Data Quality'
+++

# Scenario Process H  

[Scenario Process V](#Scenario)

<div class="use">

Use this page to [Add a Process to a
Scenario](../Use_Cases/Add_an_Integrate_Process_to_a_Scenario.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspConduct
    \></span>**Design** in the *Navigation* pane.
2.  Click the **Scenarios** icon for a category.
3.  Click the **Processes** icon for a scenario.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>INTEGRATE PROCESS ID</p></td>
<td><p>Displays the Integrate process ID associated with this scenario.</p>
<p><strong>NOTE:</strong>  The processes that display in this list box are ones that have been set as allowable at the category level. Refer to <a href="../Use_Cases/Set_Allowed_Processes_at_the_Category_Level.htm">Set Allowable Processes at the Category Level</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the priority of the process.</p>
<p><strong>NOTE:</strong> This value determines the order the process displays on the <em>Scenario (Processes)</em> page and the order in which the processes are executed for posting.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled the process is active in the scenario. If disabled the process is not active in the scenario.</p></td>
</tr>
<tr class="odd">
<td><p>Target Connection</p></td>
<td><p>Click to open the <em><a href="Scenario_Process_Target_Connection.htm">Scenario Process Target Connection</a></em> page to edit the connection ID for process template associated to the scenario.</p>
<p>Refer to <a href="../Use_Cases/View_and_Configure_External_Target_Systems_Scnrio.htm">View and Configure External Target Systems</a> for a Scenario for more information.</p></td>
</tr>
<tr class="even">
<td><p>Rules</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Scenario_Process_Rule.htm">Scenario Process Rule</a></span> page to view the default rules assigned to the process at the category level, and to add rules to the process.</p>
<p>Refer to <a href="../Use_Cases/Add_Process_Rules_at_the_Scenario_Level.htm">Add Process Rules at the Scenario Level</a> for more information.</p></td>
</tr>
</tbody>
</table>

## <span id="Scenario"></span>Scenario Process V

[Scenario Process H](#)

<div class="use">

Use this page to [Update Posting Options at the Scenario
Level](../Use_Cases/Update_Posting_Options_at_the_Scenario_%20Level.htm).

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
