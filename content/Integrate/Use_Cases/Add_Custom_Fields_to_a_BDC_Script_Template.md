+++
title = 'Add Custom Fields to a BDC Script Template'
solution = 'Platform'
+++

# Add Custom Fields to a BDC Script Template

<span id="Post Data using a BDC Script Steps" class="popUpLink">\>Review
the steps in the process. </span>

Use custom fields when conditional screen execution is required and the
data for existing template fields is not adequate. For example, the
COMPANY\_CODE field is a template field (i.e., recorded in a BDC script)
that is going to be uploaded when the record posts to SAP. If a BDC
screen only displays when COMPANY\_CODE = 0001, a user can set a
condition on the COMPANY\_CODE field to only execute when the data
mapped to COMPANY\_CODE = 0001. However, if the COMPANY\_CODE field was
not recorded in the BDC script, but the condition was still true (i.e.,
the BDC screen only displays when COMPANY\_CODE = 0001), a user can
create a custom field called "COMPANY\_CODE" and set the condition on
this field even though the field will not be uploaded into SAP.

Custom fields can be added to a BDC Script template once it is recorded.

<span style="font-weight: bold;">NOTE</span>: If the template is
recorded again, custom fields are not retained.

<span style="font-weight: bold;">NOTE</span>: If a BDC Script template
with custom fields is copied, the custom fields are not copied to the
new template.

Custom fields can be added to a template that uses loops. Loops must
have been created before adding custom fields. The loop that contains
the custom field is identified when adding the field. Refer to
[Configure Process Template Loops for a BDC Script Template with Looping
Enabled](ConfigureProcTempLoopsBDCLoopEn.htm) for more information.

<span style="font-weight: bold;">NOTE</span>: Custom fields cannot be
added to active templates.

Once a field has been added, a conditional can be applied to the field.
Refer to [Configure a Conditional for a BDC
Screen](ConfigureConditionalBDCScrn.htm) for more information.

To add a custom field:

1.  Click <span style="font-weight: bold;">Categories</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Templates</span> for a
    category.

3.  Click <span style="font-weight: bold;">Vertical View</span> for a
    template with a <span style="font-weight: bold;">TYPE</span> of BDC
    Script.

4.  Click <span style="font-weight: bold;">Configuration</span> tab.

5.  Click <span style="font-weight: bold;">Custom Fields</span>.

6.  If no custom fields have been added for the template, the page
    displays in add mode. Otherwise, click
    <span style="font-weight: bold;">Add</span>.
    
    <span style="font-weight: bold;">NOTE</span>: Custom fields cannot
    be added to an active template.
    
    [View the field descriptions for the Custom Fields
    page.](../Page_Desc/Custom_Fields.htm)

7.  Enter the name of the custom field in the
    <span style="font-weight: bold;">NAME</span> field.

8.  Enter a description of the field in the
    <span style="font-weight: bold;">DESCRIPTION</span> field.

9.  Enter an example of the data that displays in the field in the
    <span style="font-weight: bold;">SAMPLE VALUE</span> field.
    
    <span style="font-weight: bold;">NOTE</span>: This data is for
    informational purposes only.

10. Select the name of the loop in the template from the
    <span style="font-weight: bold;">LOOP</span> list box.
    
    <span style="font-weight: bold;">NOTE</span>: No options display in
    this list box if the template does not have loops.

11. Click <span style="font-weight: bold;">Save</span>.
