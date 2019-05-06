# User Control Views

Business rules may require specific functions to be disabled based on
the logged in user. A *User Control* page can be created to manage the
criteria for a User Control View. **UserControl Views** (UCV) are
created in SQL and determine if records can be added, edited, deleted or
even viewed by a specified user. Once the views are created in SQL, they
need to be registered to the page in DSP® and the control criteria must
be defined. A single User Control View can control multiple pages in a
WebApp if designed correctly and registered to multiple pages.

Refer to [Control Views](Control_Views.htm) for general information.

When creating User Control Views (UCV):

  - Use the naming convention **webXXXUcv**, where **XXX** is the name
    of the table assigned to the page minus the prefix.
  - If using one UCV across multiple tables, **XXX** is a meaningful
    name.

**NOTE:** When controlling multiple pages with a single User Control
View, Enforce Strict Naming might need to be turned off depending on the
naming convention on the view.

  - Use a UCV when the control status determinations are to be made
    based on what is known about the User.
  - Include the following columns:
      - **boaUserID** – Contains DSP®  User ID
      - **boaColumn** – Technical name of column on the page
      - **boaControlStatus** – Control Status: disabled (0), enabled (1)
        and hidden (2)

**NOTE:** Besides the DSP® Reserved Words, no other columns are
considered when applying the UCV control status settings to a page.

Setting up user control views involves the following steps:

1.  Create a User Control View in Management Studio.
2.  Register the view in DSP®.
3.  Define the control criteria on the new page.

The following steps are optional to allow management of the control
view’s functionality:

1.  Create a User Control table.
2.  Create a User Control Horizontal View to manage the criteria.
3.  Register the Page in DSP® and assign to the Configuration Menu.
4.  Create list views for the Column Properties.
5.  Assign Column Properties.
