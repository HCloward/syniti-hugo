+++
title = 'Create a Template For Advanced Users'
solution = 'Data Quality'
+++

# Create a Template For Advanced Users

Creating a template from the *[Templates](../Page_Desc/Templates_H.htm)*
page provides access to configuration settings to customize the
template. The method can be used by advanced users familiar with
dspCompose™.

To create a template:

1.  Select **Team** on the *Navigation pane*.

2.  Click the **Templates** icon for a team.
    
    **NOTE:** To access a template, a user must be granted access to a
    template role, or a user must have created the template. The count
    on the **Templates** icon displays the number of templates the user
    can access (based on the template roles to which a user is
    assigned), not the total count of templates that have been created
    for the team. If the **Templates** icon displays a count of 0, the
    user does not have access to any templates for that team.

3.  Click **Add**; the *Vertical* View displays.
    
    *[View a field descriptions of the Templates page’s Vertical
    View.](../Page_Desc/Templates_H.htm#Templates_V_All_Tabs)*

4.  Enter a name in the **Template Name** field.
    
    **NOTE**: The name must be unique and can contain A-Z, 0-9, and
    underscore. No special characters are allowed in template names. If
    a special character is entered in a template name, dspCompose™ will
    replace it with an underscore when the template is saved.

5.  Enter an SAP transaction code in the **Transaction Code** field for
    posting types of BDC Script and GUI Script. Templates of type Custom
    Setup do not require an SAP transaction code.

6.  Select a posting type from the **Type** list box.
    
    Values are:
    
      - **BDC Script** - Indicates the template is based on the results
        of a Batch Data Communication (BDC) script recorded in
        dspCompose
      - **GUI Script** - Indicates the template is based on the results
        of a GUI script recorded using the SAP Logon pad
      - **Custom Setup** – Indicates the template is custom and is not
        created using a recording
    
    **NOTE:** The only valid recordable options are BDC Script and GUI
    Script. The other available type is Custom Setup, which does not
    allow recording.
    
    **NOTE:** If the user selects **Custom Setup** and clicks **Save**,
    the **Record** button no longer displays.

7.  Select a connection ID to the target system from the **Connection
    ID** list box.
    
    **NOTE:** The SAP Connection selected from the Connection list box
    is used for recording the template. dspCompose™ can connect to
    multiple SAP instances which allows for the recordings to be done in
    a test instance and posting can be done in a QA or production
    instance.
    
    **NOTE:** If a user adds a request based on this template and does
    not select a connection ID, the default connection assigned to the
    Integrate Template is used for the request. Refer to [Establish a
    Connection to a Target
    System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
    for more information.

8.  Click **Save**.

9.  If available, click the **Record** button to launch the local SAP
    environment.
    
    **NOTE:** Template recording is available for BDC Script and GUI
    Script types only.
    
    **NOTE:** For BDC recording, SAP opens in *learning mode* using the
    defined transaction code, which utilizes the same recording
    mechanism as the SHDB transaction code in SAP to track the modified
    fields touched by a user during the recording. For GUI recordings,
    dspCompose™ tracks each action the user takes in the SAP GUI.

10. Record the transaction.
    
    **NOTE**: Refer to [Record a BDC
    Script](../../../Platform/Integrate/Use_Cases/Record_a_BDC_Script.htm)
    or [Record a GUI
    Script](../../../Platform/Integrate/Use_Cases/Record_a_GUI_Script.htm)
    in Integrate for detailed information about recording a template.
    Refer to [BDC Script and GUI Script Recording
    Tips](../../../Platform/Integrate/Use_Cases/BDCScriptGUIScriptRecTips.htm)
    in Integrate for recording tips.
    
    **NOTE:** If a mistake was made during the recording, click the
    **Record** button again for the template to start a new recording,
    which copies over the existing BDC/GUI recording.
    
    **NOTE:** Once a template has been recorded it must be further
    configured and generated before it can be used in requests. Refer to
    [Configure Templates](Configure_Templates.htm) for more information.

11. For BDC Script or GUI Script Type templates, click **Generate** on
    the **General** tab; a confirmation message displays.

12. Click **Ok**.
    
    **NOTE:** The template recording is imported into Integrate.
    Integrate creates a process with an identical name to the template.
    Integrate than creates the data entry pages based on this template
    and automatically maps the fields. Refer to [Data
    Objects](Data_Objects.htm) for more information.

13. Click the **Configuration** tab to access a link to the newly
    created Integrate process (in the field **Integrate Process ID**).
    
    **NOTE:**Until the template is generated, the Integrate Process ID
    field is blank.

14. Click the **Activate** icon on the Page toolbar to allow the
    template to be used for requests.
    
    **NOTE:** Refer to [Activate the
    Template](Activate_the_Template.htm) for more information.

15. Configure the template as needed.
    
    **NOTE:** Refer to [Configure Templates](Configure_Templates.htm)
    for detailed information.
