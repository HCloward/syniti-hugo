# Post Data to Multiple Target Systems with One Process Template

A Process Designer can reuse a process template by adding connections to
load programs for multiple target systems to a single process template.
Data can then be posted to these target systems sequentially.

At a high level, the user:

1.  [Specifies available connections at the process template
    level](Set_Connections_at_the_Process_Template_Level.htm).
2.  [Edits the connections to target systems at the process post
    level](Edit_Connections_to_Target_Systems_at_the_Process_Post_Level.htm)
    (if needed).

After a user adds a process, the system creates one process template for
that process automatically. The process template connection was added on
the <span style="font-style: italic;">Templates</span> page when the
template was created. This process template may need further
configuration depending on the template type.

A user adds an additional process template for each target system
connection. These process templates must be configured identically to
the first, except for the connection to the target system. When the
process is posted, the data is reused. The identical data is sent to
each target system.

For example, a user creates a BDC Script template with a connection to
SAP Application Server 1 and adds it to a process. The system creates a
process template automatically with a connection to SAP Application
Server 1. The user further configures this process template by setting
the primary key column name and adding fixed values and mapping values
to the process template loops.

The user then adds a second process template to the process, and
configures it identically to the first process template. The user sets
the connection to this process template to SAP Application Server 2.
After activating the process, the user posts the data, which updates
each of the target systems (SAP Application 1 and SAP Application 2)
with the same data.

Detailed information about the posting process is available in the
sections corresponding to the template type.

<span style="font-weight: bold;">NOTE</span>: Connections can be added
to a process template based on any template type. However, the types of
connections allowed are restricted based on the template type. For
example, a BODS Execution template only allows a connection to a Data
Services Repository. BDC Script and GUI Script template connections are
restricted to SAP Application Server data source types. Refer to the
[Data Source Registry page’s Vertical
View](../../Common/Page_Desc/Data_Source_Registry_H.htm#Data_Source_Registry_V)
for more information about these connections.

<span style="font-weight: bold;">NOTE</span>: There is no limit to the
number of process templates that can be created with different target
system connections.

<span style="font-weight: bold;">NOTE</span>: When a process is copied,
the allowed connections are also copied.

Begin by [setting available connections at the process template
level](Set_Connections_at_the_Process_Template_Level.htm).
