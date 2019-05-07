+++
title = 'Create a Category'
solution = 'Data Quality'
+++

# Create a Category

A process Designer performs this task.

A category is a collection of governance elements and is created to
organize business processes and related elements by the category (e.g.,
Line of Business, Business Unit or Division, Data Domain). Duplicate
categories are not permitted.

**NOTE**: A user can auto-generate request-related objects for a
category. However, if a category already has its Content WebApp and
database built, there is no reason for the Designer to use the
auto-generate request-related objects feature. It is recommended that
the Designer ensure that a page has been selected in the Request Page Id
list box on the *[Category](../Page_Desc/Category_H.htm)* page’s
*Vertical* View. The auto-generate feature will detect whether
request-related objects exist and will not create them again if they
already exist. Refer to [Auto-generate Request-related
Objects](Auto_Generate_Request_related_Objects.htm) for more
information.

To create a category in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Design** in the *Navigation* pane.

2.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.
    
    *<span style="color: #365F91;">[View the field descriptions on the
    Category page.](../Page_Desc/Category_H.htm)</span>*

3.  Enter a unique name in the **NAME** field.

4.  Select a value from the **DEFAULT WEB APP ID** list box.
    
    **NOTE:** A specific DEFAULT WEB APP ID may only be assigned to one
    category. A validation message displays if the chosen WebAppID has
    already been assigned to another category.
    
    **NOTE:** For the Content WebApp to display in the DEFAULT WEB APP
    ID list box:
    
      - An Administrator must have registered the data source in the
        platform.
      - The current user must have a BOA Tools license for the Content
        WebApp and have the ability to change it.

<!-- end list -->

1.  Enter a brief description in the **DESCRIPTION** field.

2.  Click **Save**; *Vertical* View displays.

3.  Select the page used to enter request data in the Content WebApp in
    the <span style="font-weight: bold;">Request Page Id</span> list
    box.
    
    **NOTE:**  All pages created in the Content WebApp
    display.<span> </span>

4.  Select an owner from the **Owner**  list box.
    
    **NOTE:** To save the record successfully, one of the DSP® users in
    this list must be selected.
    
    **NOTE**: The list is limited to those users with a valid email
    address in the DSP®.
    
    **NOTE**: Once the owner is assigned, the child elements inherit the
    category owner as a default if another owner is not assigned.

5.  Enter text in the **Comment** field.
    
    **NOTE**: The comments are information about the category.
    
    **NOTE**: The values on the Tasks, Roles, Scenarios and Business
    Processes icons indicate the number of elements of each type that
    have been created.<span> </span> When a category is created, these
    numbers are 0 which indicates none of these elements have been
    created.

6.  Click <span style="font-weight: bold;">Save</span>.
