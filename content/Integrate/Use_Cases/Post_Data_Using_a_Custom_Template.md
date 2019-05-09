+++
title = 'Post Data Using a Custom Template'
solution = 'Platform'
+++

# Post Data Using a Custom Template

Custom templates provide the ability for a developer to post to
proprietary systems not supported by Integrate by providing a custom
implementation for the Process Template interface which Integrate can
execute.

A developer could use a custom implementation to allow dspConduct™ to
act as a Master Data Management HUB for the most complicated Enterprise
Architectures. For example, a custom implementation could be used to
build a custom plugin that is intended to load data into third party
on-premise or cloud systems.  Some custom systems, such as
SuccessFactors, Ariba, or Workday, need data elements captured in
dspConduct™ and federated to their cloud environments. The plugin to
call the web service or a custom plugin to load that data can be created
and brought into the Business Process in correlation with other targeted
systems of dspConduct™.  

A developer must create all of the associated files and code to support
the Custom template.

During template creation in Integrate, the user enters the assembly file
name (a .dll) and the Type File Name that is specific to the Custom
template.

To post using a Custom template:

  - [Create a Custom Assembly](Create_a_Custom_Assembly)
  - [Add the Assembly File to the Integrate Process
    Folder](Add_the_Assembly_File_to_the_Integrate_Process_Folder)
  - [Create a Custom Template](Create_a_Custom_Template_Integrate)
  - [Activate the Custom Template](Activate_the_Custom_Template)
  - [Add the Custom Template to a
    Process](Add_the_Custom_Template_to_a_Process)
  - [Activate the Process](Activate_the_Process_Custom_Template)
  - [Post Data](Post_Data_Custom_Template)
