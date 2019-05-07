+++
title = 'Work with Metric Groups'
solution = 'Migration'
+++

# Work with Metric Groups

Metric groups are a subcategory of field groups and provide a way to
further organize data for metrics tracking and mapping. The metric
groups are defined in Target Design and set for Target Fields in Target
Design. Metric groups are displayed on the
<span style="font-style: italic;">[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)</span> page in Map
and several reports showing progress of the mapping process.

Each set of metric groups are delineated into logical sets of fields
that relate to a screen within the Target system. For SAP-related
objects, the metric groups can represent the tabs within an SAP screen
or TCode (for example, Customer Basic, Sales, Company and Accounting).

Metric groups are like field groups in that they have a default metric
group (\*) that all fields are assigned to by default. The default
metric group (\*) cannot be deleted or updated.

**NOTE**: Metric groups cannot be assigned to fields when they are
cloned for field groups. They can only be assigned to fields that are
assigned to the default field group (\*). For example, three field
groups have been added in Target Design (FERT, HALB, and ROH). The field
PSTAT is assigned to all three field groups and the default field group
(\*). A metric group can be added to the PSTAT field assigned to the
default (\*) field group, but cannot be assigned to the PSTAT field
assigned to the FERT, HALB or ROH field groups.

To work with metric groups in Target Design:

  - [Add a Metric Group](#Add_a_metric_group)
  - [Assign a Metric Group to a Target Field](#Assign_a_metric_group)

## <span id="Add_a_metric_group"></span>Add a Metric Group

**NOTE**: The default metric group (\*) is assigned to all fields.

To add a metric group in Target Design:

1.  Select **Configuration \> Metric Groups** in the *Navigation* pane.

2.  Click **Add**.
    
    *[View the field descriptions for the Metric Groups
    page](../Page_Desc/Metric_Groups.htm)*

3.  Enter a name for the group in the **METRIC GROUP** field.
    
    **NOTE**: This name will appear as an option in the Metric Group ID
    list box on the *Vertical* View of the *[Target
    Fields](../Page_Desc/Target_Fields_H_Target_Design.htm)* page.

4.  Enter a value in the **PRIORITY** field.
    
    **NOTE:** This value indicates the order that fields should be
    mapped in Map on the *[Field
    Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)* page. A metric
    group with a priority of 1 should be mapped first. Key and required
    fields should be mapped before optional fields.

5.  Enter a comment about the group in the **COMMENT** field.
    
    **NOTE**: This field may contain a longer descriptive name for the
    metric group.

6.  Click
**Save**.

## <span id="Assign_a_metric_group"></span>Assign a Metric Group to a Target Field

**NOTE**: A metric group can only be assigned to a Target field if the
Target is in a design status of In Design.

**NOTE**: Metric groups cannot be assigned to fields when they are
cloned for field groups. They can only be assigned to fields that are
assigned to the default mapping group (\*). For example, three field
groups have been added in Target Design (FERT, HALB, and ROH). The field
PSTAT is assigned to all three field groups and the default field group
(\*). A metric group can be added to the PSTAT field assigned to the
default (\*) field group, but cannot be assigned to the PSTAT field
assigned to the FERT, HALB or ROH field groups.

To assign a metric group to a field in Target Design:

1.  Select **Design** in the Context bar.

2.  Click the **Targets**icon on the *[Design](../Page_Desc/Design.htm)*
    page.

3.  Click the <span style="font-weight: bold;">Fields</span> icon for a
    Target.

4.  Click the **Vertical View** icon for the field that should belong to
    the metric group.

5.  Click **Edit**.
    
    *[View the field descriptions for the Target Fields page’s Vertical
    View](../Page_Desc/Target_Fields_H_Target_Design.htm)*

6.  Either:
    
    Select an option in the **Metric Group ID** combo box.
    
    OR
    
    Click the **+** sign to add a metric group. Refer to Add a Metric
    Group for more information.

7.  Click **Save**.

**NOTE**: Once the metric group is assigned to a Target field, it
displays on the *[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)* page in Map.
