+++
title = 'Final Finish Process for a Request Overview'
solution = 'Data Quality'
+++

# Final Finish Process for a Request Overview

As part of the Final Finish process, dspConduct™ downloads the data
posted by a request to tables in a target database (usually dgSAP.) The
data downloads using a CranPort package or a Data Services job.

The Final Finish process begins when a Role Processor clicks Finish for
the Post role on the [Request Role](../Page_Desc/Request_Role_H.htm)
page. Refer to [Finish a Role for the Post Role
Type](Finish_a_Role_with_the_Post_Role_Type.htm) for more information.

A Designer must register the Final Finish table(s) or job at the task
level.

When using a CranPort package, individual tables must be registered for
download. For a Data Services job, register a job only, or a job per
table. The Designer must know which tables or jobs are used.

Tables and jobs are registered for download at the Task level for main
Task parent pages only and must not be registered for child pages.

Main Task parent pages are listed as Role Tasks. Child pages are pages
that are accessed through links on a main Task parent page. For example,
register tables on the Request (Address – General) page but not on the
Request (Address – Telephone/Mobile) page.

<span style="font-weight: bold;">NOTE</span>: For new requests that are
automatically created as part of a multi-scenario business process, the
Content Request page OnValidate event is automatically executed. The
Cransoft UserID 'process' must have access to the Content Request page
in order to execute the OnValidate event.

The section includes these topics:

  - [Business Process Execution with Scenario Dependencies During Final
    Finish](Business_Process_Execution_with_Scenario_Dependencies_During_Final_Finish.htm)
  - [Business Process Execution During Final
    Finish](Business_Process_Execution_During_Final_Finish.htm)
  - [Configure Data Download During the Final Finish Process to use a
    CranPort
    Package](Configure_Data_Download_During_the_Final_Finish_Process_to_use_a_CranPort_Package.htm)
  - [Create a Final Finish Where Clause for a CranPort
    Package](Create_a_Final_Finish_Where_Clause_for_a_CranPort_Package.htm)
  - [Configure Data Download During the Final Finish Process to use a
    Data Services
    Job](Configure_Data_Download_During_the_Final_Finish_Process_to_use_a_Data_Services_Job.htm)
  - [View Final Finish Download
    Messages](View_Final_Finish_Download_Messages.htm)
