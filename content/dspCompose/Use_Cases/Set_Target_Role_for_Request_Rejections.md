# Set Target Role for Request Rejections

A *target role* is the role that will receive rejected request data. It
could be the Data role or a custom role.

The Template Administrator can set a target role for a request when a
Review role rejects all or part of a request’s records. The rejected
request records are then assigned to the target role.

The target role is set at the template role level, and can be configured
only for the Review role. This option can be set while configuring the
template or while the template is in Developer Mode.

In the workflow, if a Review role rejects all records in a request, the
request is assigned to the target role. If dspCompose™ has been
configured to allow partial approvals for a request, when the Review
role rejects some records in a request, dspCompose™ creates a new
request and assigns it to the target role.

Refer to [Perform a Partial
Approval](Review_Request_Data.htm#Perform_a_Partial_Approval) for more
information.

**NOTE**: To set a target role at the template level, the template must
not be active or must be in Developer Mode. Refer to [Modify an Active
Template in Developer
Mode](Modify_an_Active_Template_in_Developer_Mode.htm) for more
information.

To set a target role for request rejections:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Vertical View** for the Review role.

5.  Click the **Approve and Finish Settings** tab.

6.  Click **Edit**.
    
    *[View the field descriptions for the Template (Role) page’s
    Vertical
    View.](../Page_Desc/Template_Role_H.htm#Template_Role_V_All_Tabs)*

7.  Select a role from the **Reject Role Target** list box.
    
    **NOTE**: When a Review role rejects all records in a request based
    on this template, the request is assigned to this role. If the field
    is blank, dspCompose™ assigns the request to the lowest priority
    role in the request.

8.  Select a role from the **Partial Approval Reject Request Role
    Target** list box.
    
    **NOTE**: If dspCompose™ has been configured to allow partial
    approvals of requests, and a Review role rejects some of the records
    in a request, dspCompose™ creates a new request for the rejected
    records and assigns it to the role selected in the **Partial
    Approval Reject Request Role Target** list box. If the field is
    blank, dspCompose™ assigns the request to the lowest priority role
    in the request.

9.  Click **Save**.
