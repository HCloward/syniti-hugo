# Create Custom Rules for Information Steward-initiated Requests

Rules are stored procedures that have been written and saved in a data
source that is registered in the DSP®. A rule runs during a process to
manipulate data, perform an extra step in the process, or finish a task
the process starts. For example, a rule could dictate that once table A
has been populated with 1000 rows of data, that data is archived in
table B and removed from table A.

dspCompose™ allows a Template Administrator to register custom rules
that will run when a template-level event occurs. A rule is set to run
when a request is cancelled, created, deleted, or posted based on how
that request’s template is configured.

A rule can also be registered to the Request ISA Create event for
requests that are initiated by an Information Steward report. Once an
event occurs in Information Steward to create a dspCompose™ request, the
request data is loaded into a staging table. Rules can then be run on
the data before it is moved to the table used for the Data Entry role
for the request.

These custom rules must exist in a data source that is registered in the
platform (often in the cMass\_Data database), and be registered to the
template-level event on the <span style="font-style: italic;">Template
(Event Rule)</span> page.

Refer to [Register Rules to Template-level
Events](../../dspCompose/Use_Cases/Register_Rules_to_Template%20level_Events.htm)
for details on how to create custom rules for Information
Steward-initiated requests.
