+++
title = 'Post Data Using a BAPI'
solution = 'Platform'
+++

# Post Data Using a BAPI

Integrate supports the execution of any RFC enabled Function Module in
SAP, including the execution of RFCs and the posting of data via BAPIs.

Refer to [Post Using RFC Execution](Post_Using_RFC_Execution) for
more information about RFC execution.

**NOTE**: Before creating a template, ensure the RFCs and BAPIs for the
SAP connection have been downloaded.  Refer to [Extract RFC
Functions](../Config/Extract_RFC_Functions) for more information.

A process based on a BAPI template will post data bi-directionally. Data
is uploaded to be posted into SAP, and downloaded into tables that
Integrate automatically creates.  Since processes based on BAPI
templates often have return values, download registrations are often
required for BAPI templates. 

**NOTE**: BAPI template types can use transaction stringing to pass
return values to other templates assigned to a process. Refer to [Post
Data Using Transaction
Stringing](Post_Data_Using_Transaction_Stringing) for more
information.

**NOTE**: Integrate is an automation tool that allows experienced SAP
users to leverage data loading capabilities provided by SAP.  knowledge
of how to use SAP in regards to BAPIs, BDC, RFCs and others is required
to use Integrate and the documentation and technical support included
does not cover specific usage details or how these technologies work.
This use case provides an example of posting using
BAPI\_MATERIAL\_SAVEDATA, but does not supply comprehensive instructions
to suit all BAPIs.

<span id="Post Data using a BAPI Steps" class="popUpLink">\>Review the
steps in the process. </span>
