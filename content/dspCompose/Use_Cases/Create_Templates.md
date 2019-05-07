+++
title = 'Create Templates'
solution = 'Data Quality'
+++

# Create Templates

A template represents a process that will be governed and executed using
dspCompose™.

All templates must belong to a team. Refer to [Create
Teams](Create_Teams.htm) for more information.

## Template Types

  - **BDC and GUI script templates** contain an SAP recording and can be
    reused for multiple requests. Scripts can either be recorded in SAP
    directly from dspCompose™ or imported from Integrate. Refer to
    [Create a GUI Script Template](Create_a_GUI_Script_Template.htm) and
    [Create a BDC Script Template](Create_a_BDC_Script_Template.htm) for
    more information.
  - **Templates based on Integrate templates** — dspCompose™ templates
    can also work with BDC or GUI scripts with multiple loops enabled.
    Refer to [Use dspCompose™ with Integrate Looped
    Templates](Use_dspCompose_with_Integrate_Looped_Templates.htm) for
    more information.
  - **Custom templates** Refer to [Create a Custom
    Template](Create_a_Custom_Template_dspCompose.htm) for more
    information.

Advanced users access configuration settings to customize the template
by adding the template on the *Templates* page. Refer to [Create a
Template for Advanced
Users](Create_a_Template_from_the_Templates_Page.htm) for more
information.

The user who creates the template has access to all of the template
roles and can add users to the template roles. Refer to [Add Users to
Templates](Add_Users_to_Templates.htm) for more information.

Once a template has been created and generated, a user can view all of
the associated data objects dspCompose™ created for the template. Refer
to [View Data Objects](Data_Objects.htm) for more information.

## <span id="dspCompose_and_Integrate"></span>dspCompose™ and Integrate

Once a template is created and generated in dspCompose™, it is added to
the **dspCompose** category in Integrate.

Integrate also creates

  - A process based on the template
  - A loop in the process template with the Mapping Value for each field
    mapping automatically populated

A process template loop assigns a view from the process’s data source to
a loop within the template. The loop is mapped to a view that contains
the data to post for the corresponding template loop in the process.

Deleting a dspCompose™ template in dspCompose™ removes the dspCompose™
template and process from Integrate.

This section contains the following topics:

  - [Create Teams](Create_Teams.htm)
  - [Create a BDC Script Template](Create_a_BDC_Script_Template.htm)
  - [Create a GUI Script Template](Create_a_GUI_Script_Template.htm)
  - [Create a Custom Template](Create_a_Custom_Template_dspCompose.htm)
  - [Create a Template from an Integrate
    Template](Create_a_Tempate_from_an_Integrate_Template.htm)
  - [Create a Template for Advanced
    Users](Create_a_Template_from_the_Templates_Page.htm)
  - [Data Objects](Data_Objects.htm)

Once a template is created, it requires additional configuration by the
Template Administrator. Refer to [Configure
Templates](Configure_Templates.htm) for more information.
