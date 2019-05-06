# Create a View

**NOTE:** This section only applies to custom components and the three
delivered custom components: Construct, MC and dspCompose\_Data. Create
a view in a database on the DSP® database instance that returns the
values that represent the data items by which security can be
defined.  The view must follow the name convention: **web\*Sec**. 

These views should return all of the columns that are going to be
applicable in the security model.

The following view is an example of how to build a view to restrict
access on the Customers page to specific
CustomerIDs:

<span style="color: #0000ff;">CREATE</span><span style="color: #0000ff;">VIEW</span>
\[dbo\]<span style="color: #808080;">.</span>\[webCustomerIDSec\]

AS

<span style="color: #0000ff;">SELECT</span>     CustomerID

<span style="color: #0000ff;">FROM</span>         dbo<span style="color: #808080;">.</span>Customers

 

It is important to note here that 1 → n columns can be defined in the
Sec view, where *n* is the number of columns being used in defining
security. For this example, a second security view will be created that
grants record visibility based on ContactTitle and
City:

<span style="color: #0000ff;">CREATE</span><span style="color: #0000ff;">VIEW</span>
\[dbo\]<span style="color: #808080;">.</span>\[webContactTitleCitySec\]

AS

<span style="color: #0000ff;">SELECT</span><span style="color: #0000ff;">DISTINCT</span>
ContactTitle<span style="color: #808080;">,</span>
City

<span style="color: #0000ff;">FROM</span>         dbo<span style="color: #808080;">.</span>Customers

 

In addition to the columns that will be explicitly used in defining
security, designers can also include a column aliased as “FriendlyName,”
and the value returned in this column will be displayed to the on-site
administrators when they are deciding which values to assign to a role
or a user. The following is an example of security view with
“FriendlyName”:

<span style="color: #0000ff;">CREATE</span><span style="color: #0000ff;">VIEW</span>
\[dbo\]<span style="color: #808080;">.</span>\[webCustomerIDFriendlyNameSec\]

AS

<span style="color: #0000ff;">SELECT</span>     CustomerID<span style="color: #808080;">,</span>
CompanyName <span style="color: #0000ff;">AS</span>
FriendlyName

<span style="color: #0000ff;">FROM</span>         dbo<span style="color: #808080;">.</span>Customers
