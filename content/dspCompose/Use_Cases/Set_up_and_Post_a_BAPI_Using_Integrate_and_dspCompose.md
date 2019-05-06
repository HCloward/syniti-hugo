# Set up and Post a BAPI using Integrate and dspCompose™

Using Integrate and dspCompose™, an advanced user can set up a BAPI
template and post requests. This feature is for users such as BackOffice
consultants with knowledge of SQL and development in the DSP®.

To set up and post a BAPI using Integrate and dspCompose™:

1.  Create a BAPI Template and Process in Integrate. Refer to [Post Data
    Using A
    BAPI](../../../Platform/Integrate/Use_Cases/Post_Data_Using_a_BAPI.htm)
    for more information.
2.  [Create all tt Tables and Views for the BAPI
    Process](Create_tt_Tables_and_Views_for_the_BAP_Process.htm)
3.  [Create rt tables From the tt
    tables](Create_tt_Tables_and_Views_for_the_BAP_Process.htm)
4.  [Create Custom Pages and
    Views](Create_Custom_Pages_and_Views_for_the_BAPI_Process.htm)
5.  [Use the custom pages in
    dspCompose™](Use_the_Custom_Pages_in_dspCompose_for_the_BAPI_Process.htm)

**NOTE**: These generic instructions for using an Integrate BAPI with a
dspCompose™ template create one data entry page that includes all the
fields to be populated from all the loops. <span>Stored procedures may
be registered on the *Template (Role Event)* page for the Review role
and used to populate individual tables for each loop in the BAPI
process.</span>  Depending on the user’s actual process, the pages that
need to be created and the procedures used to populate page tables may
vary from this example.
