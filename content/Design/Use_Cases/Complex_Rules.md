+++
title = 'Complex Rules'
solution = 'Migration'
+++

# Complex Rules

Complex rules are managed in Target Design. They are not edited or
submitted in Map. These mappings have a message on the record stating
that the rule was created in Target Design. The mapping for a field with
a Complex rule displays in Map with an Action of Manual Rule.  Users can
add a description of a Complex rule with documentation and comments.
Complex rules provide information that the Data Services developer uses
when writing the rule. When an AutoGen request is processed, a
placeholder where Complex rules can be developed is created.

Refer to [Data Services
AutoGen](../../Data_Services_AutoGen/Data_Services_Automation.htm) for
more information.

This section contains the following topics:

  - [Add a Complex Rule](#Add_a_Complex_Rule)
  - [Sync Complex Rules with Map](#Sync_Complex_Rules_with_Map)
  - [Assign the Rule to a Field and Execution
    Stage](#Assign_the_Rule_to_a_Field)
  - [Add an Execution Stage](#Add_an_Execution_Stage)
  - [View Rules Assigned to an Execution
    Stage](#View_Rules_Assigned_to_an_Exec)

<span style="font-weight: bold;">NOTE:</span> If a field has both a
Complex and Basic rule, the mapping also displays in Map with an Action
of Manual Rule on the <span style="font-style: italic;">[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)</span> page.

<span style="font-weight: bold;">NOTE:</span> After a Target with a
Target field that has a Basic rule or Complex rule assigned is synced
with Map, these rules are automatically sent to the
<span style="font-style: italic;">[Mapping
Approval](../../Map/Page_Desc/Mapping_Approval_H.htm)</span> page for a
developer to review them; however, they do not require approval to be
used by Data Services AutoGen.

<span style="font-weight: bold;">NOTE:</span> If a Target’s Source
mappings and Target mappings ({Target Rules}) are complete, and a
Complex rule is added to a Target or field, Source mappings are not
overwritten when the Target is synced to Map. Target mappings (as in,
{Target Rules}) are overwritten when the Target is synced.

## <span id="Add_a_Complex_Rule"></span>Add a Complex Rule

<span style="font-weight: bold;">NOTE:</span> Complex rules cannot be
added to zLegacy fields.

**NOTE:** Complex rules can only be added to a Target field if the
Target has a Design Status of In Design.

To add a Complex rule in Target Design:

1.  Select **Target Rules \> Complex Rules** in the *Navigation* pane.
    
    <span style="font-weight: bold;">NOTE:</span> If no Complex rules
    have been added, the page displays in add mode. Otherwise, click
    **Add**.
    
    *[View the field descriptions for the Rules: Complex Rule
    page](../Page_Desc/Rules_Complex_Rule_H.htm)*

2.  Enter a unique name for the rule in the **NAME** field.
    
    <span style="font-weight: bold;">NOTE:</span> The default name New
    Complex Rule cannot be used.

3.  Enter a description of the rule in the **DESCRIPTION** field.

4.  Update the <span style="font-weight: bold;">ACTIVE</span> check box
    as needed.
    
    <span style="font-weight: bold;">NOTE:</span> If a Complex rule is
    active, it can be assigned to a Target field.

5.  Click **Save**; the *Vertical* View displays.

6.  Select a type from the **Rule Type** list box.
    
    <span style="font-weight: bold;">NOTE:</span> This value, and the
    information in the fields listed below, is for documentation
    purposes only.

7.  Enter code, pseudo code or a rule definition in the **Rule Syntax**
    field.

8.  Enter supplemental information or instructions in the **Comment**
    field.

9.  Click **Save**.
    
    <span style="font-weight: bold;">NOTE:</span> Once saved, the
    documented rule can be assigned to Target fields. Refer to [Assign
    the Complex Rule to a Target Field and Execution
    Stage](#Assign_the_Rule_to_a_Field) for more information.

<span id="Sync_Complex_Rules_with_Map"></span>

## Sync Complex Rules with Map

Complex rules are documented and assigned to fields in Target Design and
can store a SQL function, BODS functions or stored procedure. Once the
fields' Target is synced to Map, the Target Rules for the fields display
on the
<span style="font-style: italic;">[<span style="font-style: italic;">Field
Mappings</span>](../../Map/Page_Desc/Field_Mappings_H.htm)</span> page.

For a field with a Complex rule that uses a BODS function, the settings
on the<span style="font-style: italic;"> Field Mappings</span> page in
Map are:

  - <span style="font-weight: bold;">Action</span>— Rule
  - <span style="font-weight: bold;">Rule Status</span>— Complete
  - <span style="font-weight: bold;">Mapping Status</span>— Complete
  - <span style="font-weight: bold;">Edit</span>,
    <span style="font-weight: bold;">Reset</span>, and
    <span style="font-weight: bold;">Submit</span> icons are disabled
  - <span style="font-weight: bold;">Rule Comment</span>— Indicates that
    the rule has been added in Target Design
  - <span style="font-weight: bold;">Comment</span>— Indicates that the
    rule has been added in Target Design
  - <span style="font-weight: bold;">Mapped On</span>— Displays the date
    that the Target was synced
  - <span style="font-weight: bold;">Mapped By</span>— Displays Target
    Design

If a Complex rule has a SQL function stored in Target Design, then the
settings on the <span style="font-style: italic;">Field Mappings</span>
page in Map are:

  - <span style="font-weight: bold;">Action</span>— Manual Rule
  - <span style="font-weight: bold;">Rule SQL:</span>— Not Populated
  - <span style="font-weight: bold;">Rule Status</span>— Complete
  - <span style="font-weight: bold;">Mapping Status</span>— Complete
  - <span style="font-weight: bold;">Edit</span>,
    <span style="font-weight: bold;">Reset</span>, and
    <span style="font-weight: bold;">Submit</span> icons are disabled
  - <span style="font-weight: bold;">Rule Comment</span>— Displays the
    description or the Target Rules as added in Target Design
  - <span style="font-weight: bold;">Comment</span>— Indicates the rule
    has been added in Target Design  

Refer to [Sync Map and Target Design](Sync_Map_and_Target_Design_TD.htm)
for more
information.

## <span id="Assign_the_Rule_to_a_Field"></span>Assign the Rule to a Field and Execution Stage

After a Complex rule has been created it can be assigned to a Target
field. When assigning a complex rule to a Target field, an execution
stage must also be assigned.

Execution stages allow rules to be grouped for different execution
levels. Individual Complex rules do not have a priority set in Target
Design.

**NOTE**: Complex rules can only be assigned to fields when the Target
Design Status is In Design.

To assign a Complex rule to a Target field in Target Design:

1.  Select **Design** in the Context bar.

2.  Click the **Targets**icon on the *[Design](../Page_Desc/Design.htm)*
    page.

3.  Click the **Fields** icon for a Target.

4.  Click the **Complex Rules** icon.

5.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.

6.  Select the name of the Complex rule in the **TARGET COMPLEX FIELD
    RULE ID** list box.

7.  Click the **+** icon to add a Complex rule if needed.

8.  Select the execution stage from the **TARGET RULE EXECUTION STAGE
    ID** list box.
    
    **NOTE**: Execution stages are added on the *[Rules: Execution
    Stage](../Page_Desc/Rules_Execution_Stage_Complex_Rule.htm)* page.
    Refer to [Add an Execution Stage](#Add_an_Execution_Stage) for more
    information.

9.  Click **Save**.
    
    **NOTE**: Deleting the registration of a Complex rule to a Target
    field does not delete the Complex rule itself. The rule is still
    available on the <span style="font-style: italic;">Rules: Complex
    Rule</span> page (Target Rules \> Complex Rules).

<span id="Add_an_Execution_Stage"></span>

## Add an Execution Stage

The Execution stage allows Complex rules to be grouped for different
execution levels during Data Services AutoGen. The Primary execution
stage is created by default during installation and cannot be updated.

Creating additional execution stages is optional.

To create an execution stage in Target Design:

1.  Select **Target Rules \> Execution Stages** in the *Navigation*
    pane.

2.  Click **Add**.
    
    *[View the field descriptions for the Rules: Execution Stage
    page](../Page_Desc/Rules_Execution_Stage_H.htm)*

3.  Enter a unique name for the stage in the **NAME** field.

4.  Enter a value in the **STAGE NUMBER** field.
    
    **NOTE:** This number sets the order that rules assigned to this
    stage are added to the enrichment data flow. 

5.  Enter a brief description of the stage in the **DESCRIPTION** field.

6.  Click
**Save**.

## <span id="View_Rules_Assigned_to_an_Exec"></span>View Rules Assigned to an Execution Stage

To view the rules assigned to each execution stage in Target Design:

1.  Select **Target Rules \> Execution Stages** in the *Navigation*
    pane.
2.  Click the **Complex Rules** icon for a NAME to view all of the
    Complex rules assigned to that stage.
