# About Automate Events

Automate is delivered with several events, which are actions that
contain validation rules and/or business rules. They are associated with
an event type when registered to an interface. 

Use the following table as a reference when registering events in
Automate:

**Page**

**Event**

**Description**

**Interface Server: Parameters**

**CommandExec**

Runs a Windows Batch job.

**Wait**

Pauses the run of the Interface Job.

**Interface Server: File Operations**

**Execute**

Copies the files from the source folder to the target folder, but does
not create a separate Job in the Job Queue to run.

**FileIterator**

Copies files from a source folder to a target folder, then deletes the
files from the source folder.

**OnValidate**

This field is not used in Automate

**Process**

This field is not used in Automate

**Submit**

Same thing as Execute, but creates a separate Job in the Job Queue.

**Interface Server: Interfaces**

**Execute**

Executes the Interface, but does not create a separate Job in the Job
Queue to run.

**OnValidate**

This field is not used in Automate

**ProcessBackground**

Executes the Interface, but creates a separate Job in the Job Queue to
run it.

**Reset**

Updates the Interface Server Record nulling out the Run information.
This event is helpful if the Interface is in a non-successful status
(failed, running but does not stop).

**Submit**

Executes the Interface, but creates a separate Job in the Job Queue to
run the Interface Server Job.
