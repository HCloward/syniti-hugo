# Page Design Guidelines

Follow these steps to design a fully implemented page with all available
and relevant features to ensure a high-quality user experience for both
business users and site administrators.

  - When naming pages:
      - Use parentheses rather than hyphens to delineate the description
        of the page, e.g., Request (Role) rather than Request – Role.
      - Pluralizing page names is acceptable.
  - If applicable, determine an Update and Insert method relevant to the
    page’s underlying data set. For simple record sets, solely
    Horizontal Updates/Inserts may be sufficient. If the record requires
    several or lengthy fields to be filled out, a *Vertical* View is a
    good page supplement. If the fields to be filled out are dependent
    on a choice made on the *Horizontal* View, a dynamic substituted
    vertical view is a good option. Refer to [Dynamic Views for Multiple
    Control Fields](Dynamic_Views_for_Multiple_Control_Fields.htm) for
    more information.
  - Add in all Page Column Properties to ensure the page flow is user
    friendly. *Vertical* Views should make use of tabs and labels to
    avoid the use of vertical scrolling. *Horizontal* Views should
    utilize Rowspan and Colspan to ensure the record length doesn’t
    exceed a reasonable resolution. Prioritize important text-based
    contextual information on the left, and actions on the right. Refer
    to [Assign Column Properties](Assign_Column_Properties.htm) for more
    information.
  - Determine which column(s) comprise a logical representation of the
    record set. Create or modify the Page Column to check “Show In
    Navigation”, which causes a secondary text color to be applied to
    them, visually indicating to the user that these columns are a
    representation of the record’s identity. This also causes them to
    show up concatenated within the Navigation pages. Refer to [Enable
    Show in Navigation](Enable_Show_in_Navigation.htm)  for more
    information.
  - Review existing WebApp Groups. Determine which groups apply to the
    page and apply them. Ensure that the relevant groups have a valid
    navigation path to the page. Refer to [WebApp Group
    Design](WebApp_Security_Group_Design.htm) for more information.
  - Create any control status modifiers (DCV, PCV, UCV, Control Status
    Field) adjustments required to ensure that only the relevant fields
    are editable in the right contexts.
  - Identify any columns whose meaning cannot be easily inferred by
    context. A bit field like “Enable Advanced Tracing” should contain
    Column Help to indicate to the user what this field does.  Refer to
    [Add Column Help Text](Add_Column_Help_Text.htm) for more
    information.
  - Identify which columns may benefit from a watermark, such as list
    boxes that search for particularly named values/objects. Watermarks
    can display the expected formats to ensure that the user understands
    what’s expected. Also, suggested text formats can be useful. If the
    user is expected to use a namespace convention, indicating it during
    the add/edit is more useful than providing a warning after the save.
    Refer to [Add a Watermark](Add_a_Watermark.htm) for more
    information.
  - Identify which columns may benefit from a tooltip, such as on images
    that represent a status. When a user hovers over the icon, the
    status displays. For instance, a red light in a column called
    “Status” could have a tooltip that displays “X templates failed to
    process." A tooltip can also be useful when a field is disabled
    because prerequisites have not been met. If a “Submit” button is
    disabled because the record is “Inactive”, then the tooltip can
    state “Disabled due to being inactive.” Refer to [Add a
    Tooltip](Add_a_Tooltip.htm) for more information.
  - Identify which columns may benefit from implementing a Default View.
    If there’s any input that can be inferred based on drill-down
    criteria or other environment information, it should be included in
    a default view. Input formats should be conveyed via Watermark,
    whereas defaults or suggested values should be conveyed via
    Defaults.
  - Identify which columns may contain data that should be translated.
    Because of potential for translation overhead as well as the Pareto
    principle, cell (and other) translations are opt-in. For example, if
    a list box within the application has the options “Active” and
    “Inactive,” any application string literals or user input that may
    be used as configuration should be translated. However, do NOT
    translate everything by default. This results in a slower page load
    and a more encumbered cache. Refer to [Use Catalogs During
    Application Development](../Sys_Admin/Use_Cases/Use_Catalogs.htm)
    for more information.

Consider which supplemental page features are relevant for the page.

  - Support Download – A page, such as a metric-related page, may be
    useful to download, while a page containing sensitive information
    may not.
    
      - If Download is supported, are there fields, such as mages and
        buttons, that shouldn’t be included in the downloaded file?
        These fields can be excluded i.e., hidden via View Type on the
        *[Page Columns](../Sys_Admin/Page_Desc/Page_Columns_H.htm)*
        page. Refer to [Set Column Control
        Status](Set_Column_Control_Status.htm) for more information.
      - Alternatively, are there fields that should be included on the
        Download page that are not available on the horizontal or
        vertical? Hide fields using the page columns All Views view
        type, but then enable them on the Download for this level of
        control. Refer to [Enable File
        Upload/Download](Enable_File_Upload_Download.htm) for more
        information.

  - Support Report – Is this a page that can provide additional
    information about this record and/or its children? A page with the
    Support Report feature enabled shouldn’t solely contain the
    information that could be obtained via a download.  
    If the page supports reporting:
    
      - Should an alternative view be used for the report? If the
        columns on the *Horizontal* View differ greatly from the columns
        on the report, create a separate view to avoid bloat to the
        standard *Horizontal* View.
      - As with Download, which columns should be shown, and which can
        be ignored? Which should be added for reporting purposes?
      - Should Report Groups be used to include child records per
        reported item? If the page already has a link to a subpage that
        should be included, the link can be configured to “Report
        Follows Link” to append children data to this page’s report.
        Refer to [Include all Page Details in
        Report](Include_All_Page_Details_in_Reports.htm) for more
        information.

  - Does Search (System Admin feature) need to be enabled?

  - Persistent Insert – When the user navigates to this page, is it
    likely they will add several records at once? If so, enable this
    option.

  - Support Direct Update – Direct update allows a user to enable or
    disable a check box without having to edit the page. Enable this
    setting if there is a check box(es) on the page, and updating the
    check box(es) is commonly the only change that a user makes on the
    page. Disable this setting if it is expected that the user will
    update additional information on the page.

  - Allow Explicit Quick Link – If this page requires binding to
    function correctly ([Page Control View](Page_Control_View.htm) for
    example) then this should be unchecked. If not, it can be enabled.

  - <span style="color: #000000;">Should the page support Excel
    upload?</span> If so, what columns should be available to upload?

  - Are there any List Filter-enabled combo or list boxes on the page?
    Are there fields to add to supplement the List Filter feature? For
    example, layout pages within System Administration generate a
    Template Preview exclusively for the “Filter (Control)” view type so
    that there’s a visual example of what to expect when using that
    particular value. Refer to [Add List Boxes and Combo
    Boxes](Add_List_Boxes_and_Combo_Boxes.htm) for more information.

  - Are there fields that should not be filterable? Perhaps there are
    columns to filter against that do not exist in the page’s view. For
    example, the Messages page contains a “Date Received” datetime
    property on the Filter panel, which allows filtering on a range of
    Date Time values, even though this field is not present on the
    *Horizontal* View. Control which fields can be used as a filter on
    the *[Page Columns](../Sys_Admin/Page_Desc/Page_Columns_H.htm)*
    page’s *Vertical* View for a column with the View Type of Filter
    (Form).

  - Does the page contain referential data to another application that
    can be implicitly secured? For example, if the application is meant
    to supplement functionality based on a Wave, bind the Wave security
    definition shipped with Console to the page. When a user is granted
    access to a particular Wave, the user can view and edit data in the
    WebApp that relates to that Wave.

  - Does the page need Dynamic Subtitle to explain the core concept of
    what the user will be doing on this page? Applications like Automate
    use Page Subtitle on their landing page to give a brief explanation
    of the application’s usage. Dynamic Subtitle is defined on the
    *Catalog Page Help* page’s *Vertical* View (Admin \> Catalogs \>
    WebApps \> Pages \> Page Help),

  - Would the page benefit from a Hover View? When a record is selected
    on the page, if the user hovers the cursor over the page title,
    after a brief delay, the record’s keys display by default in the
    Information pane (below the *Navigation* pane). These values are
    usually GUIDs, which are meaningless to the end user. The Hover View
    can be populated with additional technical information about the
    selected record.

  - Finally, test the page performance under load while reviewing the
    Page Performance Monitor, accessible from any DSP® page by pressing
    Shift+Ctrl+K. Use the Page Performance Monitor results to determine
    which portions of the page run slowly when the record set (or user
    set) increases dramatically. The page Designer must know the
    anticipated largest reasonable record set. Some pages can be
    complex, and may affect a few records, whereas others may display or
    process tens of thousands.

**NOTE:** Being functionally complete does not mean code complete. It’s
possible the page behaves correctly until it is scaled. The Designer may
implement the page in a more efficient way. This happens often in
application design, regardless of the development medium.
