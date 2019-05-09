+++
title = 'Set Bulk Execution Parameters'
solution = 'Platform'
+++

# Set Bulk Execution Parameters

The Bulk Execution parameters allow the Page Designer to set processing
and record limit thresholds to control the load on the server.

To set Bulk Execution parameters:

1.  Select **Admin \> Configuration \> Parameters** in the *Navigation*
    pane.

2.  Select the **Page Parameters** tab.

3.  Click **Edit**.
    
    [View the field descriptions for the Parameters
    page](../Page_Desc/Parameters_All_TabsSysAdmin.htm)

4.  Enter the value for the **Bulk Execution Limit** field.
    
    **NOTE:** This value represents the number of records which a user
    can bulk execute against on any page. If this value is exceeded, a
    message displays to indicate the result set needs to be filtered to
    reduce the number of records visible before a Bulk Execution can be
    performed. This is meant to reduce the load on the server.

5.  Enter the value for the **Bulk Execution thread Limit** field.
    
    **NOTE:** Displays the number of concurrent threads that can process
    Bulk Execution logic. Each invocation of Bulk Execution uses half of
    the remaining threads with a minimum of 1. This is to reduce the
    load on the server when running under load and while remaining
    highly responsive while not under heavy usage.
    
    **NOTE:** Serialized events always run in 1 thread.

6.  Click **Save**.
