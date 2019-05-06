# Work With Sources Overview

Source types in the DSP® are:

  - Add Row Source
  - Update Row Source
  - Full Construction Source
  - External Source

An <span style="font-style: italic;font-weight: bold;">Add Row
Source</span> is the Source table where records are migrated from and
inserted into the Target table. Records in an Add Row Source table are
used for reconciliation. An Add Row Source is added in Target Design.
Refer to [Assign a Source to a
Target](../../Design/Use_Cases/Assign_a_Source_to_a_Target.htm) for more
information.

As an example, if an Add Row Source has 1000 records, 1000 records load
into the Target system. Add Row Sources must have a unique identifier,
which can be the legacy key field or a combination of legacy key fields
(also called a multipart key).

<span style="font-style: italic;font-weight: bold;">Update Row
Sources</span>, added in Map, have a number of uses, most commonly
attributes from an Update Row Source are used in the Add Row Source. For
example, in the SAP Target system, the Telephone2 field is on the same
table (LFA1) as all the other address fields. But the Source system
Northwind has a Supplier Add Row table and the 2nd Telephone number is
stored on the SupplierTelephone table. SupplierTelephone is an Update
Row Source, as it will update a field on the Supplier table. If applied
to the Northwind Source system, it follows the naming conventions:

stLFA1\_Northwind\_Supplier.zTELF2 copies from
stNorthwind\_SupplierTelephone.Telephone.

An Update Row Source can also be used for relevancy. The Add Row Source
may have a series of filters that must be applied. If the requirement is
to migrate vendors with only open purchase orders, then the table that
contains the purchase order status serves as an Update Row Source. If
applied to the Northwind Source system it follows the naming
conventions:

stLFA1\_Northwind\_Supplier.zOpenPO joins to stNorthwind\_POHeader where
Status=Open.

Refer to [Update Row Sources Overview](Add_Update_Row_Sources.htm) for
more information.

<span style="font-weight: bold;">NOTE:</span> The joins between Source
systems must be defined if Map cannot auto derive them. The logic to
automatically derive the join is based on the key fields on the Add Row
Source. For example, SupplierID is a key on stLFA1\_Northwind\_Supplier.
If SupplierID exists on the Update Row Source, Map builds the join. If
Map cannot find a matching field, a relationship is still created and
the user is notified during a mapping that the joins must be
established. Refer to [Add Relationship Joins to
Sources](Add_Relationship_Joins_to_Source.htm) for more information.

The system adds a Source of
<span style="font-style: italic;font-weight: bold;">Full
Construction</span> in Target Design when the user adds a Source with a
Source data source of {Full Construction}. Refer to [Full
Construction](../../Construct/Use_Cases/Full_Construction.htm) for more
information.

An <span style="font-style: italic;font-weight: bold;">External
Source</span> is an Update Row Source that is external to the system
used in the Add Row Source when establishing a relationship. Refer to
[Add an External Source](Add_an_External_Source.htm) for more
information.

This section contains the following topics:

  - [Add Add Row Sources](Add_an_Add_Row_Source.htm)
  - [Update Row Sources Overview](Add_Update_Row_Sources.htm)
  - [Add an External Source](Add_an_External_Source.htm)
  - [Use the Add Row Source Override Field with Update Row
    Sources](Use_the_Add_Row_Source_Override_Field_with_Update_Row_Sources.htm)
  - [Add Relationship Joins to
    Sources](Add_Relationship_Joins_to_Source.htm)
  - [Add ZActive Fields](Add_ZActive.htm)
  - [Add an Assemble Where Clause](Add_Assemble_Where_Clause.htm)
  - [Update Client and Language for all
    Sources](Update_Client_and_Language_for_all_Sources.htm)
  - [Copy a Target Source to Another
    Target](Copy_a_Target_Source_to_Another_Target.htm)
  - [Work with Target Sources that have Multi-part
    Keys](Work_with_Sources_with_Multipart_Keys.htm)
