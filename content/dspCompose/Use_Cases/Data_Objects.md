+++
title = 'Data Objects'
solution = 'Data Quality'
+++

# Data Objects

After a Template Administrator generates a template (by clicking
**Generate** on the *Templates* page’s *Vertical* View), the *Template
(Objects)* page lists the system-generated objects used by the template,
including pages, stored procedures, tables, views, Integrate templates
and Integrate processes. When a template is generated in dspCompose™
tables, views and a stored procedure are automatically created in the
cMass\_Data database. Each request is differentiated by the RequestID.

When a Template Administrator deletes a template, dspCompose™ deletes
all system-generated objects used by the template.

If the template uses Org Units, additional objects related to Org Units
are also generated. Refer to [Use Org Units](Use_Org_Units) for more
information.

This topic contains the following sections:

  - [Edit Data Objects](#Edit_Data_Objects)
  - [WebApp Pages Created](#WebApp_Pages_Created)
  - [Tables Created](#Tables_Created)
  - [Views Created](#Views_Created)
  - [Stored Procedure Created](#Stored_Procedure_Created)
  - [Regenerate Data Objects](#Regenerate_Data_Objects)

## <span id="Edit_Data_Objects"></span>Edit Data Objects

A Template Administrator can edit the objects, as well as enable the
Remove Template on Delete setting that will retain an object in the
database even if the template is deleted on the *Template (Objects)*
page.

**NOTE:**Two databases and WebApps are installed when dspCompose™ is
installed: the cMass and cMass\_Data databases, and the dspCompose and
dspCompose\_Data WebApps. WebApp dspCompose and its database cMass
contain all the settings and validations that come with the installation
and should not be modified. Make All customizations and create data
validations in the dspCompose\_Data WebApp and database to prevent
customizations from being overwritten during any upgrades.

**NOTE:** Data objects cannot be added, edited or deleted for an active
template. Refer to [Activate the Template](Activate_the_Template)
for detailed information for activating and deactivating templates.

To edit template objects after the template has been generated:

1.  Select **Team** on the *Navigation* pane.

2.  Click **Templates** for a team.

3.  Click **Vertical View** for a template.

4.  Click the **Configuration** tab.

5.  Click **Objects**.

6.  Click **REMOVE ON TEMPLATE DELETE** check box to deselect it if the
    object should be retained in the database even if the template is
    deleted.

7.  Click **Edit** to make changes to an object if needed.
    
    *[View the field descriptions for the Template (Objects)
    page.](../Page_Desc/Template_Objects)*

8.  Click **Save**.

The following objects are created when a template is generated or when
system objects are refreshed on the *Template (Objects)* page.

  - A template is created in Integrate for each template created in
    dspCompose™.
  - A process is created in the dspCompose™ Team in Integrate for each
    template created in dspCompose™ .

These objects are created in the dspCompose\_Data WebApp in the
platform.

## <span id="WebApp_Pages_Created"></span>WebApp Pages Created

  - **\[Template name\]** – A data entry page

  - **\[Template name\] – Archive** – The archive page for archive
    comparison

  - **\[Template name\] Approve** – A page to view the Comparison
    Approvals for the Review role

  - **\[Template name\] Archive Approve** – A page to compare the
    archives

## <span id="Tables_Created"></span>Tables Created

  - **rt\[template name\]** – An archive table

  - **rt\[template name\]Compare** – An archive comparison table

  - **tt\[template name\]** – A data entry table

  - **tt\[template name\]Compare** – A data entry comparison table

  - **tt\[template name\]Validation** – A table containing validation
    rule severities and messages

## <span id="Views_Created"></span>Views Created

  - **web\[template name\]ArchiveHor** – A view that displays all fields
    from the Archive Template table.

  - **web\[template name\]CompareArchiveHor** – A view that compares all
    of the fields from the Archive table against the Archive Compare
    table to note differences between the data.

  - **web\[template name\]CompareHor** – A view that compares all of the
    fields from the active tables to note differences between the data
    on the <span style="font-style: italic;">Comparison</span> page in
    dspCompose™.

  - **web\[template name\]Hor** – A view that displays all the fields
    from the active template table on the data entry page in
    dspCompose™.

  - **web\[template name\]RejectCountSel** – A view that displays a
    count of all Rejected records within the active template table by
    template ID.

  - **web\[template name\]ValidationErrorMessageCount Sel** – A view
    that displays a count of all Validation Error Messages within the
    active table by Template ID.

  - **web\[template name\]Dcv** – A Data Control view that manages the
    status of the <span style="font-style: italic;">Template Role</span>
    page based on row level controls.

  - **web\[template name\]Pcv** – A Page Control view that manages the
    status of the <span style="font-style: italic;">Template Role</span>
    page based on page level controls.

  - **tx\[template name\]Int** – A view used by the template to
    configure field mappings within Integrate.

## <span id="Stored_Procedure_Created"></span>Stored Procedure Created

  - **web\[template name\]CompareIns** – A shell procedure to be
    configured for the comparison of all fields from the Archive table
    against the ArchiveCompare table.

## <span id="Regenerate_Data_Objects"></span>Regenerate Data Objects

During the template creation process, a user clicks the **Generate**
button on the *Templates* page’s *Vertical* View to generate data
objects.

These system-generated objects can also be regenerated to recreate all
of the automatically generated objects in the cMass\_Data database
originally created by generating the template.

When dspCompose™ regenerates the objects, it deletes all data objects
for the template and generates the data objects again according to the
current template settings. It does not delete the Integrate process or
template.

**NOTE:** A template cannot be active to regenerate its data objects.
The Regenerate Data Objects icon does not display for active templates.

To regenerate data objects:

1.  Select **Team** on the *Navigation* pane.

2.  Click **Templates** for a team.

3.  Click **Vertical View** for a template.

4.  Click **Advanced** tab.

5.  Click **Regenerate Data Objects** button; a warning message
    displays.
    
    **NOTE:** The Template must be processed by selecting **Generate**
    on the **General** tab before the **Regenerate Data Objects** button
    will be available.

6.  Click **Yes**; a confirmation message displays.

7.  Click **Ok**.
