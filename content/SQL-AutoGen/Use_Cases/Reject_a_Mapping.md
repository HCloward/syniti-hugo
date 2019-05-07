+++
title = 'Reject a Mapping'
solution = 'Migration'
+++

# Reject a Mapping

A mapping can be rejected on the
<span style="font-style: italic;">[Automation SQL Field
Mappings](../Page_Desc/Automation_SQL_Field_Mappings_H.htm)</span> page.

A mapping can also be rejected using the [Mapping
Approval](../../Map/Page_Desc/Mapping_Approval_H.htm) page. Refer to
[Reject the
Mapping](../../Map/Use_Cases/Approve_or_Reject_Mappings.htm#Reject_the_Mapping)
for more information.

When a mapping is rejected, Mapping Status and Rule Status are updated.
Refer to [Mapping Status and Rule
Status](../../Map/Use_Cases/Mapping_Status_and_Rule_Status.htm) for more
information.

To reject the mapping in AutoGen:

1.  Click the **Automation** tab in the Quick Panel.

2.  Click the <span style="font-weight: bold;">Mappings</span> icon for
    the Target.

3.  Click <span style="font-weight: bold;">Edit</span> for a mapping.
    
    [View the field descriptions for
    the](../Page_Desc/Automation_SQL_Field_Mappings_H.htm) [Automation
    SQL Field
    Mappings](../Page_Desc/Automation_SQL_Field_Mappings_H.htm) page.

4.  Enter a comment in the <span style="font-weight: bold;">RULE
    COMMENT</span> field.
    
    **NOTE:** A comment must be entered for the mapping to be rejected.

5.  Click <span style="font-weight: bold;">Save</span>.

6.  Click the <span style="font-weight: bold;">Reject</span> icon in the
    Page toolbar; a confirmation message displays.

7.  Click <span style="font-weight: bold;">OK</span>.

<span style="font-weight: bold;">NOTE:</span> Back in Map, the Rule
Status for the mapping on the <span style="font-style: italic;">[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)</span> page is
changed to Revision Requested and the Mapping Status  is changed from
Complete to Design Required. The comment added by the Developer on the
<span style="font-style: italic;">[Automation SQL Field
Mappings](../Page_Desc/Automation_SQL_Field_Mappings_H.htm)</span> page
displays in Map on the <span style="font-style: italic;">Field
Mappings</span> page’s <span style="font-style: italic;">Vertical</span>
View.

<span style="font-weight: bold;">NOTE:</span> If the Field Mappings page
is open in Map when a mapping is rejected, refresh the
<span style="font-style: italic;">Field Mappings</span> page manually to
see the update.

<span style="font-weight: bold;">NOTE:</span> If the action for the
mapping is Manual, Rule or RuleXref, the Developer can update the SQL
code for the rule in the Rule SQL field.

<span style="font-weight: bold;">NOTE:</span> When the developer rejects
the mapping, the Mapped By and Mapped On fields in Map are set to NULL
and the Mapper is notified via a user notification. Refer to [Set Up
User Notifications](../../Map/Config/Setup_User_Notifications.htm) for
more information.
