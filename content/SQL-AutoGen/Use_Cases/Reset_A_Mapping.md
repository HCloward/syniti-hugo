# Reset A Mapping

After a mapping has been submitted in Map, it can be reset in SQL
AutoGen.

**NOTE:** A mapping will also be automatically reset if it is rejected
on the *[Mapping Approval](../../Map/Page_Desc/Mapping_Approval_H.htm)*
page. A rejection is tracked differently than a reset, as the Rejected
On and Rejected By fields that display on the
<span style="font-style: italic;">[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)</span> page’s
Vertical View and the <span style="font-style: italic;">[Field Mapping
History](../../Map/Page_Desc/Field_Mapping_History.htm)</span> page
(both in Map), are populated when a mapping is rejected.

A user can reset a mapping at any time.

**NOTE:** The Reset Field Mapping parameter set in Console on the
*[Parameters](../../Console/Page_Desc/Parameters.htm)* page controls how
a mapping is updated when it is reset. Options are:

  - **Reset all Field Mapping Fields** – All fields are cleared of
    values
    
    **NOTE:** If the mapping is associated with a field group other than
    the default field group (\* or “All”), the Target Relationship ID
    field is not updated on a reset.

  - **Reset Status Fields only** – All fields retain values except for
    the Mapping Status and Rule Status, which are set to Pending Review.

To reset a mapping in AutoGen:

1.  Click the **Automation** tab in the Quick Panel.
2.  Click the **Mappings** icon for an Object.
3.  Select the mapping.
4.  Click the **Reset** icon in the Page toolbar.

The Mapping Status and Rule Status for the selected field mapping are
reset to Pending Review in Map on the *Field Mappings* page and the
mapper must make corrections and change the Mapping Status to Complete.

**NOTE:** When a user clicks the Reset icon in the Page toolbar, the
Created By field, on the *Vertical* View of the *Field Mappings* page in
Map, is updated to display the user name of the user who clicked Reset.
If the reset was performed in AutoGen, it is indicated. The Created On
field, on the *Vertical* View of the *Field Mappings* page, is updated
to reflect the date of the reset.

**NOTE:** The *Automation SQL Field Mappings* page displays behind the
*Automation* page and, depending on how the user’s view is configured,
may be obstructed by the *Automation* page itself.  In this case, to
view the *[Automation SQL Field
Mappings](../Page_Desc/Automation_SQL_Field_Mappings_H.htm)* page either
close the *[Automation](../Page_Desc/Automation_page.htm)* page or
reduce the size of the *Automation* page.
