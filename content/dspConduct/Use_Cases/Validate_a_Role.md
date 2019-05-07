+++
title = 'Validate a Role'
solution = 'Master Data Management'
+++

# Validate a Role

A Role Processor can run a validation process for a Request Role prior
to finishing the role to validate the tasks for a role using the
validations rules registered to a pages associated to the tasks. For
each of the pages (including child pages) corresponding to the tasks,
the process executes the validation views that have been registered to
the pages. Any errors, warnings, or messages that result are displayed
in a pop-up on the page.

If there are errors when the Role Processor clicks the Validate icon,
the BOA Status is set to Failed. The errors must be corrected on the
page before the request role can be finished.

The validation process runs automatically when a role is finished (the
Role Processor clicks the Finish icon). If there are validation errors
when the Role Processor clicks Finish, the process stops and subsequent
rules are not executed. The Role Processor must fix the errors on the
page before finishing the request. If no errors are encountered the
stored procedures and other plugins are run to perform the Finish event.

**NOTE:** Validations are not run for the Post role.

To validate a role in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Requests** in the *Navigation* pane.
2.  Click the **Roles** icon for a request.
3.  Click **Validate**.
