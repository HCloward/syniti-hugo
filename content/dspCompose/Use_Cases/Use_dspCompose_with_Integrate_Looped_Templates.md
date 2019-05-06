# Use dspCompose™ with Integrate Looped Templates

dspCompose™ is designed to automate the creation and posting of mass
changes to a single looped Integrate template. Posting mass changes to
SAP that require looping requires steps to be taken outside of the
traditional dspCompose™ process flow. While the creation of dspCompose™
templates and requests to post looped Integrate templates is not a
certified component of dspCompose™ and is not supported, the
functionality can be incorporated using the following steps:

1.  Create a Looped Template and Process in Integrate. Refer to
    [Configure Process Template Loops for a BDC Script Template with
    Looping
    Enabled](../../../Platform/Integrate/Use_Cases/ConfigureProcTempLoopsBDCLoopEn.htm)
    or [Configure Process Template Loops for a GUI Script Template with
    Looping
    Enabled](../../../Platform/Integrate/Use_Cases/ConfigureProcTemplLoopsGUILoopgEn.htm)
    in Integrate for more information.
2.  [Create all tt tables and tx views for the Integrate
    Process](Create_All_tt_Tables_and_tx_Views_for_the_Integrate_Process.htm),
    either manually or by using the Auto Generate feature of Integrate
3.  [Create rt Tables from the tt
    Tables](Create_rt_Tables_from_the_tt_Tables.htm)
4.  [Create Custom Pages and Views](Create_Custom_Pages_and_Views.htm)
    in dspCompose™ to enter Template data
5.  [Create a Template that Uses the Custom Pages in
    dspCompose™](Use_the_Custom_Pages_in_dspCompose_for_the_BAPI_Process.htm)
6.  [Add Custom Roles for the Looped
    Template](Add_Custom_Roles_for_the_Looped_Template.htm)

**NOTE:** These generic instructions should provide the steps needed to
use a multi-loop Integrate template with dspCompose™. These instructions
are an example. Modifications might be needed, depending on the user’s
actual process.
