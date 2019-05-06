# Post Data Using a GUI Script

Integrate allows a user to post data to SAP using the results of a GUI
script recorded using the SAP Logon pad.

During initial template creation, the user selects the SAP system
against which the script will be created and the SAP transaction code
being recorded by the GUI script.

The user then records the GUI script during the template creation
process.

A template defines how data is posted into SAP, including which screens
and fields will be processed and whether the process contains a single
loop or multiple loops. Templates are not tied to data, but rather act
as an independent guide for posting that can be assigned to many
processes.

A process, a series of posting steps, defines how Integrate takes data
from the platform and transfers it to SAP. Each posting step is a
template that is added to the process.

Once assigned to a process, the GUI Script template can be further
configured to include transaction stringing, template process loops tied
to different views that contain the data to post to SAP, and field
mappings to a specified field value or a fixed value. Integrate can also
map fields in the template with columns in an assigned view
automatically.

After the process is configured and activated, use a process post to
send the data to SAP.

<span id="Post Data using a GUI Script Steps" class="popUpLink">\>Review
the steps in the process. </span>
