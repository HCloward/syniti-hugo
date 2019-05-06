# Post Data Using an SAP Data Services Job Overview

A template defines how data is posted to a target system, including
which target system screens and fields are processed. Every template has
a template type. The SAP Data Services Job template type uses a Data
Services Job (consisting of a Data Services Repository and a job name)
when posting request data to a target system.

The Data Services Job associated with the template type is stored in a
Data Services Repository, a set of tables that stores user-created and
predefined system objects, source and target metadata, and
transformation rules. Repositories are configured in SAP Data Services,
and then registered in Common in the DSP®.

The connection ID configured at the template level on the
[Template](../Page_Desc/Template_H.htm) page’s
<span style="font-style: italic;">Horizontal</span> View determines the
Data Services Repository the template uses. Refer to [Register a Data
Source in
Common](../../Common/Use_Cases/Register_a_Data_Source_in_Common.htm) for
more information.

After a user has added the job name on the
[Template](../Page_Desc/Template_H.htm) page’s
<span style="font-style: italic;">Vertical</span> View, this job is
created and stored in the repository.

If Global Variables, an optional feature, are to be used as inputs for a
Data Services Job used to post data to SAP, a view must be created in
SQL Server. The view serves as the basis of Process Template Loop Field
Mappings, which connect a column in a view with a field on a template.

A user can create this view using the Auto Generate Database Objects
feature. Refer to [Generate Database Objects
Automatically](Generate_Database_Objects_Automatically.htm) for more
information. Views can also be created manually. Refer to [Create a View
in SQL Server f](Create_a_View_in_SQL_Server.htm)or more information.

<span style="font-weight: bold;">NOTE</span>: When a process based on a
SAP Data Services Job template type is posted, Integrate applies the
Where clause from the process post (entered on the [Process
Post](../Page_Desc/Process_Post_H.htm) page’s
<span style="font-style: italic;">Vertical</span> View), and runs the
tx\*Int view mapped at the Process – Template – Loop level. For each
record found, Integrate calls the Data Services Job with the Global
Variables values (if applicable) from the tx\*Int view.

When posting request data using this template type, at a high level, a
Template Administrator:

  - [Creates a template with the SAP Data Services Job template
    type.](Create_an_SAP_Data_Services_Job_template.htm)

  - [Activates the template.](Activate_the_Template_DS_Job.htm)

  - [Adds the template to a
    process.](Add_the_Template_to_a_Process_DSJob.htm)

  - If using Global Variable:
    
      - [Configures a Process Template Loop for a SAP Data Services Job
        Process Template
        Manually](Configure_a_Process_Template_Loop_for_a_SAP_Data_Services_Job_Process_Template_Manually.htm).
      - [Configures a Process Template Loop for a SAP Data Services Job
        Process Template
        Automatically](Configure_a_Process_Template_Loop_for_a_SAP_Data_Services_Job_Process_Template_Automatically.htm).
      - [Configures Field Mappings for an SAP Data Services Job Process
        Template](Configure_Field_Mappings_for_an_SAP_Data_Services_Job_Process_Template.htm).

  - [Activates the process.](Activate_the_Process_DS_Job.htm)

  - [Posts data using an SAP Data Services
    Job.](Post_Data_Using_an_SAP_Data_Services_Job.htm)
