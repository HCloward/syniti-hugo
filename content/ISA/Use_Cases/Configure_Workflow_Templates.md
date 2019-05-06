# Configure Workflow Templates

Workflow emails are sent to users that contain information about data
that failed IS rules. The information can be accessed through:

An attachment to the email in the form of an Excel file

A summary email with a table listing the rules and number of failed
records for each rule for a project distribution

An email with a link to the information in the ISA and a link to the
scorecard in IS to view the progress of error resolution.  

Refer to [Attachments and Summaries](Summaries_and_Attachments.htm) for
more information.

A user’s workflow options set the type of email each user will receive.
Refer to [Configure Workflow Options](Configure_Workflow_OptionsISA.htm)
for more information.

The types of templates for workflows that can be configured are:

  - A generic template for attachment emails set at the parameter level
  - A generic template set for summary emails at the parameter level
  - A template for attachment emails at the project level
  - A template for attachment emails at the project distribution level

**NOTE**: Summary workflows are sent at the user level only. Summary
emails will not be sent to all users in a project distribution, unless
all users in that project distribution have selected to receive
summaries as a workflow option.

**NOTE:** Workflow email templates can be configured at the
[parameter](Configure_Workflow_Templates_at_the_Parameter_Level.htm),
[project](Configure_Workflow_Templates_at_the_Project__Level.htm), or
[project
distribution](Configure_Workflow_Templates_at_the_Project_Distribution_Level.htm)
level to allow emails to be customized for all users in the ISA, all
users in a project, or all users in a project distribution.

**NOTE:** When the ISA applies templates, a user’s project
distribution-level template is applied by default. If no project
distribution-level template exists, the project template is applied. If
no project-level template exists, the parameter-level template is
applied to the user’s workflow template.

**NOTE:** If the templates at the parameter, project distribution and
project level are deleted (an unlikely scenario), a template is
installed with the platform that can be used. This template’s language
is English and the language cannot be changed (i.e., the template cannot
be translated).
