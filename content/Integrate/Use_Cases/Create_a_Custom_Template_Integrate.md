+++
title = 'Create A Custom Template'
solution = 'Platform'
+++

# Create A Custom Template

A Custom template allows a user to create a mechanism for posting to any
system.

A user must create all of the associated files and code to support the
Custom template.

<span style="font-weight: bold;">NOTE</span>: The user must know the
assembly file name and the Type Full Name (NameSpace + Class Name) to
enter them while creating the template. The system does not validate
this information. Refer to [Create a Custom
Assembly](Create_a_Custom_Assembly.htm) for more information.

<span style="font-weight: bold;">NOTE</span>: A Custom template does not
have a connection type because the implementation is defined by the
custom code. An option cannot be selected in the CONNECTION TYPE list
box when creating a Custom template.

To create a template:

1.  Select <span style="font-weight: bold;">Categories</span> from
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Templates</span> for a
    category.

3.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Template
    page.](../Page_Desc/Template_H.htm)

4.  Enter a name in <span style="font-weight: bold;">TEMPLATE
    NAME</span> field.
    
    <span style="font-weight: bold;">NOTE</span>: The Template Name must
    be unique. The template name can contain A-Z, 0-9, and underscore.
    No special characters are allowed in template names. Integrate
    replaces special characters with underscores when the process is
    saved.

5.  Enter a template description in
    <span style="font-weight: bold;">DESCRIPTION</span> field.

6.  Select Custom from <span style="font-weight: bold;">TYPE</span> list
    box.
    
    <span style="font-weight: bold;">NOTE</span>: A connection ID cannot
    be selected for a Custom template.

7.  Click <span style="font-weight: bold;">Save</span>;
    <span style="font-style: italic;">Vertical</span> View displays.

8.  Enter the .dll name in the <span style="font-weight: bold;">Assembly
    File</span> field.
    
    <span style="font-weight: bold;">NOTE</span>: The Assembly file name
    includes the .dll extension.
    
    <span style="font-weight: bold;">NOTE</span>: The system does not
    validate the name.

9.  Enter the name in the <span style="font-weight: bold;">Type Full
    Name</span> field.
    
    <span style="font-weight: bold;">NOTE</span>: This name must be in
    the format NameSpace.Class Name.
    
    <span style="font-weight: bold;">NOTE</span>: The system does not
    validate the name.

10. Click <span style="font-weight: bold;">Save</span>.

Continue with [Activate the Custom
Template](Activate_the_Custom_Template.htm).
