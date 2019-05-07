+++
title = 'Start to Finish'
solution = 'Platform'
+++

# Start to Finish

This dependency type dictates that work on the predecessor task must
have started before work on the dependent task can finish.

A user clicks Next Action on the Work List to move the predecessor Plan
Task from Ready to In Progress status. Work on the dependent task may
have already begun, but the user cannot move the task status from In
Progress to Completed until the predecessor task has a status of In
Progress.

When setting a Start to Finish dependency type, the planned start date
for the predecessor task must be earlier than the Planned finish date
for the dependent task. If the dates are not set correctly, an error
message displays when saving the dependency on the *Plan Task
Dependency* page.
