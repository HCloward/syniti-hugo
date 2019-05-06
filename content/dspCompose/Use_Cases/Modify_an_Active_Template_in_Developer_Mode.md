# Modify an Active Template in Developer Mode

**NOTE**: Developer Mode should only be used by developers while
troubleshooting issues when configuring a template. It should never be
used in a Production environment.

A Template Administrator can enable Developer Mode to make configuration
changes to an active template with active requests. Once the updates are
complete, Developer Mode can then be disabled to prevent further
updates.

**NOTE**: When changes are made in Developer mode, requests that were
previously entered for the template may no longer work.

<span style="font-weight: bold;">NOTE</span>: When Developer Mode is
enabled for an active template, different icons are active on the
General tab of the <span style="font-style: italic;">Templates</span>
page’s <span style="font-style: italic;">Vertical</span> View depending
on the template type. For custom templates, the Generate Custom icon
displays. For BDC script and GUI script templates, the Generate icon
displays.

To update an active template:

1.  Click **Vertical View** on the *Templates* page for the template.

2.  Click **Advanced** tab.

3.  Click **Developer Mode**.
    
    **NOTE**: While in Developer Mode, the template’s settings, assigned
    roles, and other options can be updated. On the *Template* page’s
    *Vertical* View, the **Edit** and **Delete** buttons become active.
    On the **Advanced** tab, the **Regenerate Data Objects** icon and
    the **Reset Status** icon are active.
    
    **NOTE**: A template cannot be deactivated in Developer Mode if
    there are active requests associated with the template.

4.  Click **Developer Mode** on the **Advanced** tab of the *Templates*
    page's Vertical View when updates are complete to turn Developer
    Mode off.
