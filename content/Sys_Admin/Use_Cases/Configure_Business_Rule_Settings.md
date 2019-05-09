+++
title = 'Configure Business Rule Settings'
solution = 'Platform'
+++

# Configure Business Rule Settings

A Page Designer can configure settings that allow business rules
registered to the OnValidate page event to run or not run during the
Bulk Execution process. Business rules can run conditionally based on
the validation results. Refer to [Business
Rules](../../WebApp_Dev/Business_Rules) for more information.

A Page Designer can also prevent users from updating the Exclude
Business Rules check box on the Bulk Execution panel, preventing them
from allowing business rules to run.

To configure business rule settings:

1.  Select **WebApps** in the *Navigation* pane.

2.  Click the **Pages** icon for a **WEB APP NAME.**

3.  Click the **Events** icon for a **DESCRIPTION**.

4.  Click **Vertical View**.

5.  Click the **Bulk Execution** tab.

6.  Update the **Exclude Business Rule Default** check box, as needed.
    
    **NOTE:** If the **Exclude Business Rule Default** check box is
    checked, the **Exclude Business Rules** check box on the Bulk
    Execution panel is checked by default. Any business rules registered
    to the OnValidate event are not run during the Bulk Execution
    process. If the **Exclude Business Rule Default** check box is
    unchecked, business rules registered to the OnValidate event run by
    default during the Bulk Execution process, and the **Exclude
    Business Rules** check box on the Bulk Execution panel is unchecked
    by default.

7.  Update the **Exclude Business Rule Option** check box as needed.
    
    **NOTE:** If the **Exclude Business Rule Option** is checked, the
    user cannot uncheck the **Exclude Business Rules** check box on the
    Bulk Execution panel, and business rules registered to the OnVaidate
    page event do not run. If the **Exclude Business Rule Option** is
    unchecked, a user can update the **Exclude Business Rules** check
    box on the Bulk Execution panel.

8.  Click **Save**.
