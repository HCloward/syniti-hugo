# Create a Basic Template

A template defines how data is posted into SAP, including which screens
and fields will be processed and whether the process contains a single
loop or multiple loops. Depending on the template type, additional
configuration options are available, such as setting conditionals for
BDC Screens or GUI Script Data, and defining structures for User Defined
templates.

Templates are not tied to data, but rather act as an independent guide
for posting that can be assigned to many processes.

There are seven template types in Integrate.  The initial steps to
create a template are the same no matter the template type.

A template can also be created based on a copy of an existing template.
Refer to [*Copy a Template*](Copy_a_Template.htm) for more information.

Once the template has been created and saved on the *Horizontal* View of
the *Template* page, the *Vertical* View displays. Configuration options
display on the *Vertical* View based on the template type.

Once a template has been created and configured, it must then be
activated and added to a process.

To create a template:

1.  Select **Categories** from *Navigation pane*.

2.  Click **Templates** for a category.
    
    **NOTE**: The number on the **Templates** icon displays the total of
    active and inactive category templates. 

3.  Click **Add** on Page toolbar.
    
    [View the field descriptions for the Template
    page.](../Page_Desc/Template_H.htm)

4.  Enter a name in **TEMPLATE NAME** field.
    
    **NOTE**: The Template Name must be unique. The template name can
    contain A-Z, 0-9, and underscore. No special characters are allowed
    in template names and Integrate will replace them with underscores
    when the template is saved.

5.  Enter a template description in **DESCRIPTION** field.

6.  Select a connection from the **CONNECTION ID** list box.
    
    **NOTE:** The Connection ID defines which system is used to gather
    metadata for the template. Refer to *[Establish a Connection to a
    Target
    System](../../Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)*
    for detailed information.

7.  Select a template type from **TYPE** list box.
    
    **NOTE**: The Type defines the type of SAP interaction that the
    template will process. 

8.  Click **Save**; the *Vertical* View displays.

9.  To continue with configuring a template, refer to the section
    corresponding to the template type.
    
    The template types are:
    
      - <span style="font-weight: bold;">BAPI/RFC</span> Refer to
        [Configure an RFC Template](Configure_a_RFC_Template.htm) and
        [Configure a BAPI Template](Configure_a_BAPI_Template.htm) for
        more
        information.
      - <span style="font-weight: bold;">BDC</span><span style="font-weight: bold;">Script</span>
        Refer to [Record a BDC Script](Record_a_BDC_Script.htm) for more
        information.
      - <span style="font-weight: bold;">Custom</span>: Refer to [Post
        Data Using a Custom
        Template](Post_Data_Using_a_Custom_Template.htm) for more
        information.
      - <span style="font-weight: bold;">GUI</span><span style="font-weight: bold;">Script</span>
        Refer to [Record a GUI Script](Record_a_GUI_Script.htm) for more
        information.
      - **IG Universal Connect** Refer to [Post Data Using IG Universal
        Connect](../../IGUC/Post%20Data%20Using%20IG%20Universal%20Connect%20Overview.htm)
        for more information.
      - <span style="font-weight: bold;">SAP Data Services Job</span>
        Refer to [Post Data Using an SAP Data Services
        Job](Post_Data_Using_an_SAP_Data_Services_Job_Overview.htm) for
        more information.
      - <span style="font-weight: bold;">User Defined</span> Refer to
        [Configure an XML Template with Structures, Elements and
        Attributes](ConfigureXMTemplateStrctrEleAtt.htm) and [Create and
        Transfer Files for User Defined Fixed Width or Delimited
        Templates](CreatTransferFilesUrDTemplates.htm) for more
        information.
