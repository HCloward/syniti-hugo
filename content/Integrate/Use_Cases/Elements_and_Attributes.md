# Elements and Attributes

If the user selects **Element** in the **ELEMENT ATTRIBUTE** list box on
the *Structure Field* page, the field is added as a sub-element to the
structure element.  If the user selects **Attribute** in the **ELEMENT
ATTRIBUTE** list box, the element is added as an attribute to the
element. 

Using the following XML snippet as an example:

 

\<Customer\>

              \<Name\>Back Office Associates\</Name\>

              \<Address\>123 Main Street\</Address\>

\</Customer\>

The structure would be set up with an Element Name of “Customer” and the
Structure would have two fields, both set as Elements.  These fields
would have outputs of “Name” and “Address”.

Integrate generates this XML snippet if the user added a structure with
the name **Customer** on the *Structure* page, then clicked **Fields**
and added two elements with the values **Name** and **Address** in the
**Name** and **Output** fields.

 

Using the following XML snippet as an example:

 

\<Customer Name=”BackOffice Associates”\>

              \<Address\>123 Main Street\</Address\>

\</Customer\>

 

The structure would be set up with an Element Name of “**Customer**” and
the structure would have two fields, one set as an attribute and one set
as an element.  A field with an Output of “**Name**” would be set as an
attribute while a field with an Output of “**Address**” would be set as
an element. 

The user can add an attribute to an element by clicking the
**Attribute** button once the element is saved. On this page, the
**PRIORITY**, **NAME**, **DESCRIPTION**, and **OUTPUT** display of the
attribute can be set.  As an example:

\<Customer\>

              \<Name\>Back Office Associates\</Name\>

              \<Address Country=”US”\>123 Main Street\</Address\>

\</Customer\>

The field with an output of “**Name**” would have an attribute added
from the *File Structure Field Element – Attribute* page with an output
of “**Country**”.
