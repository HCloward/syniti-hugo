+++
title = 'BDC Post Methods and Settings on the Advanced tab'
solution = 'Platform'
+++

# BDC Post Methods and Settings on the Advanced tab

If the process post is based on a process with a single BDC Script
template, a user can select from any of the options in the **BDC Post
Method** list box on the **Advanced** tab of the *Process Post* page’s
*Vertical* View. A process post with multiple templates, or one that is
based on a template type other than BDC Script, can only use the
**StandardSAPPosting** BDC Post Method.

Methods available for a process post based on a single BDC Script
template include:

  - **BOAFileCreation** – Creates files on the web server that can be
    used in the /BOA/ZBDCPROCESS program in SE38.
  - **BOAPosting** – Posts immediately using the BOA Function
    Module.
  - <span style="font-weight: bold;">B**OAPostingWithErrorSessionCreation**</span>
    – Posts immediately using the BOA Function Module and creates an
    SM35 session with any errors. The error session contains only the
    records that failed to post, successful transactions are not
    included.
  - **BOASessionCreation** – Uses the BOA Function Module to create an
    SM35 session containing all of the data in the process post, but
    does not post the data to SAP.
  - **StandardSAPPosting** – Posts using the standard SAP Function
    Modules.

Depending on the BDC Post Method selected, certain settings on the
**Advanced** tab should not be used. For example, any process post using
**StandardSAPPosting** will not use any settings in the **BOA Function
Module Upload Options** section or in the **BOA BDC File Options**
section.

Only process posts using the **BOAFileCreation** BDC Post Method should
use the settings in the **BOA BDC File Options** section.

*[View the field descriptions for the Process Post page’s Vertical View
for detailed information.](Process_Post_H#Process_Post_V_All_Tabs)*

The following table lists which settings should be used based on BDC
Post Method and other factors.

  

BDC Post Method

BOAFileCreation

BOAPosting

BOAPostingWithErrorSessionCreation

BOASessionCreation

StandardSAPPosting

For a process post based on:

Single BDC Script template

Single BDC Script template

Single BDC Script template

Single BDC Script template

All template types

Process with multiple templates

Advanced Post Settings

 

Batch size

 

 

 

 

X

User Name

X

X

X

X

X

Password

X

X

X

X

X

Comment

X

X

X

X

X

Transfer Files to Data source

NOTE: Used with User Defined Template Types only.

 

 

 

 

X

Debug and Test Options

 

Start Template Priority

NOTE: Used with a process with multiple templates assigned.

 

 

 

 

X

End Template Priority

NOTE: Used with a process with multiple templates assigned.

 

 

 

 

X

Create GUI Debug Script

NOTE: Used only with GUI Script template.

 

 

 

 

X

BOA Function Module Upload Options

The settings in this section are not used when the BDC Post Method is
StandardSAPPosting.

Keep Session

 

 

X

X

 

Continue on Commit

X

X

X

X

 

No Data Symbol

X

X

X

X

 

Group Name

X

X

X

X

 

BOA BDC File Options

The settings in this section are only used when the BDC Post Method is
BOAFileCreation.

Session File Path

X

 

 

 

 

Session File Name

X

 

 

 

 

File Split Interval

X
