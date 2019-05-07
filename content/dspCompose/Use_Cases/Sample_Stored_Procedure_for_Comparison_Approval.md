+++
title = 'Sample Stored Procedure For Comparison Approval'
solution = 'Data Quality'
+++

# Sample Stored Procedure For Comparison Approval

These sample stored procedures are original and modified code for the
CompareIns stored procedure that must be registered to the Template Role
Event rule. Refer to [Register the CompareIns Stored
Procedure](Register_the_CompareIns_Stored_Procedure.htm) for more
information.

A user modifies the original code as needed for each client’s business
needs.

As shown in the sample original code of the stored procedure (below),
the commented section that starts after the “BEGIN” statement lists the
guidelines and the SQL Code that must be added to the modified code
between the “BEGIN” and “END” statements.

If a comparison approval for a request uses partial approvals, the user
should include additional code in the modified stored procedure.

This code displays below the comment

\--Delete logic needed to support partial approval  

in the modified stored procedure sample
below.

### Original Sample

 

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">USE</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">\[dspCompose\_Data\]</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">GO</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">/\*\*\*\*\*\*
Object:  StoredProcedure
\[dbo\].\[webAB\_BDC\_MM02Compare1CompareIns\]    Script Date:
8/8/2013 11:15:32 AM
\*\*\*\*\*\*/</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">SET</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #0000ff;">ANSI\_NULLS</span><span style="color: #0000ff;">ON</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">GO</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">SET</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #0000ff;">QUOTED\_IDENTIFIER</span><span style="color: #0000ff;">ON</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">GO</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">ALTER</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #0000ff;">PROCEDURE</span><span style="color: #008080;">\[dbo\]</span><span style="color: #808080;">.</span><span style="color: #008080;">\[webAB\_BDC\_MM02Compare1CompareIns\]</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">@RequestID</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #0000ff;">int</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;"> <span style="color: #0000ff;">AS</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">BEGIN</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">/\*
This Procedure is used for populating the ComparisonApproval page for a
Template.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  This
procedure must be modified to correctly populate table
ttAB\_BDC\_MM02Compare1Compare.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  ttAB\_BDC\_MM02Compare1Compare
should contain one record for each corresponding
record</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  in
the ttAB\_BDC\_MM02Compare1
table.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  Records
in ttAB\_BDC\_MM02Compare1Compare should contain the values currently in
SAP</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  for
the data inserted into
ttAB\_BDC\_MM02Compare1.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  The
following are guidelines for modifying this
procedure:</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  1)
Delete any records from ttAB\_BDC\_MM02Compare1Compare for the current
Request.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  2)
Delete any records from ttAB\_BDC\_MM02Compare1Compare where ID = an ID
retrieved by
the</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*       select
statement.  When requests are automatically created by partial rejection
of</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*       another
request, ID values will be duplicates of IDs inserted for the original
request.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  3)
Remove the SELECT statement delivered in this
procedure.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  4)
Insert into ttAB\_BDC\_MM02Compare1Compare by joining
ttAB\_BDC\_MM02Compare1
with</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*     all
source tables or views originally used to populate
ttAB\_BDC\_MM02Compare1.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*     --
Key fields should be populated from
ttAB\_BDC\_MM02Compare1Compare.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*     --
Data fields should be populated from the original
source(s).</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*     --
Limit the Select/Insert to the current
RequestID.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*/</span>

*<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">SELECT</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #ff0000;">''</span><span style="color: #0000ff;">WHERE</span>
1 <span style="color: #808080;">=</span>
0</span>*

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">END</span>

 

### Modified Sample

 

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">USE</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">\[dspCompose\_Data\]</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">GO</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">/\*\*\*\*\*\*
Object:  StoredProcedure
\[dbo\].\[webAB\_BDC\_MM02Compare1CompareIns\]    Script Date:
8/14/2013 2:18:42 PM
\*\*\*\*\*\*/</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">SET</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #0000ff;">ANSI\_NULLS</span><span style="color: #0000ff;">ON</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">GO</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">SET</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #0000ff;">QUOTED\_IDENTIFIER</span><span style="color: #0000ff;">ON</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">GO</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">ALTER</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #0000ff;">PROCEDURE</span><span style="color: #008080;">\[dbo\]</span><span style="color: #808080;">.</span><span style="color: #008080;">\[webAB\_BDC\_MM02Compare1CompareIns\]</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">@RequestID</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #0000ff;">int</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;"> <span style="color: #0000ff;">AS</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">BEGIN</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">/\*
This Procedure is used for populating the ComparisonApproval page for a
Template.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  This
procedure must be modified to correctly populate table
ttAB\_BDC\_MM02Compare1Compare.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  ttAB\_BDC\_MM02Compare1Compare
should contain one record for each corresponding
record</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  in
the ttAB\_BDC\_MM02Compare1
table.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  Records
in ttAB\_BDC\_MM02Compare1Compare should contain the values currently in
SAP</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  for
the data inserted into
ttAB\_BDC\_MM02Compare1.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  The
following are guidelines for modifying this
procedure:</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  1)
Delete any records from ttAB\_BDC\_MM02Compare1Compare for the current
Request.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*
 2) Delete any records from ttAB\_BDC\_MM02Compare1Compare where ID =
an ID retrieved by
the</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*        select
statement.  When requests are automatically created by partial rejection
of</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*        another
request, ID values will be duplicates of IDs inserted for the original
request.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  3)
Remove the SELECT statement delivered in this
procedure.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*  4)
Insert into ttAB\_BDC\_MM02Compare1Compare by joining
ttAB\_BDC\_MM02Compare1
with</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*     all
source tables or views originally used to populate
ttAB\_BDC\_MM02Compare1.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*
    -- Key fields should be populated from
ttAB\_BDC\_MM02Compare1Compare.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*     --
Data fields should be populated from the original
source(s).</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*     --
Limit the Select/Insert to the current
RequestID.</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">\*/</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">DELETE</span><span style="color: #0000ff;">FROM</span><span style="font-size: 9.5pt;font-family: Consolas;">  </span><span style="color: #008080;">ttAB\_BDC\_MM02Compare1Compare</span><span style="color: #0000ff;">WHERE</span><span style="font-size: 9.5pt;font-family: Consolas;">
</span><span style="color: #008080;">RequestID</span><span style="font-size: 9.5pt;font-family: Consolas;"></span><span style="color: #808080;">=</span><span style="font-size: 9.5pt;font-family: Consolas;">
</span><span style="color: #008080;">@RequestID</span>

 

<span style="color: #008080;">-</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008000;">-Delete
logic needed to support partial
approval </span><span style="font-size: 10.5pt;color: #333333;">  
</span><span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">DELETE
FROM</span><span>  </span> <span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">ttAB\_BDC\_MM02Compare1Compare</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">WHERE</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #008080;">ID</span><span style="color: #0000ff;">IN</span><span style="color: #008080;">(</span><span style="color: #0000ff;">SELECT</span><span style="color: #008080;">ID</span><span style="color: #0000ff;">FROM</span></span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">ttAB\_BDC\_MM02Compare1</span><span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">WHERE</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #008080;">RequestID
=
@RequestID)</span></span>

 

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">INSERT</span><span style="color: #0000ff;">INTO</span><span style="font-size: 9.5pt;font-family: Consolas;"></span><span style="color: #008080;">ttAB\_BDC\_MM02Compare1Compare</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">(</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">\[ID\]</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">\[RequestID\]</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">\[RMMG1-MATNR\]</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">\[MARA-BISMT\]</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">\[MARA-EXTWG\]</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">\[MARA-LABOR\]</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">\[MARA-BEGRU\]</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">\[MARA-BRGEW\]</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">\[MARA-GEWEI\]</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">\[MARA-NTGEW\]</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">\[MARA-WRKST\]</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">)</span>

 

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">SELECT</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dbo</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #008080;">ttAB\_BDC\_MM02Compare1</span><span style="color: #808080;">.</span><span style="color: #008080;">ID</span><span style="color: #808080;">,</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dbo</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #008080;">ttAB\_BDC\_MM02Compare1</span><span style="color: #808080;">.</span><span style="color: #008080;">RequestID</span><span style="color: #808080;">,</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dbo</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #008080;">ttAB\_BDC\_MM02Compare1</span><span style="color: #808080;">.</span><span style="color: #008080;">\[RMMG1-MATNR\]</span><span style="color: #808080;">,</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dgSAP</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dbo</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">MARA</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">BISMT</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dgSAP</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dbo</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">MARA</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">EXTWG</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dgSAP</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dbo</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">MARA</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">LABOR</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dgSAP</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dbo</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">MARA</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">BEGRU</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dgSAP</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dbo</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">MARA</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">BRGEW</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dgSAP</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dbo</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">MARA</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">GEWEI</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dgSAP</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dbo</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">MARA</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">NTGEW</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">,</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dgSAP</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">dbo</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">MARA</span><span style="font-size: 9.5pt;font-family: Consolas;color: #808080;">.</span><span style="font-size: 9.5pt;font-family: Consolas;color: #008080;">WRKST</span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">FROM</span><span style="font-size: 9.5pt;font-family: Consolas;">  <span style="color: #008080;">dbo</span><span style="color: #808080;">.</span><span style="color: #008080;">ttAB\_BDC\_MM02Compare1</span><span style="color: #808080;">INNER</span><span style="color: #808080;">JOIN</span><span style="color: #008080;">dgSAP</span><span style="color: #808080;">.</span><span style="color: #008080;">dbo</span><span style="color: #808080;">.</span><span style="color: #008080;">MARA</span><span style="color: #0000ff;">ON</span><span style="color: #008080;">dbo</span><span style="color: #808080;">.</span><span style="color: #008080;">ttAB\_BDC\_MM02Compare1</span><span style="color: #808080;">.</span><span style="color: #008080;">\[RMMG1-MATNR\]</span><span style="color: #808080;">=</span><span style="color: #008080;">dgSAP</span><span style="color: #808080;">.</span><span style="color: #008080;">dbo</span><span style="color: #808080;">.</span><span style="color: #008080;">MARA</span><span style="color: #808080;">.</span><span style="color: #008080;">MATNR</span></span>

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">WHERE</span><span style="font-size: 9.5pt;font-family: Consolas;"><span style="color: #008080;">dbo</span><span style="color: #808080;">.</span><span style="color: #008080;">ttAB\_BDC\_MM02Compare1</span><span style="color: #808080;">.</span><span style="color: #008080;">RequestID</span><span style="color: #808080;">=</span><span style="color: #008080;">@RequestID</span></span>

 

<span style="font-size: 9.5pt;font-family: Consolas;color: #0000ff;">END</span>
