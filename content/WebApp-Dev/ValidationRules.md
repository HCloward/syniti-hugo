+++
title = 'Validation Rules'
solution = 'Platform'
+++

# Validation Rules

Validation rules manage correct data entry. If the validation occurs
upon save and fails, a message is displayed. Validation rules are based
on views in SQL that are registered to the page in DSP.

During the design or modification of a WebApp, validations can be
incorporated into a page or can be added to a field based on an event.

This section contains the following topics:

  - Validation Rule Guidelines
  - Register a Validation Rule to a Page
  - Enable Inherit Validations

## <span id="Validati"></span>Validation Rule Guidelines

  - Use the naming convention webXXX\_YYYYVal where XXX is the primary
    table or page and YYYY describes what the validation rule is
    validating, for example, webOrderDetail\_QtyGreaterThanOnHandVal.
  - DSP automatically generates a validation rule view for columns under
    the following conditions:
      - When a column property is created with the Required value set to
        Required (soft).
        
        **NOTE:**Refer to [Assign Column
        Properties](Assign_Column_Properties.htm) for more information.
    
      - When a column property is established for a list box or filtered
        text box with the List Allow Insert option set to Constrained to
        table. Refer to [Enable List Allow
        Insert](Enable_List_Allow_Insert.htm) for more information.
    
      - When image or button column properties are added to a column and
        not linked to a page.
  - Validations only run on the page for which they are created. They
    are not connected or linked to additional pages. Inherit Validation
    enables validations to run for up to 30 linked pages. Refer to
    Enable Inherit Validations for more information.
  - Validation rules are assigned a Severity on the *[Page Validation
    Rules](../Sys_Admin/Page_Desc/Page_Validation_Rules.htm)* page
    (WebApps \> Pages \> Events \> Validation Rules) to dictate
    boastatus behavior. Severity types are:
      - **Error** – Marks the status as invalid until the error is
        corrected and the Validation rule passes.
      - **Message** – The status is valid but a message is displayed.
      - **Warning** – Displays a message and the status can be validated
        or invalidated by the user.

<!-- end list -->

  - Ensure the table has a boaStatus column. Reserved columns can be
    automatically added to tables using the Append Column feature. Refer
    to [Append BOA Reserved Columns to
    Tables](Append_BOA_Reserved_Columns_to_Tables.htm) for more
    information.
  - If the validation rule is only relevant under certain data
    conditions provide a “Conditional Column” in the view to allow for a
    0 (disabled) or 1 (enabled) value to determine whether the
    Validation rule executes. This can be useful when, for example,
    ensuring a field has a non-NULL value when another column is
    enabled.

## <span id="Register"></span>Register a Validation Rule to a Page

Refer to Validation Rule Guidelines for general information.

To register the Validation rule to a page in DSP:

1.  Select **Admin \> WebApps** in the *Navigation* pane.

2.  Click the **Pages** icon for a WebApp and click **Events**.
    
    OR

<!-- end list -->

1.  Access the page in the WebApp.

2.  Click the **Change Settings** icon on Site toolbar.

3.  Click **Design**.

4.  Click **Events** for the page.
    
    **NOTE:** An OnValidate event must be added for every page that
    contains a boaStatus field, even if there are no validation rules or
    business rules registered to the page. If the OnValidate event is
    not created, boaStatus is not automatically updated by DSP. If an
    OnValidate event has already been added, skip to step 8.

5.  Select **OnValidate** from the **Event** list box.

6.  Click **Save**, the *Vertical* View displays.
    
    **NOTE:** If populated, the Pre Message displays before the
    validation rule runs and the Post Message displays after the
    validation rule runs. Use the messages with consideration to the end
    user.

7.  Click **Save**.

8.  Return to the *Horizontal* View.

9.  Click the **Validation Rules** icon.

10. Enter a number in the **PRIORITY** field.
    
    **NOTE:** The PRIORITY is the order in which the validation rule
    runs.

11. Select an option from the **VALIDATION TYPE** list box.
    
    **NOTE:** Options are:
    
      - **External Page** - This setting executes a plugin to determine
        whether the associated record is valid. The validation fails if
        a non-zero result is returned.
      - **Stored Procedure** – This setting executes a procedure to
        determine whether the associated record is valid. The validation
        fails if a non-zero result is returned.
      - **View** – This setting binds the view against the current
        column key to determine validity. If the view returns any
        results, the Validation rule is considered failed.

12. Select an option from the **SEVERITY** list box.
    
    **NOTE:** Options are:
    
      - **Error** - If the record fails this validation, the status is
        marked as invalid and the Business rule does not run.
        
        **NOTE:** A business rule can be configured to run even when a
        validation fails. Check the Run on Validate Fail check box on
        the *[Page Business
        Rules](../Sys_Admin/Page_Desc/Page_Business_Rules_H.htm)* page’s
        *Vertical* View to configure this setting.
    
      - **Message** – This severity is an informative validation rule
        which works the same as other validation types but does not
        negatively affect the validity of the record itself (for
        example, failing a message does not fail the record validation).
    
      - **Warning** - If the record fails this type of validation, the
        user clicks Yes or No on the warning message to either pass or
        fail the record. If passed, all business rules set to “Run On
        Validate” on the *Page Business Rules* *Vertical* View run. If
        not, only the rules set to “Run On Validate Fail” run and the
        record is marked accordingly.
    
      - **Workflow Only** – Deprecated.

13. Click **Save**; the *Vertical* View displays.

14. Select the view that stores the validation rule from the **View**
    list box.

15. Enter text in the **Comment** field.
    
    **NOTE:** The text in the Comment field displays to the end user
    when the validation rule fails.

16. Click **Save**.

## <span id="Enable"></span>Enable Inherit Validations

Pages in a WebApp are not organized in a hierarchy; however, the Inherit
Validation feature uses controls linking to other pages to establish a
hierarchy.

For example, if Inherit Validation is enabled on the link between the
Orders and OrderDetail pages, the OnValidate event of the Orders page
also runs the validations from the OnValidate event on the OrderDetail
page, just as if the validation rules were registered on the OrderDetail
page.

To enable Inherit Validations between a parent and a child page:

1.  Select **Admin \> WebApps** in the *Navigation* pane.

2.  Click the **Pages** icon for a WebApp and click **Events**.
    
    OR

<!-- end list -->

1.  Access the parent page in the WebApp.

2.  Click the **Change Settings** icon on the Site toolbar.

3.  Click **Design**.

4.  Click the **Column Properties** icon for the page.

5.  Click the link in the **LINK TO PAGE** column that provides the
    navigation to the child page; the *[Page Column
    Links](../Sys_Admin/Page_Desc/Page%20Column%20Links.htm)* page
    displays.
    
    **NOTE:** The column property is not applied to the linking column
    on the parent page but rather the link property on the child page.

6.  Click the **Advanced Properties** tab.

7.  Click the **Inherit Validations** check box.
