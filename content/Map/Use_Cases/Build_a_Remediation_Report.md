+++
title = 'Build a Remediation Report'
solution = 'Migration'
+++

# Build a Remediation Report

During a mock load to test a data migration implementation, build a
remediation report using Target Design, Map and AutoGen that will be
processed in Transform.

Target Remediation allows a remediation rule to be registered to an
error report. Remediation rules are used only when there is a need to
temporarily fix a data issue so the affected records can be loaded into
a test environment.

Once Transform has processed Target data, it generates error reports.
Based on these reports, a user may create remediation rules to correct
erroneous values so that the data can be loaded successfully into the
Target system using a load tool.

Refer to [Register Target Remediation
Rules](../../Transform/Use_Cases/Register_Target_Remediation_Rules)
and [View Remediation Rule
Information](../../Transform/Use_Cases/View_Remediation_Rule_Information)
for more information.

**NOTE:** This process requires the user to move between Map, Target
Design, AutoGen and Transform. Use the Context bar at the top of the
page to move between the components.

The process for building a remediation report for a field that uses an
Xref or RuleXref action is different than the process for building a
remediation report for fields that use any other action.

To build a remediation report for field mappings with an Xref or Rule
Xref action:

1.  In Map, perform and complete an Xref or Rule Xref field mapping for
    a field with a check table (for example field BSTME on ttMARA with
    check table T006).
    
    <span style="font-weight: bold;">NOTE:</span> A mapping with an
    action of Xref or Rule Xref is required for Value Mapping. Refer to
    [Xref](Xref) and [RuleXref](Rule_Xref) for more information.
    
    <span style="font-weight: bold;">NOTE:</span> A lookup table must be
    assigned to the field in Target Design to build the report. Refer to
    [Set Up Lookup
    Tables](../../Design/Use_Cases/Set_up_a_Simple_Lookup_Table) for
    more information.
    
    <span style="font-weight: bold;">NOTE:</span> To build a remediation
    report, a Remediation value must be set in Map for check tables for
    the field. To set the value, access the
    <span style="font-style: italic;">Vertical</span> View of the
    <span style="font-style: italic;">[Field
    Mappings](../Page_Desc/Field_Mappings_H)</span> page for the
    field and enter the value in the Remediation Value field.
    
    **NOTE:** The field mapping must be approved on the Mapping Approval
    page.

2.  Select **Configuration \> Value Mapping (Config)** in the
    *Navigation* pane.

3.  Click the **Refresh** icon for the check table; a confirmation
    message displays.

4.  Click **OK**.
    
    **NOTE:** The REMEDIATION VALUE field displays the first value from
    the check table pulled in via the Refresh.
    
    **NOTE:** If the REMEDIATION VALUE needs to be updated, click Edit,
    select a new REMEDIATION VALUE from the drop down list and click
    Save.
    
    <span style="font-weight: bold;">NOTE:</span> This value is only
    used in Transform for Check table defaulting on MOCK loads. This
    value should not be used for Go-Lives.

5.  In AutoGen (select the gold Automation tab on the Quick Panel),
    select the Object that contains the Target for which the remediation
    rule is to be built.

6.  Click the **BUILD REPORTS WITH REMEDIATION** icon; a confirmation
    message displays.

7.  Click **OK**;a message displays that the Target reports with
    remediation has been built.

8.  Click **Transform** in the Context bar.

9.  Click the **Targets** icon.

10. Click the **Reports** icon for the Target with the check table.

11. Locate the Target field with the **REPORT TYPE** of Target
    Readiness.

12. Click **Execute**.

The Target report is processed and any records that need to be
remediated will be processed by the remediation rule.

A summary of the report displays in Transform on the
<span style="font-style: italic;">[Target Remediation
Overview](../../Transform/Page_Desc/Target_Remediation_Overview)</span>
page.

To build a remediation report for fields that are mapped using actions
other than Xref or RuleXref actions :

1.  Select **Design** from the Context bar.

2.  Click the <span style="font-weight: bold;">Targets</span> icon.

3.  Click **Edit** for an active field on the *[Target
    Fields](../../Design/Page_Desc/Target_Fields_H_Target_Design)*
    page that does not have a check table.
    
    *[View the field descriptions for the Target Fields
    page](../../Design/Page_Desc/Target_Fields_H_Target_Design)*

4.  Select an option from the **REQUIRED TYPE** list box. Values are:
    
      - <span class="listnumber" style="font-weight: bold;">Business
        Required</span> – This field is required to meet a business
        rule.
      - <span class="listnumber" style="font-weight: bold;">Technical
        Required</span> - This field is required so that processes may
        run, data can be saved, or for some other reason that allows the
        field to be mapped or used in
        migration.
      - <span class="listnumber" style="font-weight: bold;">Conditional</span>
        – This field is required under certain conditions related to
        Target
        rules.
      - <span class="listnumber" style="font-weight: bold;">Optional</span>
        – This field is not required.

5.  Click **Save**.

6.  In Map, click the **Mappings** icon for the Target.

7.  Click **Vertical View** for the {Target Rules} field mappings.

8.  Click **Edit**.
    
    *[View the field descriptions for the Field Mappings page's Vertical
    View](../Page_Desc/Field_Mappings_H)*

9.  Enter a value in the **Remediation Value** field.

10. Enter a value in the **Remediation Comment** field.

11. Click **Save**.

12. Click **Map** in the Context bar.

13. Click the **Targets** icon on *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map)* page.

14. Select a Target.

15. Click the **Build Reports with Remediation** icon on the Page
    toolbar; a confirmation message displays.

16. Click **OK**.

17. Click **Transform** in the Context bar.

18. Click the **Targets** icon.

19. Click the **Reports** icon for a Target.

20. Locate the Target field with the **REPORT TYPE** of Target
    Readiness.
    
    **NOTE:** The count on the TR icon displays 1.

21. Click **Execute**. The Target report is processed and any records
    that need to be remediated will be processed by the remediation
    rule.

A summary of the report displays in Transform on the *[Target
Remediation
Overview](../../Transform/Page_Desc/Target_Remediation_Overview)*
page.
