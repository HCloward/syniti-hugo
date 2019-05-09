+++
title = 'Set Plan Security'
solution = 'Platform'
+++

# Set Plan Security

User security can also be set at the plan level to assign a user
read-only access to a plan, or to restrict access for a user assigned to
the Sample Project Level Role and Sample Plan Level Role.

A user must have [security set for dspTrack™ in System
Administration](Set_dspTrack_Security_in_System_Administration)
before plan security can be set.

**NOTE:** By default, users assigned to the Business User security role
have read-only access to Plan pages and cannot import a project or copy
a plan. Similarly, any user who has been assigned read-only access
cannot copy a plan or import a project.

<span style="font-weight: bold;">NOTE:</span> If a user is assigned to
the Business User security role only, that user will not display on the
<span style="font-style: italic;">Plan Access Setup</span> page, because
Business Roles users primarily interact with the Work List.

To assign a user read-only access to a Plan or to restrict access for a
user assigned to the Sample Project Level Role and Sample Plan Level
Role:

1.  Select **Project** in *Navigation* pane.

2.  Click **Plans** for a project.

3.  Click **Vertical View** for a plan.

4.  Click the **Security** tab.

5.  Click **Setup**.
    
    **NOTE**: All users with access to the selected plan display.

6.  Click the <span>**READ ONLY** check box</span> for a user to assign
    read-only access to all pages in the plan.
    
    <span style="font-weight: bold;">NOTE:</span> The logged in user
    cannot set read only access for his or her own account and the READ
    ONLY check box is not available for the logged in user’s account. If
    a user has read only access, that user cannot update any page in the
    plan, including the *Plan Access Setup* page. Therefore, if the
    logged in user could set read only access for his or her own
    account, the logged in user could never change access for his or her
    own account back to Write Access. For example, user BFranklin is
    logged in and has access to the Software Implementation plan as a
    member of the Sample Plan Level Role. BFranklin can change
    permissions to read only for any user on the Plan Access Setup page,
    and restrict that user’s access to all pages in the Software
    Implementation plan to read only. However, BFranklin cannot change
    his own access to read only. It is set to Write Access by default.

7.  Click to enable the <span style="font-weight: bold;">Ignore During
    Sync Process</span> check box, if necessary.

<span style="font-weight: bold;">NOTE:</span> If enabled, the READ ONLY
setting for the user ID is ignored when the automatic synchronization
procedure runs. The user's read only access is not updated during this
procedure, which syncs the settings on the
<span style="font-style: italic;">Plan Access Setup</span> page with the
Security Role settings for dspTrack™. Refer to [Use Template Security
Roles](Use_Template_Security_Roles) for more information.
