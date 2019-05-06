# Run Rules and Send Workflows On Demand

A user can run rules and send workflows for all Project Distributions in
a project by clicking the **Process Project Rules** icon on the
*[Project Summary](../Page_Desc/Project_Summary_H.htm)* page. When the
user clicks this icon:

  - All rules and rule bindings with unprocessed run IDs are run for all
    project distributions in the selected project
  - Workflows are sent to all users in the project according to user
    settings on the *[Parameters](../Page_Desc/ISA_Parameters.htm)* page

To process all rules for project distributions in a project:

1.  Select **Information Steward Accelerator \> Project Summary** in the
    *Navigation* pane.
2.  Select a project.
3.  Click the **Process Project Rules** icon in the Page toolbar.

ISA also runs a service page every hour to check if IS has processed
rules and runs a service page every 10 minutes to send workflows if IS
has processed rules.

To process rules or send workflows immediately for all projects:

1.  Select **Information Steward Accelerator \> Configuration \>
    Parameters** in the *Navigation* pane.
2.  Click **Process Rules, Generate Summary Workflows,** or **Send
    Workflows** on the **General** tab.
