# Create a View in SQL Server

For data to be extracted from a component and posted to SAP via
Integrate, a view must be created in SQL Server. This view serves as the
basis of Process Template Loop Field Mappings.

Create a view manually, or use the Auto Generate Database Objects
feature to automatically create a view with all fields required to
support the template type. Refer to
*<span style="color: #0000ff;font-style: normal;">[Generate Database
Objects
Automatically](Generate_Database_Objects_Automatically.htm)</span>* for
detailed information.

Once a view and corresponding tables have been added, populate the
tables with data to be used in the posting process.

The following tips will assist the manual creation of views that
facilitate successful posts:

  - Where possible, use one column to uniquely identify each row in the
    view. It is best if this column is a Primary Key column on the table
    and is the first column in the view.
  - Be aware of user settings for data fields. Unlike Direct Loads and
    BAPIs, the date and quantity field formats for BDCs are based on the
    settings of the user running them. Dates are typically sent to BDCs
    in the format MMDDYYYY rather than YYYYMMDD, which is how they are
    stored in the tables. Convert the dates using a substring statement.
  - Use an exclamation mark instead of NULL to blank out a field. Using
    NULL in the field name leaves the existing contents in place. 
  - Ensure none of the fields being concatenated to create the unique
    key are NULL. A concatenated field value of NULL causes the entire
    field to be set to NULL. Keys should be datatype nvarchar.

If the structure being created is a Detail BDC Structure, a Primary Key
field containing a unique key in the view
**<span class="underline"><span style="color: #ff0000;">must</span></span>**
be included. If creating a Header/Detail/Footer BDC Structure, include
the following two fields in the view:

  - **Primary Key** – Key that defines when the new transaction begins.
  - **Secondary Key** – Header key concatenated to a detail key that
    makes the field unique.

An example of a Primary/Secondary Key scenario is Purchase Orders. The
Header Key would contain  
POType + PONumber + Plant and the Secondary Key would contain POType +
PONumber + Plant + POLineItemNumber.
