+++
title = 'Set Posting Options at the Category Level'
solution = 'Master Data Management'
+++

# Set Posting Options at the Category Level

By default, an Integrate process that posts dspConduct™ requests uses
the posting method Standard SAP Posting.

A user can update the posting method and set posting options for the
Integrate process used to post requests at the Category level. These
options are then used by default for all scenarios in the category added
after the posting options are updated.

These options can be overridden at the scenario level and viewed, but
not updated, at the request level. Refer to [Update Posting Options at
the Scenario Level](Update_Posting_Options_at_the_Scenario_%20Level.htm)
for more information.

Refer to [BDC Post Methods and Settings on the Advanced
tab](../../../Platform/Integrate/Page_Desc/BDCPostMethodsSettingsAdvTab.htm)
for more information about posting methods.

To set posting options in dspConduct™:

1.  Click **Design** in the *Navigation* pane.

2.  Click **Vertical View** for a category.

3.  Click the **Posting Processes** icon.

4.  Click the **Vertical View** icon for an integrate process.

5.  Click **Edit**.
    
    *[View the field descriptions for the Category Process page’s
    Vertical View.](../Page_Desc/Category_Process.htm#Category)*

6.  Update options as needed.
    
    **NOTE:** Refer to the field descriptions above for more
    information.

7.  Click **Save**.

Any scenarios created in the category will have these posting options by
default. The posting options for scenarios that already exist in the
category are not updated.
