+++
title = 'OnValidate Events'
solution = 'Platform'
+++

# OnValidate Events

OnValidate events run:

  - after an insert
  - after an edit
  - when boaStatus changes

Determine which of these are actually relevant to the business logic and
what can be done to ensure complex logic only runs when necessary.

Refer to [Create Events](Create_Events.htm) for general information.

Compromising Between Implicit Behavior and Excess Overhead

It is easy to overload computation and configuration logic onto an
OnValidate event, because it requires the least amount of effort to
ensure the logic runs as often as it needs to. However, this can
introduce complexity problems at run time.

An extreme example is on the *[Data
Sources](../Sys_Admin/Page_Desc/Data_Sources_HSysAdmi.htm)* page in
System Administration. An OnValidate Business rule exists, which
attempts to create system views in the database. The Business rule runs
if the System Views check box is checked on the *Vertical* View of the
*Data Sources* page. If the data source is accidentally configured with
invalid connection information, every time an update is saved, the DSP
attempts to connect to the data source and prepare to create system
views. After 30 seconds, a timeout error occurs. This frustrates users,
because saving even a small change takes 30 seconds each time and then
results in an error.

To avoid this potential problem, alter the logic of the Business rule
event to check if the rule is meant to create the system views prior to
attempting to access the database.

Instead of using an OnValidate event that runs every time the user saves
changes, a designer could create a “Create System Views” or “Check
System Views” button, which would run the Business rule only when
needed. Updates to the database would be fast and without timeout
errors.

One extra click to save 200ms per edit can significantly mitigate users'
frustration.

Minimize Work by using Keys or Drill column values

Never perform “Global” operations using OnValidate. The OnValidate event
must run on the current record being validated only, and not on all
records on a page. If an event must run on every record in the page, you
can create a button in the toolbar that executes against all records
when clicked.

There are use cases where a child record affects a parent record, but it
is still utilizing data from the child row for that manipulation. That
operation should only affect one record (the parent) by filtering the
affecting SQL with column values passed through the navigation of pages.
