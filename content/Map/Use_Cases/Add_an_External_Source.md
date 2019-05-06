# Add an External Source

An External Source is an Update Row Source that is external to the
system used in the Add Row Source when establishing a relationship. For
example, a finance system may create vendor information, but the
invoicing information is managed in another system. To support relevancy
rules, the user must link the systems together.

A Source is designated as an External Source when the user adds a Source
to a Target in Target Design with a Source type of External Source.

When an External Source is used, the External Source ID field on the
[Field Mappings](../Page_Desc/Field_Mappings_H.htm) page must be
populated with the Source ID.

An External Source is not treated as an Add Row Source, and is not
synced from Target Design when the Target is synced. It must be added on
the <span style="font-style: italic;">[Target Source (Update
Row)](../Page_Desc/Target_Sources_Update_Row.htm)</span> page and
configured manually.

To add an External Source:

1.  Add the External Source to the Target in Target Design. Refer to
    [Assign a Source to a
    Target](../../Design/Use_Cases/Assign_a_Source_to_a_Target.htm) for
    more information.

2.  Click <span style="font-weight: bold;">ProcessArea</span> in the
    <span style="font-style: italic;">Navigation</span> pane in Map.

3.  Click <span style="font-weight: bold;">Targets</span> on the
    *[Process Area Launch](../Page_Desc/Process_Area_Launch_map.htm)*
    page.

4.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.

5.  Click the <span style="font-weight: bold;">Update Row Sources</span>
    icon for a Source.

6.  Click <span style="font-weight: bold;">Add</span> on the
    <span style="font-style: italic;">Target Sources (Update Row)</span>
    page.
    
    [View the field descriptions for the Target Sources (Update Row)
    page](../Page_Desc/Target_Sources_Update_Row.htm)

7.  Select the External Source from the
    <span style="font-weight: bold;">Source ID</span> list box.
    
    **NOTE:** Select the External Source added in Target Design.

8.  Select the Source table from the
    <span style="font-weight: bold;">Source DATABASE OBJECT</span> list
    box.

9.  Click <span style="font-weight: bold;">Save</span>; the
    <span style="font-style: italic;">Vertical</span> View displays.

10. Click <span style="font-weight: bold;">Save</span> and navigate back
    to the <span style="font-style: italic;">Horizontal</span> View.

11. Click the <span style="font-weight: bold;">Mappings</span> icon for
    the External Source.

12. Click **Vertical View** for each field mapping for the External
    Source.

13. Select the name of the External Source in the
    <span style="font-weight: bold;">External Source ID</span> list box.

14. Click <span style="font-weight: bold;">Save</span>.
