# Requests vs. Templates

A request is based on a single template and manages the data entry,
review and posting of data into a target ERP system such as SAP.

### Templates

A template represents a defined unit of work that can be performed in
the target system and is based on a BDC or GUI recording, an Integrate
template or a custom template (a template that is not recorded in SAP).

A template, like a small WebApp, has unique configuration, validation,
business rules, and workflows. It is highly customizable and can be
configured for complicated request scenarios.

Templates are recorded by users who are familiar with the target system
where the data is created or changed.

Template security can control user access to request data. Security can
be set at the user level, role level and Org Unit level.

Once a user saves a template, Integrate creates an Integrate process
based on the template.

### Requests

A request, typically used by business users, is a mass change data
process object that is created, approved and posted to a target ERP
system in a single batch.

A typical role processor does not require knowledge about how the data
is entered into the target system; that user enters, reviews, and posts
data for a request based on a template.

Requests are workflow-enabled, meaning that each user assigned to a role
in a request can receive a notification when the role has work assigned.
A workflow is a notification method sent from a component, in this
instance when a role is finished. When one stage of work (i.e., a role)
has been completed for a request, dspCompose™ sends an email notifying
all members of the next dependent role or roles that they have tasks to
complete. The email contains a link to trigger specific events and to
launch the relevant page in dspCompose™. Users assigned to the role also
receive a notification pop-up from within dspCompose™.
