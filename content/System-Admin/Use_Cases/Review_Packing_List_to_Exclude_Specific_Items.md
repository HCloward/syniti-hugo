+++
title = 'Review Packing List to Exclude Specific Items'
solution = 'Platform'
+++

# Review Packing List to Exclude Specific Items

Once the package is built, review the list of package items to exclude
specific items from the package.

To exclude items from the package:

1.  Verify the package was built.

2.  From the *[CTS Build](../Page_Desc/CTS_Build_H.htm)* page, click
    **Packing List**.

3.  Click the button corresponding to the type of item to review (All,
    User Defined, SQL Object, SQL Script, File, Folder, Data) on the
    *[CTS Packing List
    Summary](../Page_Desc/CTS%20Packing%20List%20Summary.htm)* page.

4.  To exclude the entire configuration item (for example, dspCompose –
    Team, CranSoft – SQL Object), click the **Exclude** button on the
    *[CTS Packing List](../Page_Desc/CTS_Packing_List_H.htm)* page or
    
    To exclude an individual packing list item, click **Exclude** on the
    *[CTS Packing List By Config
    Item](../Page_Desc/CTS%20Packing%20List%20Config%20Item.htm)* page.

**NOTE:** If the item needs to be added back to the package, return to
the *CTS Build* page and click the **Items** icon. The excluded items
display in the Items list with the Include check box unchecked. Either
check the Include check box or delete the specific Item that you want to
re-include. Then, rebuild the CTS Package using the Build Packing List
button on the *CTS Build* page.

**NOTE:** Once an archive is built, click **Manifest** on the
*[Archives](../Page_Desc/Archives_H.htm)* page to view the contents.

Continue with [Build an Archive from a
Package](Build_an_Archive_from_a_Package.htm).
