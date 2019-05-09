+++
title = 'Set up After Post Rules to Check for Failed Posts for BAPI or RFC Processes'
solution = 'Platform'
+++

# Set up After Post Rules to Check for Failed Posts for BAPI or RFC Processes

After posting a request based on an Integrate process that uses BAPIs or
RFCs, the posting process may return a Message Type of success even if
data did not post correctly.

In this case, a validation view or a stored procedure in SQL can be
written to detect posting failure messages in the Output/Download
table(s) that Integrate created for the BAPI or RFC.  

<span style="font-weight: bold;">NOTE</span>: This documentation does
not provide steps for working in SQL.

If using a validation view, only one validation view can be registered
for an Integrate process template. This view must include the PostingID
found in the ttRequestIntegrateProcess table and the Download table.

Refer to [Register a Status View as an After Post
Rule](Register_a_Status_View_as_an_After_Post_Rule) for more
information.

A stored procedure to gather and pass messages may be required for
complicated BAPIs that have multiple Download/Output tables. An After
Post Rule stored procedure only receives the “PostingID” parameter.
Refer to [Register a Stored Procedure as an After Post
Rule](Register_a_Stored_Procedure_as_an_After_Post_Rule) for more
information.

The stored procedure can read the RequestID and other required values
out of the ttRequestIntegrateProcess table by searching for that
PostingID value.

Inside the stored procedure call the API stored procedure found in
dspConduct™ database apiPostRuleMessageIns. This stored procedure
requires the PostingID and a RecordSuccess.  RecordSuccess can be set to
a value of 0 (zero) to indicate a failure or 1 (one) to indicate a
success.  

The following parameters are optional (and may be available in the BAPI
Output/Download table depending on the BAPI):

  - RecordID
  - Message
  - MessageType
  - Comment
  - ReturnValue1
  - ReturnValue2
  - ReturnValue3
  - ReturnValue4
  - PrimaryKey

Any records passed with a RecordSuccess of 0 result in a request's
posting status of "Failed."
