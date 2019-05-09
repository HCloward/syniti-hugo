+++
title = 'Context, the Context Bar, and Navigation in dspMigrate™ Advanced Data Migration (ADM)'
solution = 'Migration'
+++

# Context, the Context Bar, and Navigation in dspMigrate™ Advanced Data Migration (ADM)

Use Console to create a context, which is the combination of a Wave and
Process Area, then assign an object, target and source (or multiple
objects, targets and sources) to a context. A context creates a
consolidated structure across dspMigrate™, which is accessible while
working in any dspMigrate™ Advanced Data Migration (ADM) component.

Generally, a migration project uses the components of
dspMigrate™Advanced Data Migration (ADM) in this order:

1.  Console
2.  Design
3.  Map
4.  Construct
5.  Transform

As a user works with components in dspMigrate™, the context displays in
the Context bar. Selecting the context allows the user access to the
context’s assigned object, target and source.

The Context bar is also used to navigate throughout the components of
dspMigrate™. Click the component name in the Context bar and the
component opens. The user can then work in that component with the
object, target and source assigned to the context.

While working in a migration project, a user works in one and only one
context at a time. Since the Context bar displays the current context, a
user can always know which objects, targets and sources are being worked
on.

The Wave Process Areas that display on the *[Context
Select](../Console/Page_Desc/Context_Select)* page depend on the
logged in user’s security settings. All contexts display for a user if
the user is assigned to the Migration Developer security role. This role
grants access to all Waves, including new Waves as they are added to
Console. If a user belongs to a security role other than Migration
Developer, the keys for each new Wave, Process Area, target and source
must be added to the security role when the Wave, Process Area, and
object are are added in Console and when targets and sources are added
in Target Design. Once the keys are added, the associated context
displays on the Context Select page. Refer to [Set up Security for
dspMigrate™](Set_Up_Security_for_dspMigrate) for more information.

**NOTE**: A user must have access to the Wave, the Process Area, the
object, the target and the source to be able to view and select it.
Refer to [Set up Security for
dspMigrate™](Set_Up_Security_for_dspMigrate) for more information.

To switch to a new context in the Context bar:

1.  Click the context name in the Context bar.
2.  Click the link in the Wave Process Area column.

The Context bar updates, displaying the new context, and the object,
target and source assigned to that context can be used in the component.

**NOTE**: If the user navigates to a component outside of dspMigrate™,
the Context bar no longer displays.

**NOTE**: If a user is currently working in a context (for example, that
context displays on the user’s Context bar), neither the Wave nor
Process Area in the context can be deleted.
