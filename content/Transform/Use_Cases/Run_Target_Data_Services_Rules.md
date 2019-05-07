+++
title = 'Run Target Data Services Rules'
solution = 'Migration'
+++

# Run Target Data Services Rules

DSP® registers the Data Services jobs against the Target in Transform as
Data Services rules. When a Data Services Repository is registered with
an object, the Data Services Rules and Data Services Reports icons
become active on the *[Targets](../Page_Desc/Targets_H.htm)* page in
Transform.

Jobs are registered automatically unless they are running against a
utility Target, which is a Target that does not exist in the Target
system used to register rules and reports in Transform. A Target is
designated as a utility Target on the
*[Targets](../../Design/Page_Desc/Targets_H_Design.htm)* page in Target
Design (Design \> Targets). In this case, the job runs as either a
preprocessing or a post process task. As an example, preprocessing could
include duplication of a data set and post processing could include the
post load validation of data to ensure it has loaded correctly into the
Target system.

Jobs are inactive by default and the user must activate the jobs in
Transform before they can be executed in Data Services by processing the
specific Data Services rule or whole Target in Transform.

When the Data Services jobs are run in Transform, the Data Services Web
Service layer is called, calling the job and parsing in the parameters
from the global variables. Running the job in Transform provides the
ability to build Data Services reports, which can show whether there are
errors in the data or where enrichments have been applied.

The output of the validations performed by the Data Services Jobs are
written to a single TT\_RULE\_VIOLATION table and a
TT\_RULE\_VIOLATION\_VALUES table that allows reports to be written for
each Target. The reports provide the information on which validations
have failed and what is required of the end user to action and resolve
the data issues. For example, not finding a value mapping value in the
Target system configuration would mean that either the Target system
must be updated to include the value or a value must be remediated to
one that does exist.

**NOTE:** The global variables may be updated prior to executing Data
Services jobs. Refer to [Configure Target Data Services Rule Global
Variables](Configure_Target_DS_Rule_Global_Var.htm).

<span style="font-weight: bold;">NOTE:</span> For the Data Services
options and pages to be available, the Data Service Repository must be
registered in Common. Refer to [Register a Data Source in
Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
for more information.

<span style="font-weight: bold;">NOTE:</span> The status for the Data
Services rule must be Active before it can be executed in Data Services.

Target rules can be run in the foreground or background.

**NOTE:** If a process takes less than 0.5 seconds to run, the duration
in the DURATION field is 0.

Run a rule in the background if there is a large amount of data to
process that may affect system performance or may time out a session.
Monitor rules that run in the background on the
*[Monitor](../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm)*
page.

To run a Target Data Services rule in the foreground in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.

2.  Click the **Data Services Rules** icon for a Target.
    
    **NOTE:** This icon displays if a Data Services repository has been
    set at the object level. Refer to [Configure Data Services
    Functionality](../../Console/Config/Configure_Data_Services_Functionality.htm)
    for more information.

3.  Click the **Execute** icon in the Page Toolbar in the child pane.

To run a Target Data Services rule in the background in Transform:

1.  Click the **Process Information** tab on the *Vertical* View of the
    *[Target Data Services
    Rules](../Page_Desc/Target_Data_Services_Rules_H.htm)* page.
2.  Click the **Process** icon; a confirmation message displays.
3.  Click **OK**.

Additional features are available for Target Data Services rules:

  - **Reset** – Resets the processing status if the process fails for
    any of the Target rules. This option is available on the
    *Horizontal* View only.
  - **Queue** – Allows monitoring of background job processes for Target
    rules. This option is available on the Horizontal View only.
