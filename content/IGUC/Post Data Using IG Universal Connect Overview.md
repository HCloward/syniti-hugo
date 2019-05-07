+++
title = 'Post Data Using IG Universal Connect Overview'
solution = 'Platform'
+++

# Post Data Using IG Universal Connect Overview

A Template defines how data is posted to a Target system, including
which Target system screens and fields are processed. Every Template has
a Template type. The IG Universal Connect Template type uses a Boomi
Process when posting data to a Target system.

IG Universal Connect allows a connection with many systems, such as
Salesforce or Workday, as defined by the connector associated with a
Boomi Process. The Boomi Process also has an associated atom, the
default execution environment (for example, Dev, QA and Prod).

**NOTE**: The atom can be changed at the Process Template level. Refer
to [Update the Connection for a Process
Template](Update%20the%20Connection%20for%20a%20Process%20Template.htm)
for more information.

The connection ID configured at the Template level on the
*[Template](../Integrate/Page_Desc/Template_H.htm)* page’s *Horizontal*
View determines the IG Universal Connection the Template uses. Refer to
[Register a Data Source in
Common](../Common/Use_Cases/Register_a_Data_Source_in_Common.htm) for
more information.

If parameters, an optional feature, are to be used as inputs to a Boomi
Process when posting data, a view must be created in SQL Server. The
view serves as the basis of Process Template Loop Field Mappings, which
connect a column in a view with a field on a Template.

A user can create this view using the Auto Generate Database Objects
feature. Refer to [Generate Database Objects
Automatically](../Integrate/Use_Cases/Generate_Database_Objects_Automatically.htm)
for more information. Views can also be created manually. Refer to
[Create a View in SQL
Server](../Integrate/Use_Cases/Create_a_View_in_SQL_Server.htm) for more
information.

**NOTE**: When a Process based on an IG Universal Connect Template type
is posted, Integrate applies the Where clause from the Process post
(entered on the *[Process
Post](../Integrate/Page_Desc/Process_Post_H.htm)* page’s *Vertical*
View), and runs the tx\*Int view mapped at the Process – Template – Loop
level. For each record found, Integrate calls the Boomi Process with the
parameter values (if applicable) from the tx\*Int view.

**NOTE**: When Integrate executes a Boomi process, it passes in the
LinkID for the execution, which is used to return a status to the DSP®
once the execution is complete. **The user must add any additional
parameters required for the process.**

Standard Integrate features are available for IG Universal Connect.
Refer to the following topics for more information.

  - [Register After Post Rules to a Process
    Template](../Integrate/Use_Cases/Register_After_Post_Rules_to_a_Process_Template_Overview.htm)
  - [Post Data to Multiple Target Systems with One Process
    Template](../Integrate/Use_Cases/Post_Data_to_Multiple_Target_Systems_with_One_Process_Template.htm)
  - [Post a Process with Multiple
    Templates](../Integrate/Use_Cases/Post_a_Process_with_Multiple_Templates.htm)

When posting request data using this Template type, at a high level, a
Template Administrator:

  - [Creates a Template with the IG Universal Connect Template
    type.](Create%20an%20IG%20Universal%20Connect%20Template.htm)
  - [Activates the Template.](Activate%20the%20Template%20IGUC.htm)
  - [Adds the Template to a
    Process.](Add%20the%20Template%20to%20a%20Process%20IGUC.htm)

If using parameters:

  - [Configures a Process Template Loop for an IG Universal Connect
    Process Template
    Manually.](Configure%20a%20Process%20Template%20Loop%20for%20an%20IG%20Universal%20Connect%20Process%20Template%20Manually.htm)
  - [Configures a Process Template Loop for an IG Universal Connect
    Process Template
    Automatically.](Configure%20a%20Process%20Template%20Loop%20for%20an%20IG%20Universal%20Connect%20Process%20Template%20Automatically.htm)
  - [Configures Field Mappings for an IG Universal Connect Process
    Template.](Configure%20Field%20Mappings%20for%20an%20IG%20Universal%20Connect%20Template.htm)

The Template Administrator then:

  - [Activates the Process.](Activate%20the%20Process%20IGUC.htm)
  - [Posts Data Using the Boomi
    Process.](Post%20Data%20Using%20IG%20Universal%20Connect.htm)
