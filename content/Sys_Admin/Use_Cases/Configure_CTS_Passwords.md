+++
title = 'Configure CTS Passwords'
solution = 'Platform'
+++

# Configure CTS Passwords

The CTS password is a security measure that ensures objects are moved to
the correct instance. To move objects between instances, the CTS
password must be the same on both instances.

<span style="font-weight: bold;">NOTE:</span> The password can be
anything, as long as it is identical on both the source and the target
instance. The password cannot be blank.

To configure CTS passwords:

1.  Log in to the DSP®  source instance.

2.  Select **Admin \> Configuration \> Parameters** in the *Navigation*
    pane.

3.  Click the **Security Settings** tab.

4.  Click **Edit**.
    
    [View the field descriptions for the Parameters
    page](../Page_Desc/Parameters_All_TabsSysAdmin)

5.  Enter a password in the **CTS Password** field.

6.  Click **Save**.

7.  Repeat all steps for the target instance, making sure to enter the
    same password on both instances.
