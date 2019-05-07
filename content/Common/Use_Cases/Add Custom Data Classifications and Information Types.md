+++
title = ''
solution = 'Platform'
+++

# Add Custom Data Classifications and Information Types

A Common Administrator can configure custom data classifications and
information types used for data protection. The DSP includes information
types and data classifications by default that cannot be edited or
deleted.

A data classification allows a client to classify the data in an object,
such as Human Resources, Sales, Customer or Personal.

An information type, assigned to a data classification, dictates whether
a retention period is required for an object that is assigned this data
classification. In this case, a workflow is sent to the object’s Data
Controller with a warning that data is to be purged on the retention
period expiration date.

To add a custom information type:

1.  Select **Common \> Configuration \> Modules \> Collect \>
    Information Type** in the *Navigation* pane.

2.  Click **Add**.
    
    *[View the field descriptions for the Information Type
    page](../Page_Desc/Information%20Type.htm)*

3.  Enter a name in the **Information Type** field.
    
    **NOTE:** This name displays on the *[Data
    Classification](../Page_Desc/Data%20Classification.htm)* page.

4.  Enable the **RETENTION PERIOD WARNING** check box if needed.
    
    **NOTE:** If checked, a retention expiration date must be added to
    an object’s Data Protection settings if a data classification using
    this information type is used.

5.  Click **Save**.

To add a custom data classification:

1.  Select **Common \> Configuration \> Modules \> Collect \> Data
    Classification** in the *Navigation* pane.

2.  Enter a name to classify the data in an object in the **DATA
    CLASSIFICATION** field.

3.  Select a type in the **INFORMATION TYPE** list box.
    
    **NOTE:** The information type setting dictates whether objects
    using this data classification are Personal, requiring a retention
    expiration date, Restricted, Public or custom.

4.  Click **Save**.
