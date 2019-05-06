# Attachments and Summaries

A workflow email can contain an attachment in Excel 2007 or later
(.xlsx) format that lists all the failed data records for each rule.
Each worksheet displays data for one run, one rule and one table.
Workflow emails with attachments are sent at the project distribution
level. No emails are sent with attachments for all failed rules in a
project.

A workflow email can also contain only a summary table listing the rules
and number of failed records for each rule for a project distribution.

**NOTE**: Summary workflows are sent at the user level only. Summary
emails will not be sent to all users in a project distribution, unless
all users in that project distribution have selected to receive
summaries as a workflow option.

Whether a user receives an attachment or a summary email (or no email)
is set using the WORKFLOW OPTION setting on the
*[Users](../Page_Desc/Users_ISA.htm)* page. Refer to [Configure Workflow
Options](Configure_Workflow_OptionsISA.htm) for more information.

The workflow emails also contain a link to the scorecard in Information
Server for the associated rule(s). Refer to [Access
Scorecards](Access_Scorecards.htm) for more information.

If the server or port name changes for the IS installation, use the
**Information Steward Settings** tab on the
<span style="font-style: italic;">[Parameters](../Page_Desc/ISA_Parameters.htm)</span>
page to enter the new information and update the project scorecard link.
Refer to [Update the Scorecard Link](Update_the_Scorecard_Link.htm) for
more information.

<span style="font-weight: bold;">NOTE</span>: If a rule has no failed
records, the rule does not display in workflow emails or in the Excel
file attached to workflow emails.

<span style="font-weight: bold;">NOTE</span>: If a rule is bound to a
single table on multiple fields, each binding will generate a
spreadsheet to send as an attachment to users in the project
distribution. The spreadsheet will contain data that failed the rule for
each field-table combination.

<span style="font-weight: bold;">NOTE:</span> If a rule has no failed
records, the rule does not display in workflow emails or in the Excel
file attached to workflow emails.
