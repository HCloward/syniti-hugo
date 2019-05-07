+++
title = 'Set Tables to Store Posting Feedback'
solution = 'Data Quality'
+++

# Set Tables to Store Posting Feedback

After a request has been posted, dspCompose™ creates a post message and
a post fail indicator for each posted record. To customize posting
feedback for dspCompose™-generated and custom data entry pages, a
Template Administrator can set, at the template level, the tables that
dspCompose™ should update with this data.

If a dspCompose™ template is associated with a multi-template Integrate
process, the Post Message Table settings must be updated. The Template
Administrator must assign an Integrate Template ID to each Post Error
Column and Post Message Column combination.  If this Integrate Template
ID is not assigned, the user cannot know which template in the
multi-template process failed.

For example, a user in Integrate creates four Integrate templates, one
for each update to a single attribute in material master basic data.
These templates are combined into one Integrate process (called a
multi-template process).

A Template Administrator then creates a template in dspCompose™ that
captures all the data to provide to the four Integrate templates on a
single record.

On the <span style="font-style: italic;">[Template (Post Message
Tables)](../Page_Desc/Template_Post_Message_Tables.htm)</span> page in
dspCompose™, a user must associate the post message table for each Post
Error Column and Post Message Column combination with its respective
Integrate Template ID.

Refer to [Post Request Data to the Target ERP
System](Post_Request_Data_to_a_Target_ERP_System.htm) for more
information.

**NOTE:** To set tables for posting feedback, the template must not be
active or must be in Developer Mode. Refer to [Modify an Active Template
in Developer Mode](Modify_an_Active_Template_in_Developer_Mode.htm) for
more information.

<span style="font-weight: bold;">NOTE:</span> A Post Message table must
be defined on the <span style="font-style: italic;">Template (Post
Message Table) page</span> (Team \> Templates \> Vertical View \>
Configuration \> Post Message Tables). This page must have a record for
the Data Entry table that contains the column where the returned Post
Message is stored. If the Post Message table is not defined, an error
displays when a user clicks Post on the
<span style="font-style: italic;">Request (Roles)</span> page and the
posting process stops.

To set the tables to store posting feedback:

1.  Click **Team** in the *Navigation* pane.

2.  Click **Templates** for a team.

3.  Click **Vertical View** for a template.

4.  Click **Configuration** tab.

5.  Click **Post Message Tables**.

6.  Click **Add**.
    
    *[View the field descriptions for the Template (Post Message Tables)
    page.](../Page_Desc/Template_Post_Message_Tables.htm)*

7.  Select a data source from the **DATA SOURCE** list box.
    
    **NOTE:** The DATA SOURCE contains the table to be updated with the
    posting message and post error indicator.

8.  Select a table name from the **TABLE NAME** list box.
    
    **NOTE:** The TABLE NAME is the table to be updated with the posting
    message and post error indicator.

9.  Select a column from the **POSTING PRIMARY KEY COLUMN** list box.
    
    **NOTE:** The POSTING PRIMARY KEY COLUMN is the column on the table
    that contains the values marked as the Primary Key column in
    Integrate for the Integrate Process registration.

10. Select a column from the **POST ERROR COLUMN** list box.
    
    **NOTE:** The POST ERROR COLUMN is the column on the table to which
    the post error indicator should be written.

11. Select a column from the **POST MESSAGE COLUMN** list box.
    
    **NOTE:** The POST MESSAGE COLUMN is the column on the table to
    which the post messages should be written.

12. Select a template ID from the
    <span style="font-weight: bold;">INTEGRATE TEMPLATE ID</span> list
    box, if needed.
    
    **NOTE:** This option must be selected for each Post Error Column
    and Post Message Column combination if the dspCompose™ template is
    associated with an Integrate mutli-template process.

13. Click **Save**.
