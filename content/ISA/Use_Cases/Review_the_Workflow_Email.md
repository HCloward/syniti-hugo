# Review the Workflow Email

Depending on a user’s workflow options settings,a workflow email can
contain a summary oran attachment.

Refer to [Attachments and Summaries](Summaries_and_Attachments) for
more information.

Workflow emails for summaries and attachment have a link to the IS
scorecard for the project.

If a user has the Workflow option set to receive attachments, the ISA
attaches an Excel file to the email that contains information about data
that failed IS rules for a given Project Distribution.

The Excel file contains a summary worksheet and a worksheet for each
rule that has failed records within a given Project Distribution.

The summary worksheet lists:

  - All rules in the workbook with a link to the worksheet that contains
    the rule.
  - The Quality Dimension set in IS for the rule.
  - The Table or View from which the failed records came.
  - The binding columns for the table (i.e., which column(s) contains
    the values that are evaluated by the rule).
  - The number of records that failed the rule.
  - A summary email contains a table that lists each of the rules with
    failed records, a record count, and a link to view details about
    each rule in the ISA.

In both the summary and attachment emails, the contents are translated
to the user-specified language if the catalog has been configured to
translate the contents and titles to the user-specified language. In the
summary sheet, all values can be translated. In the separate rule
binding sheets, the column heading description can be translated.

<span style="font-weight: bold;">NOTE:</span> If a rule is bound to a
single table on multiple fields, each binding generates a spreadsheet to
send as an attachment to users in the project distribution. The
spreadsheet contains data that failed the rule for each field-table
combination.

<span style="font-weight: bold;">NOTE:</span> If a rule has no failed
records, the rule does not display in workflow emails or in the Excel
file attached to workflow emails.
