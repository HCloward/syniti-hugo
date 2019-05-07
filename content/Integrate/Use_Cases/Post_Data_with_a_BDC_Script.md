+++
title = 'Post Data with a BDC Script'
solution = 'Platform'
+++

# Post Data with a BDC Script

Integrate allows a user to post data to SAP using the results of a Batch
Data Communication (BDC) script recorded using either Integrate or the
SHDB transaction in  SAP (which is then imported into Integrate).

During initial template creation, the user selects the SAP system
against which the script will be created and the SAP transaction code
being recorded by the BDC script.

A template defines how data is posted into SAP, including which screens
and fields will be processed and whether the process contains a single
loop or multiple loops. Templates are not tied to data, but rather act
as an independent guide for posting that can be assigned to many
processes.

**NOTE**: A BDC Script template can also be created by copying a
template. Refer to [Copy a Template](Copy_a_Template.htm) for more
information. Integrate allows the screens in a BDC Script template to be
merged with another BDC Script template. Refer to [Merge or Copy BDC
Screens to Another BDC Script
Template](MergeCopyBDCScrnsAnotherBDCScript.htm) for more information.

A process, a series of posting steps, defines how Integrate takes data
from the platform and transfers it to SAP. Each posting step is a
template that is added to the process.

Once assigned to a process, the BDC Script template can be further
configured to include transaction stringing, template process loops tied
to different views that contain the data to post to SAP, and field
mappings to a specified field value or a fixed value. Integrate can also
map many fields in the template with columns in an assigned view
automatically.

After the process is configured and activated, use a process post to
send the data to SAP.

<span id="Post Data using a BDC Script Steps" class="popUpLink">\>Review
the steps in the process. </span>
