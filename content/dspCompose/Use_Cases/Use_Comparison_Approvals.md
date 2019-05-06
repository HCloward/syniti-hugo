# Use Comparison Appovals

The *Comparison Approval* functionality allows the Review role user to
see the current SAP field value as well as the value the field will be
changed to as a result of the data entry process. The Review role can
then easily compare the current state and the future state of records
before any changes take place. The Review role has the ability to reject
any changes and keep the original values.

**NOTE:** Advanced users such as BackOffice consultants should configure
the comparison approval feature as it requires knowledge of both SQL and
SAP. Once configured, business end users assigned to the Review role can
use the feature.

To configure and use comparison approvals:

1.  Create the template. Comparison approvals can be used for requests
    based on BDC Scripts, GUI Scripts and custom templates.
2.  [Configure the Comparison Approval
    Setting](Configure_the_Comparison_Approval_Setting.htm)
3.  [Register the CompareIns Stored
    Procedure](Register_the_CompareIns_Stored_Procedure.htm)
4.  [Create a Request for Comparison
    Approval](Create_a_Request_for_Comparison_Approval.htm)
5.  [Use the Comparison Approval
    Page](Use_the_Comparison_Approval_Page.htm)

Once dspCompose™ is set to use Comparison Approvals, when a template is
generated, dspCompose™ creates a stored procedure used to control the
Comparison page in the cMass\_Data database. The naming convention for
the procedure is **web\[Template Name\]CompareIns**. To see the before
and after data entries, the CompareIns stored procedure must be
modified.

Refer to [Sample Stored Procedure For Comparison
Approval](Sample_Stored_Procedure_for_Comparison_Approval.htm) for an
example of a modified stored procedure.

The stored procedure is used to insert what is currently in SAP (the
dgSAP tables) to the Comparison staging table in cMass\_Data for the
request.

**NOTE:** Comparison approvals can be used on a template that also
allows partial approvals. Refer to [Perform a Partial
Approval](Review_Request_Data.htm#Perform_a_Partial_Approval) for more
information.
