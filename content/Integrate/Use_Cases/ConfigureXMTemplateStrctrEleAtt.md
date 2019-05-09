+++
title = 'Configure an XML Template with Structures, Elements and Attributes'
solution = 'Platform'
+++

# Configure an XML Template with Structures, Elements and Attributes

<span id="Create and Transfer XML files Steps" class="popUpLink">Review
the steps to create and transfer XML files. </span>

An XML template, when added to a process and posted, will create an XML
file. Though a User Defined template, the registration of an XML file
varies from the setup of a Fixed Width or Delimited template as an XML
file has several additional options. 

**NOTE**: Begin template creation on the *Template* page in *Horizontal*
View. Refer to [Create a Basic Template](Create_a_Basic_Template)
for more information.

**NOTE**: The steps below describe adding structures and elements for
Vendor Master data in SAP as an example only. How a user adds structures
and elements depends on how the generated XML file should display. The
user should outline the hierarchy of the XML file prior to defining it
in Integrate.

To add structures to an XML template on the *Vertical* View of the
*Template* page:

1.  Select **XML** in the **User Defined Template Type** list box.

2.  Click **Save**.

3.  Click **Edit**.

4.  Click **Configuration** tab.

5.  Select \[**None**\] from the **Fixed Width Pad Location** list box.

6.  Click **Save**.

7.  Click **General** tab.

8.  Click **Define**.
    
    *View the field descriptions for the Structure page.*
    
    **NOTE**: The *Structure* page displays a Root Node record that
    cannot be deleted and is the first level in the XML file’s
    hierarchical structure. The **Fields** button is disabled for this
    record. No fields can be added for this structure. Fields are added
    to child structures. 
    
    **NOTE**: The Root Node’s priority is set to 1. The priority sets
    the order the structure appears in the generated XML file. Integrate
    automatically sets the priority for all structures.  A user cannot
    update the priority.

9.  Click **Edit**.

10. Enter a name for the structure in **NAME**. In the example, the user
    entered **VENDORS**.
    
    **NOTE**: All of the child structures in the file, with
    corresponding elements and attributes, appear below this Root Node
    when Integrate generates the XML file.

11. Enter additional information about the structure in **Description**.
    In the example, the user entered **Vendor Master**.

12. Enter a name that is the first level of the hierarchy in the XML
    file to be generated in **ELEMENT NAME**. The user entered
    \<**VENDORS**\>.
    
    **NOTE**: The **Element Name** is used when mapping the template to
    data via a process and is the name of the element in the resulting
    XML file.  After the structure is saved, the Element name displays
    in the *Horizontal* View surrounded by the tag characters \<\>. 
    
    **NOTE**: Because XML is a hierarchical structure, each element
    added to the template must be added as a child of an existing
    structure. 

13. Click **Add Child Structure**.
    
    **NOTE**: The new structures display in the order they were added on
    the *Structure* page. The **PRIORITY** field indicates which child
    structures are below others in the hierarchy. For example, the root
    node (VENDORS) structure’s priority is 1. A child structure (also
    called an element) added to this structure is assigned a priority of
    1.1. Another child structure (element) added to the root node
    structure has a priority of 1.2. The child structures for Vendor
    Information and General Data is added in the steps below. Integrate
    assigns a child structure added to an element the priority of 1.1.1.

14. Enter a name for the structure in **NAME**. The user entered
    **Vendor**.

15. Enter additional information about the structure in **DESCRIPTION**.
    The user entered **VendorInformation**.

16. Enter a name in **ELEMENT NAME**. The user entered \<**Vendor**\>

17. Click **Save**.
    
    **NOTE**: The first child structure (Vendor) displays with the
    priority 1.1 and displays beneath the parent structure (VENDORS).
    The Element Name is indented below the Root Node.

18. Click **Add Child Structure** for the Root Node.

19. Enter a name for the structure in **NAME**.  The user entered
    **General Data**.

20. Enter additional information about the structure in **DESCRIPTION**.
    The user entered **General Data**.

21. Enter a name in **ELEMENT NAME**. The user entered
    \<**GeneralData**\>.

22. Click **Save**.
    
    **NOTE**: The second child structure (General Data) displays with
    the priority 1.2 and at the same level in the hierarchy as the first
    child structure (Vendor) added (with the priority 1.1).

23. Click **Add Child Structure** for a structure. The user selected
    **General Data**. 

24. Enter a name for the structure in **NAME**. The user entered
    **Address**.

25. Enter additional information about the structure in **DESCRIPTION**.
    The user entered **VendorAddressInfo**.

26. Enter a name in **ELEMENT NAME**. The user entered \<**Address**\>.

27. Click **Save**.
    
    **NOTE**: Integrate assigns this child structure (Address) a
    priority of 1.1.1
    
    Once these structures have been added and saved, the *Structure*
    page displays with the data.

To add fields (elements and attributes) to a structure:

1.  Click the **Fields** icon to add fields to the selected structure.
    The user selected **Address**.
    
    **NOTE**: If no fields have been added to an element the icon does
    not display a number.

2.  Enter a value in **PRIORITY**.
    
    **NOTE**: The **PRIORITY** sets the display order for the field in
    the XML document, if the field is an element.

3.  Enter a field name in **NAME**. The user entered **Street**.
    
    **NOTE**: The name is used when mapping the template to data via a
    process, so should be the equivalent of a column name in the view in
    SQL that contains the data to map. Refer to [Add Data to be Included
    in the XML file in SQL](AddDataIncludedXMLSQL) for more
    information. 

4.  Enter details about the field in **DESCRIPTION**. The user entered
    **Street Address**.

5.  Select an option in the **ELEMENT ATTRIBUTE** list box. The user
    selected **Element**.
    
    **NOTE**: Refer to [Elements and
    Attributes](Elements_and_Attributes) for more information.

6.  Enter the output of the field in **OUTPUT**. The user entered
    **street**.
    
    **NOTE**: The **OUTPUT** column allows a user to set how the Element
    or Attribute displays in the resulting XML file. 

7.  Click the **INCLUDE IF EMPTY** check box.
    
    **NOTE**: If the check box is selected and no value exists for the
    element, the field will still be included in the XML file.

8.  Click **Save**.
    
    **NOTE**: This page uses persistent insert, which means that when a
    user adds an element or attribute and saves it, an empty row
    displays ready to accept data for the next element or
    attribute.  Click **Cancel** to close persistent insert to
    configure attributes, if necessary.

9.  Click the **Attribute** icon if the field is an element (if
    **Element** has been selected in the **ELEMENT ATTRIBUTE** list
    box).
    
    **NOTE:** This example does not cover adding an Attribute.
    
    **NOTE**: If the field is an attribute, the **Attribute** icon is
    disabled. Refer to the  section for more information.

10. Enter a value in **PRIORITY**.
    
    **NOTE**: The **PRIORITY** sets the display order for the attribute
    attached to the element in the XML document. 

11. Enter an attribute name in **NAME**.

12. Enter details about the field in **DESCRIPTION**.

13. Click **Save**.
    
    **NOTE**: The **Fields** icon displays the number of fields added to
    each structure.

14. Navigate to the *Template* page's *Vertical* View.

15. Click **Documentation** tab.

16. Click **Report**.

17. Verify the structures and elements and attributes have been added to
    the template correctly.
    
    **NOTE**: Like the **Street** element added to the **Address** child
    structure in the example above, the **General Data** child structure
    had fields added. In this case, **VendorNumber**, **Name**, and
    **Search term** were added.

Once the user finishes adding the elements to this structure, and
completes the other steps necessary to create and transfer files,
Integrate generates the following XML file.
