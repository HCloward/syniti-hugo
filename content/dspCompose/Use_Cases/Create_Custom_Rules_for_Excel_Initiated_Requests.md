# Create Custom Rules for Excel-initiated Requests

dspCompose™ allows a Template Administrator to register custom rules
<span> </span>that will run when a template-level event occurs. A rule
is set to run when a request is cancelled, created, deleted, or posted
based on how that request’s template is configured.

A rule can also be registered to the Request Excel Create event for
Excel-initiated requests. Once an external contact sends an Excel file
to dspCompose™ and the Excel file passes the initial validations, the
request data is loaded into a staging table. Rules can then be run on
the data before it is moved to the table used for the Data Entry role
for the request.

These custom rules must exist in a data source that is registered to the
platform (often in the cMass\_Data database), and be registered to the
template-level event on the *Template (Event Rule)* page.

Refer to [Register Rules to Template-level
Events](Register_Rules_to_Template%20level_Events.htm) for details on
how to create custom rules for Excel-initiated requests.
