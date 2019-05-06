# Include DSP® Pages Listed on *Template (Objects)* Page

When CTSing a template, include all the DSP® pages listed on the
*Template (Objects)* page in dspCompose™  in the Packing List.

To include DSP® pages in the CTS:

1.  Create a CTS package that contains a CTS Item for each page and add
    CTS Item Keys. Refer to [Create Package and Build Archive in Source
    Instance](../../../Platform/Sys_Admin/Use_Cases/CreatePckgeBuildArcSrceInstance.htm)
    for detailed information.
    
    1.  When adding CTS Items to the package, select **CranSoft-Page**
        from **CTS CONFIG ITEM ID** list box.
    
    2.  When adding the CTS Item Keys for the Items, select the WebApp
        where the page resides from **Value** list box for WebApp ID
        Name. Type the first letters of the template name (e.g., If
        template is named “MM01\_0917,” type “MM01”) in the **Value**
        combo box for Page ID Name and choose one of the pages that has
        been created on the source for the template.
    
    **NOTE**: The CTS Items list is complete when there is a CTS Item
    for every page listed on the *Template (Objects)* page for the
    template.

2.  Click **Build Packing List** button.

3.  Click **Packing List** to review what is included. Compare this list
    to the objects on the *Template (Objects)* page.
    
    **NOTE**: Views associated with the pages added in step \#1 are
    automatically included in the Packing List.
    
    **NOTE**: The remaining objects listed on the *Template (Objects)*
    page that were not included in the Page Packing List must be
    included in a separate CTS package.

4.  Create a CTS package for the remaining objects listed on the
    *Template (Objects)* page.
    
    1.  Select **CranSoft-SQL** from **CTS CONFIG ITEM ID** list box and
        add the following objects:
        
          - The tx Posting View
        
          - Any stored procedures listed on *Template (Objects)* page
        
          - Any other views that have been created in the source to
            process the template that have not been included in the
            CranSoft Pages Archive

5.  Import all archives for the dspCompose™ template to the target
    system.

6.  Recompile objects for the dspCompose™ data source and any other data
    sources affected by the imports (within System Administration,
    navigate to Data Sources, select DATA SOURCE NAME and click
    Recompile Objects).
    
    **NOTE**: The recompile objects process should detect any missing
    SQL objects.
