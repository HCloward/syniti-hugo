+++
title = 'Create a GUI Script Template'
solution = 'Data Quality'
+++

# Create a GUI Script Template

A user can record a GUI script in dspCompose™ to create a template. When
using this method, only those fields that are required for recording the
template display.

The user must have the SAP Logon Pad installed to perform the GUI
recording, and must end the recording by clicking **Stop Recording** in
dspCompose™, not by saving data in SAP.

The process for recording a template in dspCompose™ is the same as the
recording process in Integrate. Refer to [Record a GUI
Script](../../../Platform/Integrate/Use_Cases/Record_a_GUI_Script.htm)
 in Int

egrate for detailed information about recording a GUI template.

When a dspCompose™ template is created, an Integrate process is
automatically created in the Integrate category set for dspCompose™.
This category, called **dspCompose**, is automatically added to
Integrate during installation.

To create a template based on a new GUI recording in dspCompose:

1.  Click **Team** in the *Navigation* pane.

2.  Click the **Create Template** icon for a team.

3.  Click **Create from GUI Recording**.
    
    **NOTE:** If no records exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    [View the field descriptions for the Create Template (Recording)
    page](Create_Template_Recording.htm)

4.  Enter a name in the **TEMPLATE NAME** field.
    
    **NOTE:** The name must be unique and can contain A-Z, 0-9, and
    underscore. No special characters are allowed in template names. If
    a special character is entered in a template name, dspCompose™
    replaces it with an underscore when the template is saved.

5.  Enter the SAP transaction code in the **TRANSACTION CODE** field.

6.  Select an option from the **CONNECTION ID** list box.
    
    **NOTE:** The SAP Connection selected from the Connection list box
    is used for recording the template. dspCompose™ can connect to
    multiple SAP instances, which allows for recordings to be done in a
    test instance and posting to be done in a QA or production instance.
    
    **NOTE:** If a user adds a request based on this template and does
    not select a connection ID, the default connection assigned to the
    Integrate Template is used for the request. Refer to [Establish a
    Connection to a Target
    System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
    for more information.

7.  Click **Save**.

8.  Click the **Record** icon.

9.  Record the transaction.
    
    **NOTE:** Refer to [Record a GUI
    Script](../../../Platform/Integrate/Use_Cases/Record_a_GUI_Script.htm)
    in Integrate for detailed information about recording a template.
    Refer to [BDC Script and GUI Script Recording
    Tips](../../../Platform/Integrate/Use_Cases/BDCScriptGUIScriptRecTips.htm)
    in Integrate for recording tips.

10. Once the recording is complete, return to dspCompose™ and click
    **Stop Recording**; the *Create Template (Recording)* page displays.

11. Click **Create Template**; a confirmation message displays.

12. Click **Ok**.

Refer to [Configure Templates](Configure_Templates.htm) for more
information.
