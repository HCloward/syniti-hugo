+++
title = 'Configure Templates'
solution = 'Data Quality'
+++

# Configure Templates

A template represents a process that will be governed and executed using
dspCompose™. It may contain an SAP recording. Scripts can either be
recorded in SAP directly from dspCompose™ or imported from Integrate.
Templates can be reused for multiple requests.

A user can also create a custom template or base a dspCompose™ template
on an Integrate template.

Refer to [Create Templates](Create_Templates) for more information.

Once a template is created, it requires additional configuration by the
Template Administrator.

**NOTE**:Two databases and WebApps are installed when dspCompose™ is
installed: the cMass and cMass\_Data databases, and the dspCompose and
dspCompose\_Data WebApps. WebApp dspCompose and its database cMass
contain all the settings and validations that come with the installation
and should not be modified. Make all customizations and create data
validations in the dspCompose\_Data WebApp and database to prevent
customizations from being overwritten during any upgrades.

To configure a template, the template must be inactive or must be in
Developer Mode. Refer to [Modify an Active Template in Developer
Mode](Modify_an_Active_Template_in_Developer_Mode) for more
information.

To configure a template the following options are available:

  - [Add and Configure Template
    Roles](Add_and_Configure_Template_Roles)
  - [Configure Columns for File Generation and Data
    Entry](Configure_Columns_for_File_Generation)
  - [Add Org Units to
    Templates](Set_up_Org_Units#Add_Org_Units_to_a_Template)
  - [Link a Template to a Page](Link_a_Template_to_a_Page)
  - [Add Users to Templates](Add_Users_to_Templates)
  - [Set Validation Threshold](Set_Validation_Threshold)
  - [Configure Retention Parameters](Configure_Retention_Parameters)
  - [Assign Default Data Source and
    Views](Assign_Default_Data_Source_and_Views)
  - [Add a Data Source that Stores Views for
    Import](Add_a_Data_Source_that_Stores_Views_for_Import)
  - [Add a Rule to a Template Role
    Event](Add_a_Rule_to_a_Template_Role_Event)
  - [Register Rules to Template-level
    Events](Register_Rules_to_Template%20level_Events)
  - [Set Tables to Store Posting
    Feedback](Set_Tables_to_Store_Posting_Feedback)
  - [Set Force Reject Severity](Set_Force_Reject_Severity)
  - [Register Tables for Download as a Finish
    Process](Register_Tables_to_Download_as_a_Finish_Process_Using_Collect)
  - [Register Tables for Download through Data
    Services](Register_Tables_for_Download_through_Data_Services)
  - [Activate the Template](Activate_the_Template)
  - [Modify an Active Template in Developer
    Mode](Modify_an_Active_Template_in_Developer_Mode)
