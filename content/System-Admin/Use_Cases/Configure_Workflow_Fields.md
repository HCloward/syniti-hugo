# Configure Workflow Fields

The workflow fields determine what is displayed in the subject line,
body text, and other fields of the workflow. These fields must be added
to the view and aliased correctly to be utilized in the workflow.

To configure the workflow fields:

1.  Select **WebApps** in the *Navigation* pane.

2.  Click the **Pages** icon for a WEB APP NAME.

3.  Click the **Events** icon for a **DESCRIPTION**.

4.  Click the **Business Rules** icon for an **EVENT**.

5.  Click **Vertical View** for a business rule with a PROCEDURE TYPE of
    Workflow.

6.  Click **Workflow Fields**.

7.  Click **Edit**.
    
    *[View the field description for the Advanced Workflow
    page.](../Page_Desc/Advanced_Workflow.htm)*

8.  Select a field from the **From** list box.
    
    **NOTE:** Displays the column name from the Alternate View that
    contains the sender’s email address.

9.  Select a field from the **To** list box.
    
    **NOTE:** Displays the column name from the Alternate View that
    contains the email address(es) or userID(s) of the TO recipients.

10. Select a field from the **CC** list box.
    
    **NOTE:** Displays the column name from the Alternate View that
    contains the email address(es) or userID(s) of the CC recipients. If
    the workflow contains a link, each recipient receives a separate
    notification or email.

11. Select a field from the **BCC** list box.
    
    **NOTE:** Displays the column name from the Alternate View that
    contains the email address(es) or userID(s) of the BCC recipients.
    If the workflow contains a link, each recipient receives a separate
    notification or email. 

12. Select a field from the **Subject** list box.
    
    **NOTE:** Displays the column name from the Alternate View that
    contains the subject of the email.

13. Select a field from the **Body** list box.
    
    **NOTE:** Displays the column name from the Alternate View that
    contains the content of the email. If **Support Workflow
    Authentication** is enabled (on the
    *[Parameters](../Page_Desc/Parameters_All_TabsSysAdmin.htm)*page),
    disclaimer text (to inform the email recipient that any user who
    clicks the workflow link is automatically authenticated based on the
    email recipient’s user account) appears above the **Body** text.

14. Select a field from the **Email Attachment** list box.
    
    **NOTE:** Displays the column name from the Alternate View where the
    paths to the file attachment(s) are specified.

15. Click **Save**.
    
    **NOTE:** When a workflow is executed, the WorkflowedBy and
    WorkflowedOn fields are updated in the page table, if the table
    exists.
