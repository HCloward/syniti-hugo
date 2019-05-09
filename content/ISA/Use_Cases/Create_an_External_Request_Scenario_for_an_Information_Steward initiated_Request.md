# Create an External Request Scenario for an Information Steward-initiated Request

<span style="font-weight: bold;">NOTE:</span> Information Steward (IS)
is SAP’s software for data profiling and metadata management. The
Information Steward Accelerator by Back Office Associates® (ISA)
extracts data that failed IS rules, then distributes the data to groups
of users via reports.

An external request scenario can be configured to remediate failed data
on ISA reports using dspCompose™. Refer to [Create a Request in
dspCompose™ From the ISA Report Data Viewer
Page](Create_a_Request_in_dspCompose_From_ISA) for more information.

**NOTE:** An external request scenario cannot be created for an active
template.

**NOTE:** For the template that uses the ISA external request scenario
that creates a request from an ISA report, there can only be one Role
defined with the lowest Priority.

**NOTE:** For the template that uses the ISA external request scenario
that creates a request from an ISA report, there cannot be an External
Data role defined.

To create an external request scenario in dspCompose™ for an Information
Steward-initiated request:

1.  Click **Team** in the *Navigation* pane.

2.  Click the **Templates** icon for a team.

3.  Click the **ISA External Request Scenarios** icon for a template.
    
    **NOTE:** This icon does not display if the ISA is not installed and
    licensed.
    
    **NOTE:** If the template is not active and no scenarios have been
    created for this template, the page displays in add mode. Otherwise,
    click **Add**.
    
    **NOTE:** The Add button does not display if the template is active.
    
    [ View the field descriptions for the Template (ISA External Request
    Scenario)
    page](../Page_Desc/Template_ISA_External_Request_Scenario_H)

4.  Enter a rule name (for exmaple, NoRegion) in the **RULE ID** field.

5.  Enter the name of the ISA rule the scenario applies to (for example,
    Customers – Region) in the **RULE BINDING ID** field.

6.  Enter a description, if other than the default, in the **REQUEST
    DESCRIPTION FORMAT** field.
    
    **NOTE:** The text entered in this field displays on the *Request*
    page in the DESCRIPTION field for a request created from this
    external request scenario. The field defaults to **Request from ISA
    - \#Date\#**; the actual Date value will be substituted in the
    DESCRIPTION field when the request is created.
    
    **NOTE:** A value preceded and followed by \# is a dynamic
    substitution value for replacement at run time  A user can add these
    variables to the description:
    
     \#ISAProjectID\# - ISAProjectID (ISA Project ID)
    
     \#ISARuleBindingID\# - ISARuleBindingID (ISA Rule Binding ID)
    
    \#ISARuleID\# - ISARuleID (ISA Rule ID)
    
    \#RuleID\# - ExternalRequestAlias (Rule ID)
    
    \#RuleBindingID\# - Scenario (Rule Binding ID)
    
    \#RequestConnectionID\# - RequestConnectionID (RequestConnectionID)

7.  Click **Save**; the *Vertical* View displays.

8.  Select the name of the project that contains the rule from the **ISA
    Project ID** list box.
    
    **NOTE:** All projects that exist in the ISA display.

9.  Select the rule binding from the **ISA Rule Binding ID** list box.
    
    **NOTE:** Only rule bindings associated with the project in the ISA
    Project ID list box display.

10. Select a data source, if other than the default data source, where
    the staging table will be created in the **Staging Data Source ID**
    list box.
    
    **NOTE:** The Staging Data Source ID is populated with a default
    data source, but the value may be changed. This staging data source
    must be registered in the platform.

11. Enter the table name, if other than the default, for the staging
    table in the **Staging Table Name** field.
    
    **NOTE:** The staging table name is created automatically using the
    naming convention st\[Template Name\] \[Scenario\]\_ISAStaging. This
    table name can be changed.
    
    **NOTE:** Data is moved from the ISA report to this staging table
    where custom rules can then be run against the data before the data
    is moved to the Data Entry table of a request.

12. Click **Save**.
    
    **NOTE:** Once the record is saved, the ISA Rule ID field displays
    the ISA Rule Binding Description. Refer to [Edit Rule Binding
    Descriptions](Edit_Rule_Bindings) for more information.

13. Click the **Connections** icon to select a connection to the target
    system for each process template used in the scenario.
    
    **NOTE:** The connection is used to post the data during the posting
    role. dspCompose™ can post to multiple instances of the target
    system.
    
    **NOTE:** The Process Templates for which a connection can be set
    are based on:
    
      - The Integrate template type. Refer to [Create a Basic
        Template](../../../Platform/Integrate/Use_Cases/Create_a_Basic_Template)
        in Integrate for more information.
      - The "Allowed Connections" configured at the Integrate Process
        Template level. Refer to [Set Available Connections at the
        Process Template
        Level](../../../Platform/Integrate/Use_Cases/Set_Connections_at_the_Process_Template_Level)
        in integrate for more information.

14. Click **Edit**.

15. Select the connection from the **CONNECTION ID** list box.
    
    **NOTE:** If a user adds a request based on this template and does
    not select a connection ID, the default connection assigned to the
    Integrate Template is used for the request. Refer to [Establish a
    Connection to a Target
    System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview)
    for more information.

16. Click **Save**.

17. Return to the *[Template (External Request
    Scenario)](../../dspCompose/Page_Desc/Template_External_Request_Scenario)*
    page’s *Vertical* View.

18. Click the **Build Staging Area** icon.
    
    **NOTE:** If this template has not been generated, this icon is
    disabled.
    
    **NOTE:** A report for the chosen ISA Rule Binding ID must have been
    run in ISA before that staging table can be built.

19. Click **OK**.

**NOTE:** dspCompose™ creates a staging table in the Staging Data Source
database. The column names in the table match the column names listed on
the *Report Data Viewer* page for the associated ISA report.

**NOTE:** In some cases, the staging table may need to be rebuilt. Clear
the staging table by clicking **Clear Staging Area,** then click **Build
Staging Area**.

Refer to [Map Columns from the Template to Columns from the ISA
Report](Map_Columns_from_the_Template_to_Columns_from_the_ISA_Report)
to continue configuring the external request scenario.
