+++
title = 'Configure the Migration Dashboard'
solution = 'Platform'
+++

# Configure the Migration Dashboard

After the Agent Interface has been [installed and
configured](../Config/Set_up_and_Configuration_for_a_BackOffice_IGC_Connector_Agent%20Interface.htm),
configure the Migration dashboard in the DSP®.

Configure a wave within the DSP to send data to the Dashboard after the
initial structure of the Wave (Wave, Process Areas and Objects) has been
defined and the first steps of Target Design have begun. The first
metrics displayed on the Dashboard are that of Design Complete, thus
there is no requirement to configure the Wave to send metrics data to
the Dashboard until after Target Design has started.

To configure the Migration dashboard:

1.  Enter the **Start Date** and **End Date** for the active wave on the
    *Vertical* View of the
    *[Waves](../../../Migration/Console/Page_Desc/Waves_H.htm)* page in
    Console.
    
    **NOTE:** To view Quality metrics, the wave must have opportunity
    and error reports created and registered against one or more of the
    targets assigned to the objects in the wave.

2.  Select **Agent Interface \> Dashboards \> Migration Dashboard** in
    the *Navigation* pane.
    
    **NOTE:** All active waves across all contexts display on the *[Wave
    Identification](../Page_Desc/Wave_Identification_H.htm)* page.

3.  Click the **SEND WAVE AND MILESTONE METRICS** check box to include
    the wave in the Migration dashboard.
    
    **NOTE:** Two milestones are added by default for the start date and
    end date when this check box is checked. The thresholds for the
    start date are set to 0% for all values. The thresholds for the end
    date are set at 100% for all values, except the data quality
    thresholds, which are set to 6 and 7 sigma thresholds.

4.  Click the **Milestones** icon for the wave.

5.  Either:
    
      - Click **Add** to add a milestone or
    
      - Select the **START** or **END** milestone and click **Edit**.
        
        [View the field descriptions for the Wave Milestones
        page](../Page_Desc/Wave_Milestones_H.htm)

6.  Enter a name for the milestone in the **NAME** field.
    
    **NOTE:** This name cannot be the same name as another milestone in
    the wave.

7.  Enter a four-character version of the name in the **ABBREVIATION**
    field.
    
    **NOTE:** This abbreviation displays on the Migration dashboard, and
    cannot be the same abbreviation as an abbreviation for another
    milestone in the wave.

8.  Click the **MILESTONE DATE** date picker and select a date by which
    the milestone must be completed.
    
    **NOTE:** If the user adds a milestone, the date must be after the
    wave’s start date and before the wave’s end date.
    
    **NOTE:** The date cannot be the same date as another milestone date
    in the wave.
    
    **NOTE**: A milestone added for the current date does not display on
    the Migration dashboard.
    
    **NOTE:** The REQUIRED check box is selected by default for the
    Start Date and End Date milestones. These milestones cannot be
    deleted. The REQUIRED check box cannot be checked for any other
    milestones.

9.  Enter the percentage complete for the milestone in the **DESIGN
    COMPLETE UPPER THRESHOLD** field.

10. Enter the percentage complete for the milestone in the **DESIGN
    COMPLETE LOWER THRESHOLD** field.
    
    **NOTE:** Design Complete indicates how much of the design work has
    been completed. This percentage is calculated as the total number of
    active fields within active targets where design is complete (the
    design status is Design Complete or Finished) divided by the total
    number of active fields within active targets, regardless of design
    status. This percentage calculation is compared to the threshold in
    relation to the milestone date. If the percentage calculation is
    equal to or greater than the upper threshold percentage, this
    milestone is complete and the detail row for the Design Complete
    metric displays green on the dashboard. If the percentage
    calculation is between the upper and lower thresholds, the detail
    row for the metric displays light blue. If the percentage
    calculation is less than or equal to the lower threshold, the detail
    row for the metric displays red.

11. Enter the percentage complete for the milestone in the **MAPPING
    COMPLETE UPPER THRESHOLD** field.

12. Enter the percentage complete for the milestone in the **MAPPING
    COMPLETE LOWER THRESHOLD** field.
    
    **NOTE:** Mapping Complete indicates how much of the field mapping
    and value mapping work has been completed. This percentage is
    calculated as the total number of total mappings opportunities for
    both value and field mapping divided by the total number of mappings
    in Complete status. This percentage calculation is compared to the
    threshold in relation to the milestone date. If the percentage
    calculation is equal to or greater than the upper threshold
    percentage, this milestone is complete and the detail row for the
    Mapping Complete metric displays green on the dashboard. If the
    percentage calculation is between the upper and lower thresholds,
    the detail row for the metric displays light blue. If the percentage
    calculation is less than or equal to the lower threshold, the detail
    row for the metric displays red.

13. Enter the percentage complete for the milestone in the **RULES
    COMPLETE UPPER THRESHOLD** field.

14. Enter the percentage complete for the milestone in the **RULES
    COMPLETE LOWER THRESHOLD** field.
    
    **NOTE:** Rules Complete indicates how many of the rules have been
    completed. This percentage is calculated by the total number of
    source and target rules for the active fields with a rule status of
    Complete divided by the total number of source and target rules
    (also called rule opportunities). This percentage calculation is
    compared to the threshold in relation to the milestone date. If the
    percentage calculation is equal to or greater than the upper
    threshold percentage, this milestone is complete and the detail row
    for the Rules Complete metric displays green on the dashboard. If
    the percentage calculation is between the upper and lower
    thresholds, the detail row for the metric displays light blue. If
    the percentage calculation is less than or equal to the lower
    threshold, the detail row for the metric displays red.

15. Enter the percentage complete for the milestone in the **QUALITY
    UPPER THRESHOLD** field.

16. Enter the percentage complete for the milestone in the **QUALITY
    LOWER THRESHOLD** field.
    
    **NOTE:** Quality indicates the data quality of the wave. This
    percentage is calculated using the totals on the error reports
    registered to the wave and targets (post load reports) divided by
    the total number of records on the opportunity reports registered to
    the waves and targets (preload reports). Reports are registered on
    the [Data Quality Report
    Assignment](../Page_Desc/Data_Quality_Report_Assignment.htm) page.
    This percentage calculation is compared to the threshold in relation
    to the milestone date. If the percentage calculation is equal to or
    greater than the upper threshold percentage, this milestone is
    complete and the detail row for the Quality metric displays green on
    the dashboard. If the percentage calculation is between the upper
    and lower thresholds, the detail row for the metric displays light
    blue. If the percentage calculation is less than or equal to the
    lower threshold, the detail row for the metric displays red.

17. Click **Save**.

18. On the *[Wave
    Identification](../Page_Desc/Wave_Identification_H.htm)* page, click
    **the Data Quality Report Assignment** icon for the wave to select
    the error and opportunity reports to use in the Quality metrics
    calculation.

19. Select the wave-process area-object-target and click the **Edit**
    icon for the row.
    
    [View the field descriptions for the Data Quality Report Assignment
    page](../Page_Desc/Data_Quality_Report_Assignment.htm)

20. Select the report from the **DATA QUALITY OPPORTUNITY REPORT** list
    box.
    
    **NOTE:** This preload report lists the number of records for the
    combination to be used in the Quality metrics calculation.
    
    **NOTE:** All active and inactive reports, whether they are assigned
    to the target or not, display in this list.
    
    **NOTE:** For reports to display in this list box, they must follow
    the proper naming conventions:
    
      - tv\[InformalTableName\]\_\[FieldName\]\_\[Description\]Sel or
      - tv\[InformalTableName\]\_\[FieldName\]Sel or
      - tv\[InformalTableName\]\_\[Description\]Sel
    
    Refer to [Naming
    Conventions](../../../Migration/Transform/Use_Cases/Naming_Conventions.htm)
    and [Naming Conventions and the Enforce Strict Naming
    Feature](../../WebApp_Dev/Naming_Conventions_and_the_Enforce_Strict_Naming_Feature.htm)
    for more information.

21. Select the report from the **DATA QUALITY ERROR REPORT** list box.
    
    **NOTE:** This postload report lists the number of error records for
    the combination to be used in the Quality metrics calculation.
    
    **NOTE:** All active and inactive reports, whether they are assigned
    to the target or not, display in this list.
    
    **NOTE:** For reports to display in this list box, they must follow
    the proper naming conventions:
    
      - tv\[InformalTableName\]\_\[FieldName\]\_\[Description\]Sel or
      - tv\[InformalTableName\]\_\[FieldName\]Sel or
      - tv\[InformalTableName\]\_\[Description\]Sel
    
    Refer to [Naming
    Conventions](../../../Migration/Transform/Use_Cases/Naming_Conventions.htm)
    and [Naming Conventions and the Enforce Strict Naming
    Feature](../../WebApp_Dev/Naming_Conventions_and_the_Enforce_Strict_Naming_Feature.htm)
    for more information.

22. Click **Save**.

When configuration is complete, the wave, milestone and threshold data
is sent to the IGC Migration dashboard via a series of Service pages. By
default, the pages that send data related to adding and updating a wave
and adding and updating metrics send the data hourly. Service pages
relating to purging logs and metrics data runs once a day. The dashboard
metrics are updated hourly.
