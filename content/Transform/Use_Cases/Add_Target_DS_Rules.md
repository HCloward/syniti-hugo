# Add Target Data Services Rules

A Target Data Services rule cleans and manipulates data before it is
loaded into the Target.

**NOTE:** Target Data Services rules are created using Data Services
AutoGen. Refer to [Build and Refresh Data Services
Jobs](../../Data_Services_AutoGen/Use_Cases/Build_and_Refresh_DS_Jobs.htm)
for more information.

**NOTE:** For the Data Services options and pages to be available, the
Data Service Repository must be registered in Common. The Data Services
check box must be enabled in Console for the Process Area: Object. Refer
to [Register a Data Source in
Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
and  [Create the Context by Adding a Wave and Creating
Elements](../../Console/Use_Cases/Add_a_Wave_and_Create_Elements.htm)
for more information.

To add a data services rule to a Target in Transform:

1.  Click **Targets** on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page in Transform.

2.  Click the **Data Services Rules** icon for a Target.
    
    **NOTE:** The *Target Data Services Rules* page displays in Add Mode
    if no Target rules have been added for the Target.

3.  Click **Add**.
    
    [View the field descriptions for the Target Data Services Rules
    page](../Page_Desc/Target_Data_Services_Rules_H.htm)

4.  Enter a sort value in the **PRIORITY** field.
    
    **NOTE:** If multiple rules are registered to the Target, the
    priority determines the order the rule is processed. In Data
    Services rules are grouped and run by priority.

5.  Select a value from the
    **<span id="Status" class="popUpLink">STATUS</span>** list box.

6.  Select a type from the **RULE TYPE** list box. Options are:
    
      - **Delete –** Delete only rules.
      - **Insert –** Insert only rules.
      - **Manual –** All rules.
      - **Move –** Move only rules.
      - **Update –** Update only rules.

7.  Enter a name for the rule in the **TARGET DATA SERVICES RULE**
    field.
    
    **NOTE:** This is the name of the job that was created using the
    Data Services AutoGen process. Refer to [Build and Refresh Data
    Services
    Jobs](../../Data_Services_AutoGen/Use_Cases/Build_and_Refresh_DS_Jobs.htm)
    for more information.

8.  Enter a brief Target rule description in the **DESCRIPTION** field.

9.  Click **Save**; the *Vertical* View displays.

10. Click the **Documentation** tab.
    
    *[View the field descriptions of the Target Data Services Rule
    page’s Vertical View Documentation
    tab](../Page_Desc/Target_Data_Services_Rules_H.htm)*

11. Enter text in the **Comment** field to document any notes about the
    Target Data Services Rule (optional).

12. Click **Save**.
