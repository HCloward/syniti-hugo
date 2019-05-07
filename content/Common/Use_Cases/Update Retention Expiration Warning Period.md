+++
title = ''
solution = 'Platform'
+++

# Update Retention Expiration Warning Period

If an object is assigned a data classification that requires a retention
period warning, the DSP sends a workflow email warning the Data
Controller assigned to that object that data is to be purged from a
target, target source, or table.

The email lists all objects to be purged, and contains a link to the
object in the Collect. By default, the email is sent daily for the 7
days prior to the retention expiration date.

A Common Administrator can update the number of days prior to the
retention expiration date that the DSP sends the warning email to Data
Controllers.

After receiving the email, a Data Controller can choose to update the
retention expiration date. An e-signature is required for this update.

**NOTE:** The Collect Administrator must check the **WORK FLOW SUMMARY**
check box for the target and Data Controller on the *[Workflow Summary
User
Settings](../../Collect/Page_Desc/Workflow_Summary_User_Settings.htm)*
page. The Data Controller is added to this page automatically. If the
check box is not checked, the Data Controller will not receive a warning
email that data is going to be purged.

Refer to [Update the Retention Expiration
Date](../../Collect/Use_Cases/Support_Regulatory_Compliance.htm#Update_the_Retention_Expiration_Date)
for more information.

To update the retention warning expiration period in Common:

1.  Select **Configuration \> Modules \> Parameters – Collect** in the
    *Navigation* pane.

2.  Click the **Workflow Settings** tab.

3.  Click **Edit**.
    
    [View the field descriptions for the Parameters – Collect
    page](../Page_Desc/Parameters_Collect.htm)

4.  Enter the number of days before data is purged (the retention
    expiration date) that a warning workflow email is sent to the Data
    Controller in the **Retention Expiration Date Notification** text
    box.

5.  Click **Save**.
