+++
title = 'Post Using RFC Execution'
solution = 'Platform'
+++

# Post Using RFC Execution

Integrate supports the execution of any RFC enabled Function Module in
SAP, including the execution of RFCs and the posting of data via BAPIs.

Refer to [*<span style="color: #0000ff;font-style: normal;">Post Data
Using a</span>* BAPI](Post_Data_Using_a_BAPI.htm) for more information.

**NOTE**: Before creating an RFC template, the RFC functions must be
extracted from SAP in Common. Refer to
*[<span style="color: #0000ff;font-style: normal;">Establish an SAP
Connectio</span><span style="color: #0000ff;">n</span>](../../Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)*
and [Extract RFC Functions](../Config/Extract_RFC_Functions.htm) for
more information.

A process based on an RFC template will post data bi-directionally. Data
is uploaded to be posted into SAP, and downloaded into tables that
Integrate automatically creates.  Since processes based on RFC templates
often have return values, download registrations are often required for
RFC templates. 

**NOTE**: RFC template types can use transaction stringing to pass
return values to other templates assigned to a process. Refer to
[*<span style="color: #0000ff;font-style: normal;">Post Data Using
Transaction
Stringing</span>*](Post_Data_Using_Transaction_Stringing.htm) for more
information.

**NOTE**: Integrate is an automation tool that allows experienced SAP
users to leverage data loading capabilities provided by SAP.  knowledge
of how to use SAP in regards to BAPIs, BDC, RFCs and others is required
to use Integrate and the documentation and technical support included
does not cover specific usage details or how these technologies work.
This use case provides an example of posting using the RFC
<span style="font-family: &#39;Times New Roman&#39;, serif;">BOA/ZRFC\_READ\_TABLE
– External access to R/3 tables via RFC</span>, but does not supply
comprehensive instructions to suit all RFCs.

<span id="Post Data using an RFC Steps" class="popUpLink">\>Review the
steps in the process. </span>
