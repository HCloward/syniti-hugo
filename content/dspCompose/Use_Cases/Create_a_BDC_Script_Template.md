+++
title = 'Create a BDC Script'
solution = 'Data Quality'
+++

# Create a BDC Script

A user can record a BDC script in dspCompose™ to create a template. When
using this method, only those fields that are required for recording the
template display.

The process for recording a template in dspCompose™ is the same as the
recording process in Integrate. Refer to [Record a BDC
Script](../../../Platform/Integrate/Use_Cases/Record_a_BDC_Script.htm)
in Integrate for detailed information about recording a BDC template.

When a dspCompose™ template is created, an Integrate process is
automatically created in the Integrate category set for dspCompose™.
This category, called **dspCompose**, is automatically added to
Integrate during the BackOffice Solutions installation.

To create a template in dspCompose:

1.  Click **Team** in the *Navigation* pane.

2.  Click the **Create Template** icon for a team.

3.  Click **Create from BDC Recording**.
    
    **NOTE:** If no records exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    [View the field descriptions for the Create Template (Recording)
    page](Create_Template_Recording.htm)

4.  Enter a name in the **TEMPLATE NAME** field.
    
    **NOTE:** The name must be unique and can contain A-Z, 0-9, and
    underscore. No special characters are allowed in template names. If
    a special character is entered in a template name, dspCompose™
    replaces it with an underscore when the template is saved.

5.  Enter an SAP transaction code in the **TRANSACTION CODE** field.

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

8.  Click the **Record** icon to launch the local SAP environment.
    
    **NOTE:** For BDC recordings, SAP opens in *learning mode* using the
    defined transaction code, which utilizes the same recording
    mechanism as the SHDB transaction code in SAP to track the modified
    fields touched by a user during the recording.

9.  Record the transaction.
    
    **NOTE:** Refer to [Record a BDC
    Script](../../../Platform/Integrate/Use_Cases/Record_a_BDC_Script.htm)
    in Integrate for detailed information about recording a BDC
    template. Refer to [BDC Script and GUI Script Recording
    Tips](../../../Platform/Integrate/Use_Cases/BDCScriptGUIScriptRecTips.htm)
    in Integrate for recording tips.
    
    **NOTE:** If a mistake was made during the recording, click
    **Record** again for the template to start a new recording, which
    copies over the existing BDC recording.

10. Once the recording is complete, the *Create Template (Recording)*
    page displays.

11. Click **Create Template**; a confirmation message displays.

12. Click **Ok**.

Refer to [Configure Templates](Configure_Templates.htm) for more
information.
